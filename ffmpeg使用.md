## 媒体转码

大多数视频网站的编码格式：

MP4封装：H264视频编码 + AAC音频编码

谷歌方案：

WebM封装：VP8视频编码 + Vorbis音频编码

others：（HTML默认支持，开源）

OGG封装：Theora视频编码 + Vorbis音频编码



**媒体文件转码默认语句举例**

```
ffmpeg -i input.mp4 output.flv
```



### 音频文件操作

.flac 转 .mp3

```bash
ffmpeg -i in.flac -acodec libmp3lame -ar 44100 -ab 320k -ac 2 out.mp3
```

其中 

`-acodec`: a为Audio缩写，codec为编解码器；-acodec libmp3lame 为选择mp3的编解码器（不写也可以，ffmpeg会自动匹配编解码器）

`-ar`: 设置音频采样率（不输入的话使用原音频的采样率）

`-ab`: 设置比特率（默认128k）

`-ac`: 设置声道数量（默认使用原音频的声道数）



使用 `ffmpeg -h` 查看可用参数中的 Audio部分

`-aframes` 设置音频帧数

`-aq` 设置音频的质量

`-an` 禁用音频

`-vol` 设置音频音量（默认256：100%音量）

`-af` 设置音频过滤器

![image-20210814141803717](https://tva1.sinaimg.cn/large/008i3skNgy1gtgalmy350j60pk0940tv02.jpg)



### 视频文件操作

举例 .webm -> .mp4

```bash
ffmpeg -i in.webm -s 1920x1080 -pix_fmt yuv420p -vcodec libx264 -preset medium -profile:v high -level:v 4.1 -crf 23 -acodec aac -ar 44100 -ac 2 -b:a 128k out.mp4
```

`-s` 输出视频的宽和高

`-pix_fmt` pixel format 的缩写，设置颜色空间; 可以使用 **ffmpeg -pix_fmts** 来查看所有的，网络视频大多使用的是 **yuv420p**

`-vcodec` 设置输出视频流的编码器指令；libx264是h264的软件编码器（通用、稳定），ffmpeg还支持硬件编码、GPU加速、多线程等等

`-preset` 编码器预设可以有以下10个参数可以选（可以改变编码算法的精度，精度越高，资源占用越高，编码速度越慢,  但体积会小一些）

```
ultrafast superfast veryfast faster fast
medium slow slower veryslow placebo
```

默认使用midium；录制视频一般使用veryfast；压制视频一般使用veryslow

`-profile:v` 制定编码器的配置，压缩比和画质的权衡；**[1,5.2]** ，越**高**画质越好

`-crf` 码率控制（constat rate factor 恒定速率因子模式）适用于对画质有要求，对空间无关紧要的情况，参数选择范围 **[0, 51]** ，数字越**小**质量越高，0就是无损画质，一般在**[18,28]** 之间做选择

`-r` 设置视频帧率，填写30就是设置视频每秒30帧

`acodec` 设置音频编码器

`-b` 等同于上面音频的 `-ab`



### 码率控制

画质越好，要求的码率也越高，文件体积也越大

也就是决定为每一个帧画面分配多少比特数，这是一个在权衡画面体积和画面质量，实际上ffmpeg一共支持三种码率控制控制模式

`-qp`（constant quantizer恒定量化器模式）利用算法讲画质转化为数字，这样每一帧画面的质量都可以通过这些量化参数来判定，这些量化参数是可以通过手动来设置的，在这种模式下，画质被分为 **[0,51]** 个级别，0就是无损画质

无损压缩的例子

**快速编码**

```bash
ffmpeg -i input -vcodec libx264 -preset ultrafast -qp 0 output.mkv
```

**高压缩比**

```bash
ffmpeg -i input -vcodec libx264 -preset veryslow -qp 0 output.mkv
```



`-crf` （最普及）也就是浮动的qp模式，对于每一帧分配不同的画质参数，对于人眼来说，前一帧高一些，后一帧低一些很难察觉出来，所以使用这种方法可以将码率稍微降低一些，然后把这些省下来的码率用在视觉敏感的画面中，这样一来画质的变化基本看不出来；可以手动设置浮动范围（一般都是默认）

**qp 与 crf 都是单遍编码，最好搭配 veryslow，参数控制更精准一些**



`-b` （bitrate 固定目标码率模式）输出结果固定的码率和大小的视频

默认采用 `VBR`（variable bit rate 动态比特率）：简单的内容少给点码率，复杂的内容多给码率

现在网络视频基本采用的是 `ABR`  （average bit rate 平均比特率）

`CBR` （conatant bit rate 恒定比特率）其实是在ABR的基础上附加一些指令，让码率基本固定在一个数值上（不推荐）



## 合并、提取音视频

**提取视频部分，不要音频**

```bash
ffmpeg -i in.mp4 -vcodec copy -an out.mp4
```

`-vcodec copy` 保持原编码格式



**剔除视频，只要音频**

```bash
ffmpeg -i in.mp4 -vn -acodec copy out.m4a
```

如果视频中有多条音频流比如

```bash
Stream #0:2[0x81]:Audio:ac3,48000 Hz,5.1,s16,384 kb/s
Stream #0:3[0x81]:Audio:ac3,48000 Hz,5.1,s16,384 kb/s
Stream #0:2[0x80]:Audio:ac3,48000 Hz,5.1,s16,384 kb/s
```

加入需要选出第二条那么就是在上面的语句中加入 `-map 0:3`



**将音视频合并**

将两个编码格式相符的音频和视频进行以下操作

```bash
ffmpeg -i in.m4a -i v.mp4 -c copy out.mp4
```

如果不相符需要改变编码格式的话就使用上面所说的编码语句来进行转码



**截取音频的某一段**

```bash
截取两个时间点使用 -to
ffmpeg -i in.mp3 -ss 00:01:00 -to 00:01:10 -acodec copy out.mp3

截取时长使用 -t
ffmpeg -i in.mp3 -ss 00:01:00 -t 10 -acodec copy out.mp3

从视频末尾截取
ffmpeg -sseof -10 -i input.mp3 output.mp3
```



**视频截取某一段**

```bash
ffmpeg -i in.mp4 -ss 00:01:00 -to 00:01:10 -c copy out.mp4
ffmpeg -ss 00:01:00 -i in.mp4 -to 00:01:10 -c copy out.mp4
ffmpeg -ss 00:01:00 -i in.mp4 -to 00:01:10 -c copy -copyts out.mp4
```

第一行和第二行的 `-i` 与 `-ss` 指令调换的位置，虽然只是命令的顺序不一样但是第二行使用了关键帧技术（加速操作），就是在指定的时间点附近自行设置起点终点，结果就有可能并不是期望的区间

为了避免这种状况就使用第三行的命令



**连接多个音视频**

```bash
ffmpeg -i '1.mp4|2.mp4|3.mp4' -c copy out.mp4
```



## 截图、水印、动图

**截图**

```bash
ffmpeg -i in.mp4 -ss 5 -vframes 1 img.jpg
```

截取第五秒`-ss`的第一帧`-vframes`图片



**添加水印**

```bash
ffmpeg -i input.mp4 -i img1.jpg -filter_complex "overlay=20:20" out.mp4
```

`-filter_complex`  用来添加滤镜； `overlay=20:20` 表示离左边20像素 离顶部20个像素



制作gif动图

```bash
ffmpeg -i input.mp4 -ss 7.5 -to 8.5 -s 640x320 -r 15 out.gif
```



**直播推流**

```bash
ffmpeg -stream_loop -1 -re -i input.flv -c copy -f flv "rtmp地址/直播码"
```


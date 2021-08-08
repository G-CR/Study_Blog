E: Unable to locate package vim

![image-20210808160714960](https://tva1.sinaimg.cn/large/008i3skNgy1gt9g1e2sgjj306o0100sk.jpg)

增加一条源地址在 **/etc/apt/sources.list** 文件末尾

> echo deb http://archive.ubuntu.com/ubuntu/trusty main universe restricted multiverse >> /etc/apt/sources.list

然后

> apt-get update

一下就可以使用apt install 来安装了

![image-20210808161156704](https://tva1.sinaimg.cn/large/008i3skNgy1gt9g68wnysj30tx0rz0z3.jpg)
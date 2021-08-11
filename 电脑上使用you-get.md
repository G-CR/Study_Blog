**1、前置安装 Python 3.x**

**2、先把pip升级到最新版本**

```bash
pip install --upgrade pip
```

**3、接着使用pip安装 you-get**

```bash
pip3 install you-get
```

4、正常来说可以已经可以使用了，可以使用一下语句测试一下

```
you-get https://www.bilibili.com/video/BV1F54y1H7eW
```

参数也很简单，直接 you-get + 视频链接 下载地址默认的是根目录

![正常运行截图](https://tva1.sinaimg.cn/large/008i3skNgy1gtd8sgdsrrj60vg0fswgx02.jpg)

5、如果没有运行成功，就在原本的语句中间加上一条 --debug 看一下报错信息是什么,如果最后一行是 TypeError 或者 HTTP Error 就自己检查粘贴的链接是否正确，如果报错信息中包含 CERTIFICATE_VERIFY_FAILED 就有以下解决方案

a、

```bash
pip3 install --upgrade certifi
```



b、x为自己电脑上Python版本，本语句目的是打开 **Certificates.command** 文件，mac外别的系统的路径可以自行查找

```
open /Applications/Python\ 3.x/Install\ Certificates.command
```

之后就可以运行上面的语句了



贴一个Python代码用于自定义保存位置和下载链接

```python
import sys
from you_get import common as you_get       #导入you-get库

directory = r'#####'                         #设置下载目录
url = '######'      #需要下载的视频地址
sys.argv = ['you-get','-l','-o',directory,url]       #sys传递参数执行下载，就像在命令行一样；‘-l’是指按列表下载，如果下载单个视频，去掉‘-l’即可；‘-o’后面跟保存目录。
you_get.main()
```




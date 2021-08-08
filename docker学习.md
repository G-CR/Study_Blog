##  常用命令

### 镜像相关

**查看镜像：** 

```
docker images
```



**安装镜像：**

```
docker pull ...(镜像名称)
```



**删除镜像：**

按照镜像ID删除镜像：

```
docker rmi ...(IMAGE ID，在docker images里面查看，每个镜像都包括的唯一ID)
```

删除所有镜像：

```
docker rmi `docker images -q`
```



### 容器相关

**查看正在运行的容器**

```
docker ps
```

**查看所有容器（不管是否运行）**

```
docker ps -a
```

**创建容器命令**

```
docker run 
```

$-i :$ 表示运行容器

$-t :$ 表示容器启动后会进入其命令行。加入 **-it** 这两个参数后，容器创建就能登录进去，即分配一个伪终端。

$--name:$  为创建的容器命名

$-v:$ 表示目录映射关系（前者是宿主机目录，后者是映射到宿主机上的目录），可以使用多个 **-v** 做多个目录或者文件映射。注意：做目录映射时，在宿主机上做修改，然后共享到容器上。

$-d:$ 在run后面加上 **-d** 参数，则会创建一个守护式容器在后台运行（这样创建容器后不会自动登录容器，如果只加 -**it** 两个参数，创建后就会自动进去容器）

$-p:$ 表示端口映射，前者是宿主机端口，后者是容器内映射端口。可以使用多个 **-p** 做多个端口映射

**举例：**

直接运行，占用命令行

```
docker run -it --name=mycentos centos bash
```

这种方式exit后容器直接退出



守护方式（后台）运行：

```
docker run -id --name=mycentos2 centos
```

后台运行的容器的调用

```
docker exec -it mycentos2 /bin/bash
```

停止运行容器

使用这种方法运行容器使用exit后容器会保存到后台，并不会直接退出,如果想要停止这个容器,那么就需要使用 **docker ps** 来找到这个进程，然后找到对应的 **CONTAINER ID** 之后使用

```
docker stop ...(当前的id)
```

就可以停止当前的容器了



如果想要启动某一个容器，那么就使用 **docker ps -a** 查询所有的容器，找到对应的 **CONTAINER ID** ，然后使用

```
docker start ...(对应ID)
```



**退出容器**

**-it** 运行的容器在exit后也就直接关闭了，而 **-id** 运行的容器还会停留在后台

```
exit
```



**删除容器**

```
docker rm ... (名称或者id都可以)
```





### 目录挂载

我们可以在创建容器的时候，将宿主机的目录与容器内的目录进行映射，这样我们就可以通过修改宿主机某个目录的文件从而去影响容器

创建容器 添加 $-v$ 参数后边为宿主机目录：容器目录， 举个例子：

```
docker run -id -v /User/gongchaorui/mydata:/usr/local/mydata --name=mycentos3 centos
```

宿主机中的挂载目录必须先在docker客户端中提前录入（ **setting -> Resources -> FILE SHARING** ）





### 安装一些常用的环境

MySql：一般来说 **docker pull mysql** 就够了，由于docker官方提供的MySQL没有arm64架构的，但是MySQL官方提供了mysql/mysql-server有，所以m1芯片的mac可以运行 **docker pull mysql/mysql-server** 

**启动容器**

```
docker run -id --name=mysql -p 3306:3306 -e MYSQL_ROOT_PASSWORD=root mysql/mysql-server
```



**运行容器**

```
docker exec -it mysql /bin/bash
```



**连接mysql**

```
mysql -uroot -proot --default-character-set=utf8
```




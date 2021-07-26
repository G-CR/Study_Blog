[参考视频](https://www.bilibili.com/video/BV1yJ411S7Wu)

在github中对项目进行搜索的时候，可以针对项目的 **名称、描述、readme、star数量、fork** 中的内容进行精确搜索（而不是直接在搜索框中输入笼统的名字出来一堆不感兴趣的东西）

下面列举的条件都可以**并行**使用

以Spring Boot为例

一、关键字出现的位置

1、出现在项目名中

```
in:name spring boot
```

![image-20210726190126767](https://tva1.sinaimg.cn/large/008i3skNgy1gsuk0n0ipij31f90u0wjy.jpg)



2、出现在readme中

```
in:readme spring boot
```

![image-20210726191414026](https://tva1.sinaimg.cn/large/008i3skNgy1gsukdwr750j31e10u0n30.jpg)



3、出现在描述中

```
in:description spring boot
```

![image-20210726191610313](https://tva1.sinaimg.cn/large/008i3skNgy1gsukfx2j3vj31e40u078x.jpg)





二、添加筛选条件

1、如果对项目的star数量也有要求，那么就直接在后面加上star的约束条件即可。加入需要筛选star数大于50000的项目

```
start:>50000
```

![image-20210726190734905](https://tva1.sinaimg.cn/large/008i3skNgy1gsuk6zca45j31f10u041k.jpg)



2、筛选 fork 数也是同理,筛选fork数量大于1000的项目就在后面加上

```
forks:>1000
```

![image-20210726191232842](https://tva1.sinaimg.cn/large/008i3skNgy1gsukc59ggbj31e80u0q82.jpg)

3、限制编程语言

假如需要查找项目名中为Spring Boot并且项目主要编程语言是python的项目,只需要在后面添加 language:python

```
language:python
```

![image-20210726191912939](https://tva1.sinaimg.cn/large/008i3skNgy1gsukj3zjagj31ep0u0gpz.jpg)

4、限制最后一次更新的时间

需要找到一些较新的项目，就需要添加筛选最后一次push的时间的条件，假如需要查找最后一次提交在2021年7月1日之后的项目，就需要在后面添加

```
pushed:>2021-07-01
```

![image-20210726192226558](https://tva1.sinaimg.cn/large/008i3skNgy1gsukmgdq3gj31eq0u0wjw.jpg)
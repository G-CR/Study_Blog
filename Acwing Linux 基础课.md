## homework 1 show

1. 常用命令介绍
    ctrl c: 取消命令，并且换行
    ctrl u: 清空本行命令
    tab键：可以补全命令和文件名，如果补全不了快速按两下tab键，可以显示备选选项
    ls: 列出当前目录下所有文件，蓝色的是文件夹，白色的是普通文件，绿色的是可执行文件
    pwd: 显示当前路径
    cd XXX: 进入XXX目录下, cd .. 返回上层目录
    cp XXX YYY: 将XXX文件复制成YYY，XXX和YYY可以是一个路径，比如../dir_c/a.txt，表示上层目录下的dir_c文件夹下的文件a.txt
    mkdir XXX: 创建目录XXX
    rm XXX: 删除普通文件;  rm XXX -r: 删除文件夹
    mv XXX YYY: 将XXX文件移动到YYY，和cp命令一样，XXX和YYY可以是一个路径；重命名也是用这个命令
    touch XXX: 创建一个文件
    cat XXX: 展示文件XXX中的内容

2. 创建作业 & 测试作业的正确性
    homework 1 create 可以重新创建所有lesson_1的作业
    homework 1 create id 可以单独创建lesson_1的第id个作业. e.g.
        homework 1 create 0 可以只重新创建lesson_1的第0个作业
    homework 1 test 可以评测lesson_1的所有作业

3. 作业
    创建好作业后，先进入文件夹/home/acs/homework/lesson_1/，然后：
    (0) 进入homework_0文件夹，分别创建文件夹dir_a, dir_b, dir_c
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_0$ ls
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_0$ mkdir dir_a
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_0$ mkdir dir_b
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_0$ mkdir dir_c
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_0$ homework 1 test
    ```
    
    (1) 进入homework_1文件夹，将a.txt, b.txt, c.txt 分别复制成: a.txt.bak, b.txt.bak, c.txt.bak
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_0$ cd ..
    acs@b5a0e56c53d4:~/homework/lesson_1$ cd homework_1
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_1$ ls
    a.txt  b.txt  c.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_1$ cp a.txt a.txt.bak
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_1$ cp b.txt b.txt.bak
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_1$ cp c.txt c.txt.bak
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_1$ ls
    a.txt  a.txt.bak  b.txt  b.txt.bak  c.txt  c.txt.bak
    ```
    
    
    
    (2) 进入homework_2文件夹，将a.txt, b.txt, c.txt 分别重命名为: a_new.txt, b_new.txt, c_new.txt
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_1$ pwd
    /home/acs/homework/lesson_1/homework_1
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_1$ ls
    a.txt  a.txt.bak  b.txt  b.txt.bak  c.txt  c.txt.bak
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_1$ cd ..
    acs@b5a0e56c53d4:~/homework/lesson_1$ cd homework_2
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_2$ ls
    a.txt  b.txt  c.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_2$ mv a.txt a_new.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_2$ mv b.txt b_new.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_2$ mv c.txt c_new.txt
    ```
    
    (3) 进入homework_3文件夹，将dir_a文件夹下的a.txt, b.txt, c.txt分别移动到文件夹dir_b下
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_2$ cd ../homework_3
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3$ ls
    dir_a  dir_b
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3$ cd dir_a
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3/dir_a$ ls
    a.txt  b.txt  c.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3/dir_a$ mv a.txt ../dir_b/a.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3/dir_a$ mv b.txt ../dir_b/b.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3/dir_a$ mv c.txt ../dir_b/c.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3/dir_a$ cd ..
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3$ cd dir_b
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3/dir_b$ ls
    a.txt  b.txt  c.txt
    ```
    
    (4) 进入homework_4文件夹，将普通文件a.txt, b.txt, c.txt删除
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3/dir_b$ pwd  
    /home/acs/homework/lesson_1/homework_3/dir_b
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_3/dir_b$ cd ../../homework_4
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_4$ ls
    a.txt  b.txt  c.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_4$ rm *  
    ```
    
    (5) 进入homework_5文件夹，将文件夹dir_a, dir_b, dir_c删除
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_4$ cd ../homework_5
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_5$ ls
    dir_a  dir_b  dir_c
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_5$ rm * -r
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_5$ ls
    ```
    
    (6) 进入homework_6文件夹，查看task.txt的内容，并按其指示进行操作
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_5$ cd ../homework_6
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_6$ ls
    task.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_6$ cat task.txt 
    将task.txt重命名为done.txt, 创建目录dir_a，将done.txt移动到目录dir_a下
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_6$ mv task.txt done.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_6$ ls
    done.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_6$ mkdir dir_a
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_6$ mv done.txt dir_a/done.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_6$ ls
    dir_a
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_6$ homework 1 test
    ```
    
    (7) 进入homework_7文件夹，创建文件夹dir_0, dir_1, dir_2，
        将a.txt, b.txt, c.txt复制到dir_0下，重命名为a0.txt, b0.txt, c0.txt;
        将a.txt, b.txt, c.txt复制到dir_1下，重命名为a1.txt, b1.txt, c1.txt;
        将a.txt, b.txt, c.txt复制到dir_2下，重命名为a2.txt, b2.txt, c2.txt;
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_6$ cd ../homework_7
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ mkdir dir_0 dir_1 dir_2
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ ls
    a.txt  b.txt  c.txt  dir_0  dir_1  dir_2
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp a.txt dir_0/a0.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp b.txt dir_0/b0.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp c.txt dir_0/c0.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cd dir_0
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7/dir_0$ ls
    a0.txt  b0.txt  c0.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7/dir_0$ cd ..
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp a.txt dir_1/a1.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp b.txt dir_1/b1.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp c.txt dir_1/c1.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ ls
    a.txt  b.txt  c.txt  dir_0  dir_1  dir_2
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cd dir_1
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7/dir_1$ ls
    a1.txt  b1.txt  c1.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7/dir_1$ cd ..
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ ls  
    a.txt  b.txt  c.txt  dir_0  dir_1  dir_2
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp a.txt dir_2/a2.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp b.txt dir_2/b2.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp
    cp     cpgr   cpp    cpp-9  cppw   
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cp c.txt dir_2/c2.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ ls
    a.txt  b.txt  c.txt  dir_0  dir_1  dir_2
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7$ cd dir_2
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7/dir_2$ ls
    a2.txt  b2.txt  c2.txt
    ```
    
    (8) 进入homework_8文件夹，分别在dir_a, dir_b, dir_c文件夹下查看task.txt的内容，并分别按照指示进行操作
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_7/dir_2$ cd ../../homework_8
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8$ ls
    dir_a  dir_b  dir_c
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8$ cd dir_a
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_a$ ls
    a.txt  task.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_a$ cat task.txt 
    将a.txt删除
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_a$ rm a.txt 
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_a$ cd ..
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8$ cd dir_b
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_b$ ls
    b.txt  task.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_b$ cat task.txt 
    将b.txt重命名为b_new.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_b$ mv b.txt b_new.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_b$ ls
    b_new.txt  task.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_b$ cd ..
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8$ cd dir_c
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_c$ ls
    c.txt  task.txt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_c$ cat task.txt 
    将c.txt复制成c.txt.bak
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_c$ cp c.txt c.txt.bak
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_c$ ls
    c.txt  c.txt.bak  task.txt
    ```
    
    (9) 进入homework_9文件夹，将其中所有txt类型的文件删除
    acs@b5a0e56c53d4:~/homework$ 
    
    ```bash
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_8/dir_c$ cd ../../homework_9
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_9$ ls
    file_0.dmg   file_11.txt  file_14.doc  file_17.ppt  file_2.doc   file_22.doc  file_25.ppt  file_28.dmg  file_4.dmg  file_7.txt
    file_1.ppt   file_12.dmg  file_15.txt  file_18.doc  file_20.dmg  file_23.txt  file_26.doc  file_29.ppt  file_5.ppt  file_8.dmg
    file_10.doc  file_13.ppt  file_16.dmg  file_19.txt  file_21.ppt  file_24.dmg  file_27.txt  file_3.txt   file_6.doc  file_9.ppt
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_9$ rm *.txt 
    acs@b5a0e56c53d4:~/homework/lesson_1/homework_9$ ls
    file_0.dmg  file_10.doc  file_13.ppt  file_16.dmg  file_18.doc  file_20.dmg  file_22.doc  file_25.ppt  file_28.dmg  file_4.dmg  file_6.doc  file_9.ppt
    file_1.ppt  file_12.dmg  file_14.doc  file_17.ppt  file_2.doc   file_21.ppt  file_24.dmg  file_26.doc  file_29.ppt  file_5.ppt  file_8.dmg
    ```
    
    ![image-20210821204733101](https://tva1.sinaimg.cn/large/008i3skNgy1gtop71yloqj60j20bsdh902.jpg)
    
    
# vim - 1 - # 存活下来

存活下来🥊

## 更新 apt 源，升级 vim

## `vim` 是什么

- `vim` 是类 `unix` 系统上的一个文本编辑神器，在 `Linux` 系统环境中也被许多程序员使用，书写程序和文档。
- 我们本次课程将围绕 `Vim` 进行全面的介绍及学习。

## 工欲善其事，必先利其器

- `vim` 在环境中，已经默认安装好了，我们可以直接使用。在使用前，我们先对它进行升级，升级后会有更好的功能体验。

下面打开终端，输入以下命令，进行升级：

\#首先是更新源sudo apt update#然后是升级vimsudo apt install vim

## 运行vim

在升级完成后，我们再通过命令运行 `vim`。

vim

## 进入 `vim` 的基本界面

![vim1-1](https://i0.hdslb.com/bfs/article/9eda67c4c389bcc027cdf6eefdcd2fa31f8aaf57.jpg@942w_767h_progressive.webp)

- `vim` 默认的模式 是 `Normal mode(正常模式)`
- 这个时候你会发现按回车、空格等按键，都是没有用的

## 退出vim

## 我想要退出vim

- 我输入ctrl+c尝试退出
- 系统进行如下提示📕

![vim1-1](https://i0.hdslb.com/bfs/article/292df59779db0dd4656a5b6b9f30475a78c80dfb.jpg@942w_761h_progressive.webp)

- 左下角可以看到系统的提示

- - 下面我们只需按照系统提示进行操作，输入 `:quit<Enter>` 退出 `vim`

## 尝试退出 `vim`

- 按照提示依次输入 `:quit`

- - 输入 `:` 时，输入的内容显示在屏幕的左下角
    - `:` 的输入，让 vim 的模式从 `Normal mode（正常模式）`，变成了  `Command-Line mode（命令行模式）`
    - 如果输入内容在主编辑窗口的话，需要先esc进入 `Normal mode（正常模式）`
    - `:` 的输入让左上角的绿色光标消失
    - 左下角随着键盘的输入，将显示字符
    - 注意 vim 对于大小写是敏感的，我们使用半角英文字符

- 输入完 `:quit` 后，按回车执行这个 `:quit` 命令

- 执行命令 `:quit` 命令

- 退回到 `shell`

- 别小看这一步

## 多少人倒在了这里

![vim1-1](https://i0.hdslb.com/bfs/article/87a7bfcb0af0c4dfacd308e955c0b7901f21a426.jpg@942w_761h_progressive.webp)

## 第一步

- 迈出第一步是最难的
- 截止到2021/8/3
- 8年多来，239万人卡在vim里
- 退出Vim编辑器甚至成为了开发者之间的一个笑话

## 发展趋势

- 国内趋势

![vim1-1](https://i0.hdslb.com/bfs/article/e1815aafae86ceed22b3418ecea0369fbd1a8363.png@942w_414h_progressive.webp)

- 国外趋势

![vim1-1](https://i0.hdslb.com/bfs/article/af370eb8e81ce3e8576d954813170205a66cf50c.png@942w_495h_progressive.webp)

- 那些图形界面还是占用资源过多
- 还需要系统gui的支持
- 微软拥抱开源只是姿态
- 商业巨头还是想垄断行业、标准、语言、思想

## 总结

- 升级了 vim
- 进入了 vim
- 退出了 vim
- 多少人倒在了这一步

![vim1-1](https://i0.hdslb.com/bfs/article/d42d545e0f0e141ae0c673446236aa1438d0d760.png@942w_777h_progressive.webp)

## 这就是我们对于 vim 最初的接触。恭喜您存活了下来！

- vim 还有什么好玩的呢？🤔
- 我们下次再说！*



# vim - 2 - # 使用帮助

回忆上节课内容

- 更新和运行 vim
- 进入和退出 vim
- 存活了下来
- 从中我们知道 vim 有两种模式：正常模式（Normal mode）和命令行模式 （Command-Line mode）
- 为了您能更好在 `vim` 中生存，必须给您更强大的工具🔧 -- 帮助手册
- vim 有没有可以用的帮助系统呢

\#首先进入vimvim

## 使用帮助文件📕

- 进入 `vim` 之后，我们面对的是正常模式

- 输入半角:进入 `命令行` 模式

- 什么不会，就 `:help` 什么

- - 比如说 `:quit` 不会
    - 就 `:help` 这个 `:quit`
    - 输入 `:help :quit`
    - `:help` 的对象是 `:quit`，中间留了一个空格
    - 回车之后执行命令

- 我们查到 `:q[uit]` 就是退出当前窗口

- 方括号中的内容可以省略

- 也就是说可以用 `:q` 这种简写形式来退出

![vim-help-1](https://i0.hdslb.com/bfs/article/935d5f7559b0476eb1a44ccf5123b2b028b9edf1.png@942w_764h_progressive.webp)

- 可以用 `:q` 退出当前帮助📕

- 再用 `:q` 退出 vim

- 注意输入 `:` 的时候

- - 左手的小拇指先按下Shift
    - 右手的小拇指再按一下;
    - 左手小拇指抬起
    - 记住这个手法
    - 多练几次

## 查看一下关于 :help 自己的帮助

- 我们上次 `:help` 了 `:quit`

- - `:help :quit` 可以查询什么是 `:quit`

- 原则就是

- - 什么不会，就 `:help` 什么

- 那么 `:help` 本身不会怎么办呢？

- 什么不会就 `:help` 什么

- - `:help` 不会就 `:help :help`
    - `:help :help` 可以查询 `:help` 自己的帮助

![vim-help-1](https://i0.hdslb.com/bfs/article/0cf8ec6172b69ae1aad46ae70fbf0e63f6879a62.png@942w_768h_progressive.webp)

- `:help` 完整写法位为 `:h[elp]`

- - 中括号里面的东西是可以省略的
    - 可以简写为 `:h`
    - 或者直接用功能键F1
    - 注意功能键只能在字符模式下能用
    - 桌面模式下不能用

- 我们可以 `:q` 退出帮助

- 然后 `:h` 再进入帮助

- `:help :help` 可以简写为 `:h :h`

- 那我能问问关于正常模式 `(Normal mode)` 的事情吗？🤔

- 行动起来！！！👊

## 查看关于模式的帮助

- `vim` 是有状态的编辑器 `(modal editor)`
- 所处的状态不同
- 进行同样键盘录入
- 具体执行的效果不同

\#使用 help 查询帮助:help Normal#或者把 help 简写成 h :h Normal

![vim-help-1](https://i0.hdslb.com/bfs/article/b8f1912f5e2b9a61776022b9dbd9eef0fff273c7.png@942w_1254h_progressive.webp)

## 我们可以看到 vim 总共有 6 种基本模式

- 正常模式 `(Normal mode)`

- - 也叫默认模式。
    - 进入 `vim` 时默认的模式所有输入的键都直接对应着命令
    - 也被叫做命令模式.

- 插入模式 `(Insert mode)`

- - 任何键盘录入都会插入到当前文档中

- 可视模式 `(Visual mode)`

- - 很像正常模式
    - 但是移动命令会改变选中的一块高亮区域
    - 执行的命令会对选定范围进行

- 选择模式 `(Select mode)`

- - 可以用鼠标或光标键高亮选择文本
    - 任何输入都会替换选择的高亮文本
    - 并进入插入模式

- 命令行模式 `(Command-Line mode)`

- - 可以窗口下方执行一条命令
    - 一般是通过:执行单行命令
    - 通过/和?进行搜索

- Ex mode  `(多行命令执行模式)`

- - `Ex` 指的是 `Execute`
    - 在 `Normal` 正常模式下使用gQ进入
    - 使用 `:visual` 退出

## 总结

## 我们这次了解了基本的帮助操作

- 什么不会就 `:help` 什么

- `:help` 命令有两种写法

- - 完整 `:help`
    - 简写 `:h`

- `vim` 有六种基本模式

- 我们现在还没有写过文件呢呀，怎么写呢？🤔

- 还得下次再说！*

# vim - 3 - # 打开文件

打开文件🔖

## 回忆上节课内容

- 什么不会,就 `:help` 什么

- 命令有完整和简写两种模式

- - `:help` 和 `:h`
    - `:quit` 和 `:q`
    - 注意`:`是左右手小拇指配合输入的

- `vim` 有 `6` 种基本模式

- 但是我们还没有打开过文件

## 创建一个文件📒

\#首先对于当前文件夹进行 ls 列表操作ls -l .#然后把ls的结果，输出到 oeasy.txt 中ls -l . > oeasy.txt#使用cat查看 oeasy.txt 的内容 cat oeasy.txt

![oeasy_list](https://i0.hdslb.com/bfs/article/9a8a7b6add6aefa918a6a7808619a0a87127f7a1.png@942w_705h_progressive.webp)

## 打开

## 用 `vi` 打开一个 `oeasy.txt`

vi oeasy.txt

- 我们可以看到在`标准屏幕(80*24)`上
- 显示出了 `oeasy.txt`
- 当前 `vim` 处于 `正常模式（Normal mode）`

![vim_oeasy](https://i0.hdslb.com/bfs/article/836c5e74ad345736d7941a088dea97e150c93cca.png@942w_710h_progressive.webp)

- 我怎么才能知道 vim 当前编辑的是哪个文件呢？🤔

## 使用帮助命令

- 键入:

- - 把模式从正常（Normal）切换到命令行（Command-Line）

- 使用 `:file`

- - 可以在状态栏看到当前文件的信息
    - `:file` 有详细的帮助吗？
    - 输入命令 `:h :file`，查一下

![help_file](https://i0.hdslb.com/bfs/article/ba6a5148faeaedea6b11d7d3d9bc0dfd06f9f293.png@942w_710h_progressive.webp)

- `:f[ile]`可简写为

- - `:fi`
    - `:f`

- 使用ctrl+G也有同样的作用

## 总结

- 我们制作了 `oeasy.txt`
- 我们用 `vim` 打开了 `oeasy.txt`
- 我们分析了 `vi` 环境基本结构
- 我们用 `:f[ile]` 查询了当前文件的信息
- 这个帮助系统好像挺有用
- 还可以获得更多的帮助吗？🤔
- 下次再说！*

# vim - 4 - # 深入帮助

## 深入帮助📕

## 回忆上节课内容

- 上次制作了 `oeasy.txt`
- 用 `vim oeasy.txt` 打开了文件
- `:f[ile]` 查询了当前文件 🔖 的信息
- 从 `正常模式或命令模式(Normal mode)` 切换到 `命令行模式 (Command-Line mode)` 要使用:
- 从 `命令行模式（Command-Line mode）` 按回车执行命令，执行完了就回来了

![mode](https://i0.hdslb.com/bfs/article/440f89a2ff1f28808c61784e2d76fc5036aa7067.png@942w_636h_progressive.webp)

- 我们已经可以在两个模式（`命令模式`、`底线命令模式` 模式）之间切换
- 我们这次想要了解更多的帮助信息

## 运行帮助📕

## 在 `vim` 中运行 `:help`

![help move](https://i0.hdslb.com/bfs/article/9f0af461846ba61b126f27e750a061154a6154a9.png@942w_674h_progressive.webp)

- 我们可以使用h、j、k、l进行移动
- 方向如上图所示
- 这个时候 `hjkl` 不是输入字符而是移动方向的命令
- 不光是这四个字符
- 所有的键盘字符都对应命令
- 这就是为什么默认的正常模式 `(Normal mode)` 也被称作命令模式

## 命令模式

- 命令模式可以直接按键来执行命令
- 比如移动
- 还有很多各种命令

GIF

![help move](https://i0.hdslb.com/bfs/article/0cfcae47854e492ed03c1ff8bc727efb85a690cc.gif@1s.webp)

- 命令模式 `(Normal mode)` 和 命令行模式 `(Command-Line mode)` 不同

- - 命令模式 `(Normal mode)` 直接按键执行
    - 而命令行模式 `(Command-Line mode)` 在底部行输入命令后按回车执行*

- 模式不同，对应的操作不同

- 这也是 `vim` 上手最难的原因

## 学习曲线

![help move](https://i0.hdslb.com/bfs/article/7bd890e32eb62144d2eafd37c06921c55ce2d3d0.jpg@816w_551h_progressive.webp)

- vim 是公认的非常陡峭的学习曲线
- 不过突破上去了之后，效率是相当高的
- 多易必多难
- 最开始看起来容易的东西，比如 ide
- 什么都给你配好了，但是你对于底层完全失去了理解和控制，到最后反而是最难
- 我们一点点翻越这陡峭的山，征服 vim

**但是为什么是h、j、k、l对应方向呢？**

## 起源

- `vim` 起源于 `vi`
- `vi` 早期是 Bill Joy 在 `adm3A` 上制作和使用的
- `adm3A` 是一台终端
- `adm3A` 的键盘没有方向键
- 所以这个习惯就延续的到了今天⚠️

![help move](https://i0.hdslb.com/bfs/article/a3a2c50e8873ce991ddbe18b964011d66bbc6864.jpg@942w_840h_progressive.webp)

- 我们可以看到上图键盘上的h、j、k、l按键上面对应的方向

**现在还需要用h、j、k、l按键控制光标么？**

## 键盘核心区

**是的！🤓 现在还可以使用h、j、k、l按键控制光标。**

- 在使用 vim 时，咱们可以把手放在键盘核心区有助于提高效率

- - 将左手食指放在f上
    - 将右手食指放在j上

![help move](https://i0.hdslb.com/bfs/article/fad77232134a1f95b29f5675c97502cb38d11726.jpg@942w_522h_progressive.webp)



在上面图片中展示的现代 101 键盘中有加入了方向键：

- 在右手的右下面的非核心区
- 笔记本键盘方向键也需要物理移动手的位置
- 所以这种移动会降低效率，那我们能用鼠标定位么？

## 使用鼠标🐭

想在 vim 中使用鼠标控制，我们先需要进行基本的配置：

- 首先我们在 vim 中搜索帮助，输入 `:h mouse`，可以看到如下图所示的界面：

![help move](https://i0.hdslb.com/bfs/article/d45916187c57e3889b5b769f753365cd02077f5c.png@942w_674h_progressive.webp)

- 现在我们进行主题设置

- 从上图中我们可以看到，vim 提示我们执行 `:set mouse=a`，就可以用鼠标了！！！

- - 我们可以使用鼠标移动光标
    - 使用滚轮可以翻页
    - 还可以使用鼠标点击相关的主题链接

这些现代科技真的很不错，使用鼠标后操作更便捷了，但是鼠标其实会更**影响效率**，因为鼠标会让我们的手离开键盘。

然而 `vi` 就是想让用户可以实现，手不离开键盘核心区域就完成所有的编辑工作：

- 方向移动是最常用的操作
- 他想让你相对灵活的右手位置在键盘核心区完全不动
- 只需要按下手指就完成相应的移动操作
- 而且比鼠标还快速

## 位置记忆

- 用 l 来表示右边很难记忆
- 怎么办呢？有用户想到了这个

![图片描述](https://i0.hdslb.com/bfs/article/d067ba742cb47508c7b43b9da48669f8e6056f80.png@942w_260h_progressive.webp)

- 东 洛杉矶
- 南 爪哇岛
- 西 黄河
- 北 共青城

![图片描述](https://i0.hdslb.com/bfs/article/cea0d6deac1965d44b28ce3ba5ca988d71cd58f7.png@618w_432h_progressive.webp)

- 用熟了其实很简洁
- 逐渐将操作变成肌肉记忆，不要走脑子

**现在我们有一个新问题，当年在没有鼠标的时候，Bill Joy 是如何跳转超链接主题的呢？**

## 键盘跳转

![help move](https://i0.hdslb.com/bfs/article/5776f545e25052e3c048b7ed6b0f837d2e3e7761.jpg@942w_678h_progressive.webp)

- 运行 `:help` 回到主题开头
- 我们可以看到 `bars` 这样的链接
- 使用h、j、k、l移动光标
- 把光标移动到链接上
- 是ctrl+]就可以**跳入链接**
- ctrl+o可以**跳出链接**，回到原位置 `older position`
- 我们可以试试反复跳跃🤸‍♀️

## 两套手册

- 在翻阅 vim 的 manual 的时候
- 我们发现 vim 有两套 manual

![图片描述](https://i0.hdslb.com/bfs/article/cc0f57a23cbdf1f936667c91c7556acbe4edfc4e.png@942w_374h_progressive.webp)

## 用户手册

![图片描述](https://i0.hdslb.com/bfs/article/6d4108c7b414ebc80772caeafe81cf829e74d427.png@942w_911h_progressive.webp)

- 一套是用户手册

- - 像一本书一样
    - 从头读到尾
    - 从简单到复杂
    - 适合初学

## 引用手册

![图片描述](https://i0.hdslb.com/bfs/article/962fd360d7b2cb4cf14ec98c63978b08a67c68e9.png@942w_761h_progressive.webp)

- 另一套是引用手册

- - 精确的描述每个主题
    - 以及主题内容是如何工作的
    - 适合查询

## 总结

- 我们这次看了

- - 正常模式
    - 命令行模式
    - 以及他们切换的方式

- 了解了帮助文件的正确打开方式

- h、j、k、l命令的历史来源

- 在文档中使用鼠标(并不建议)

- 使用全键盘方式跳入跳出超链接

- 帮助文件的两种手册

- 不过说到这里我们还是没改文档啊啊啊啊！😓

- 好饭不怕晚？🤪

- 我们下次再说！*



# vim - 5 - # 插入模式

## 插入模式 

## 回忆上节课内容

![mode](https://i0.hdslb.com/bfs/article/440f89a2ff1f28808c61784e2d76fc5036aa7067.png@942w_636h_progressive.webp)

- 我们总结了，模式切换的方式

- - 命令模式 `Normal mode`
    - 底线命令行模式 `Command mode`

- 帮助文件的正确打开方式

- - `:h`

- 在文档中使用鼠标

- - `set mouse=a`
    - 建议不用鼠标

- 使用全键盘方式跳入跳出超链接

- - <kbd>ctrl</kbd>+<kbd>]</kbd>
    - <kbd>ctrl</kbd>+<kbd>o</kbd>

- 帮助文件的两种手册

- - 用户帮助手册
    - 引用帮助手册

- 这次我们来插入内容，修改文档

## 插入模式

## 想要插入内容的话，应该进入插入模式 `(Insert mode)`

- 首先我们还是打开上次的那个 `oeasy.txt`

```
ls -l . > oeasy.txt vi oeasy.txt
```



- 然后如何进入插入模式呢？
- 我们使用 `:help insert` 看看是否有什么命令

![insert mode](https://i0.hdslb.com/bfs/article/eddf2dc4a7e50c52c01093cd1b74ba0b3f606c42.png@942w_723h_progressive.webp)

- 我们需要先退出帮助模式

- - `:q`

- 然后按下 <kbd>i</kbd> 进入插入模式

- 进入插入模式后

- - `左下角` 状态栏会显示 **`-- 插入 --`**
    - 这意味着已经进入了插入模式
    - 时刻留意左下角
    - 左下角就像小地图一样
    - 是统管全局的所在

![insert mode](https://i0.hdslb.com/bfs/article/7aec94f6ca4f7b0be388d95f665fe02a9f9ce16a.png@942w_117h_progressive.webp)

- 如果没有进入插入模式的话

- - 可能因为处在新开的帮助中
    - 先 `:q` 退出帮助

## 插入文字🅰️

- 插入模式下我们可以任意打字
- 按键不再是命令而是输入字符
- 冒号回车都能打出来🤪

![insert oeasy](https://i0.hdslb.com/bfs/article/c75595efb67f0f1dd1c357adb2e262ce613bf7dc.png@942w_710h_progressive.webp)

- 输入完成之后，又想要移动位置怎么办呢？

- - <kbd>esc</kbd> 退回到命令模式 `Normal mode`
    - 或者 <kbd>ctrl</kbd>+<kbd>c</kbd> 回到命令模式 `Normal mode`
    - 尽量选择 <kbd>ctrl</kbd>+<kbd>c</kbd> 因为可以让双手保持正位
    - 左手小指 <kbd>ctrl</kbd> + 右手食指 <kbd>c</kbd>

- 注意退回到命令模式后

- - 左下角状态栏不再显示 **`-- 插入 --`**
    - 而是变回空白

- 观察左下角

- 时刻注意

## 文件细节

![图片描述](https://i0.hdslb.com/bfs/article/813ee5f02cfb7a59320f8ed795e9976bce625e74.png@942w_414h_progressive.webp)

- 注意有内容的地方是具体的文字内容
- 在没有内容的地方
- 前面会有 `tilder(~)` 进行提示
- `tilder(~)` 意味着空行，就是啥都没有

## 使用 `i` 命令进入插入模式

- 按 <kbd>i</kbd> 再次进入插入模式
- 按 <kbd>esc</kbd> 或 <kbd>ctrl</kbd>+<kbd>c</kbd> 退回到命令模式

![force quit](https://i0.hdslb.com/bfs/article/2e2024d2b32df86d260796dcd3a7f2672512a45c.png@942w_636h_progressive.webp)

- 可以用 <kbd>i</kbd> 和 <kbd>ctrl</kbd>+<kbd>c</kbd> 反复切换模式
- 观察左下角

## 帮助细节

- `i` 到底什么意思？
- 可以 `:h` 他一下
- `:h i` 就是 `help` 一下 `i` 命令究竟做些什么

![图片描述](https://i0.hdslb.com/bfs/article/aaf746dd82d0fc5da9c8c1785f70e64972656362.png@942w_269h_progressive.webp)

- 那 <kbd>ctrl</kbd>+<kbd>c</kbd> 是啥意思？

## 查询快捷键

- 什么不会就 `:h` 什么
- `:h ctrl-c` 就是帮助我们查找一下 `ctrl-c` 快捷键究竟做些什么

![图片描述](https://i0.hdslb.com/bfs/article/ab30ceee638e9e4d144d752aea7abdb4ca77e9e9.png@942w_105h_progressive.webp)

- 同理还有 `:h ctrl-g`

![图片描述](https://i0.hdslb.com/bfs/article/4c199fffa928c9d83d21e3da3dbb0ab6742acd73.png@942w_330h_progressive.webp)

- <kbd>CTRL</kbd>+<kbd>G</kbd> 对应着 `:f[ile]` 命令
- 可以查看当前文件信息

## 尝试退出

- 输入 `:q` 希望退出
- 但是屏幕 📟 显示如下

![force quit](https://i0.hdslb.com/bfs/article/b7c3b6f7ee57dae91aa17242af544a8dd80106ab.png@942w_90h_progressive.webp)

- 按照他的要求输入 `:q!`
- `cat oeasy.txt` 显示文件并未修改😧
- 原来 `:q!` 只是不保存，强制quit退出
- 囧，虽然还没成功保存...
- 但是曾经真的插入文字了！😃
- 我们先总结一下📘

## 总结

- 我们这一次进入了插入模式
- 在正常模式下使用命令 <kbd>i</kbd>
- 在插入模式下使用 <kbd>esc</kbd> 退回到正常模式
- 使用 `:q!` 不保存强制退出
- 哎～看来保存只能下次再说了 😅
- 我们下次再说！*





# vim - 6 - # 保存修改

## 另存与保存 

## 回忆上节课内容🤔

![force quit](https://i0.hdslb.com/bfs/article/2e2024d2b32df86d260796dcd3a7f2672512a45c.png@942w_636h_progressive.webp)

- 我们上次进入了插入模式
- 从正常模式，按<kbd>i</kbd>，进插入模式
- 从插入模式，按<kbd>ctrl</kbd>+<kbd>c</kbd> 退回到正常模式
- 这次我们想想应该如何保存这个文件

```
ls -l . > oeasy.txt vi oeasy.txt
```



## 保存文件

- 首先要查询 `save` 相关的帮助📕
- `:h save`
- 只是找到了 `saveas {file}`
- 这一看就是 `另存为` 啊

![force quit](https://i0.hdslb.com/bfs/article/ca48b6be91fb1e2b31008ba10e615264f1825b0b.png@942w_710h_progressive.webp)

- 我们来试一下 <kbd>i</kbd> 进入插入模式
- 随便打字 🅰️
- 然后另存为 `:saveas o2z.txt`
- 这个 `o2z.txt` 是 `saveas` 的参数,也就是保存的文件名
- 然后退出 `:q`

```
cat o2z.txt
```



**可以看到另存的 `o2z.txt` 真的被保存下来了！🤪，但是能否直接保存当前文件呢？**

## 直接存储

- 我们再次打开 `oeasy.txt`
- 我们继续查帮助 `:h save`
- 往上翻

![force quit](https://i0.hdslb.com/bfs/article/72ef8729537e7f3dfc745a7f63d1d4c841db18e6.png@942w_717h_progressive.webp)

## write 命令

- 找到了一个 `:w[rite]` 命令

- - 复杂写法是 `:write`
    - 简单写法是 `:w`

- 我们再对文件进行修改

- 注意文件名 `oeasy.txt[+]` 中那个 `[+]`，就是有修改但是未保存的标志

- 然后 `:w`

![write](https://i0.hdslb.com/bfs/article/dff67a2fd723cf8d4c768ba2111898317705e317.png@942w_701h_progressive.webp)

## 左下角状态栏

我们查看右下角状态栏显示了：

- 文件名
- 行数
- 字符数
- 如果没显示，就 `:file`

## 这时候我们再退出

- 我们先执行操作 `:q` 再执行 `cat`查看 `oeasy.txt`
- 真的已经被修改了！！！🤪

## 总结

- 这次我们学会了另存为命令 `:saveas {file}`
- 还有直接保存命令 `:w`
- 真的可以把修改的内容保存了😃
- 还有什么可玩的？🤔
- 我们下次再说！*



# vim - 7 - # 从头插入

## 另存与保存

## 回忆上节课内容🤔

- 上次我们学会了另存为命令 `: saveas {file}`
- 还有这个直接保存命令 `: w`
- 真的可以把修改存了 😀

![force quit](https://i0.hdslb.com/bfs/article/72ef8729537e7f3dfc745a7f63d1d4c841db18e6.png@942w_717h_progressive.webp)

**下面我们来研究插入命令的细节。**

## 插入命令

- 首先我们可以查询这个插入命令的帮助📕
- `:help insert`
- 简写为 `:h i`

![force quit](https://i0.hdslb.com/bfs/article/cfdc68e56471c29f69646fa4f75f1a3de8e98ddc.png@942w_707h_progressive.webp)

- 我们可以看到小写 `i` 是在当前光标的前面插入

## 切换模式

- 我们可以i进入插入模式

- esc回到正常模式

- 然后反复切换

- 观察状态栏下面的提示

- - `--插入--` 就是插入模式
    - 啥都没有就是正常模式

## 重复插入

- 我们可以先点击i进入插入模式
- 输入 `oeasy 空格`
- ctrl+c回到正常模式
- 在正常模式下，按下.可以重复刚才的操作
- 再按下.可以再重复刚才的操作
- 还按下.可以还重复刚才的操作
- 这个.是什么意思
- `:h .`

![图片描述](https://i0.hdslb.com/bfs/article/767b37038a7632315d6ec1ef85771b9c5b55695d.png@942w_458h_progressive.webp)

## 撤销插入

- 在正常状态下按下u可撤销操作

- - 按一次u撤销一步
    - 再按u再撤销
    - 还按u还撤销
    - 一直u按到头，就撤销到头

- 查询帮助

- `:h u`

![图片描述](https://i0.hdslb.com/bfs/article/a4f8a70bce107f82059caa17d07d196f78137cbc.png@942w_396h_progressive.webp)

- 撤销了之后又反悔了可以么？

## 重做

- 反悔是重做

- 就在 `u` 的帮助下面有介绍

- ctrl+r

- 在正常状态下按ctrl+r可撤销撤销操作

- 就是重做

- - 按一次u撤销一步
    - 再ctrl+r再撤销撤销
    - 按一次u撤销一步
    - 再ctrl+r再撤销撤销
    - 好像可以来回来去拉锯

## 在前方插入

- 比如我们的光标当前所在的位置，在 `用` 字的位置
- 按下i进入到插入模式
- 然后就在绿色的光标前面插入字符
- 这就是所谓的 `before cursor` 的意思
- 就是插在光标之前

![force quit](https://i0.hdslb.com/bfs/article/be00497bf565afc43908b8cc45ff90db9768d07a.png@942w_710h_progressive.webp)

## 插在最前面

- 在 `:h i` 帮助的周围可以有命令 `I`
- 如果我们使用大写的 `I`，不管你的光标在什么位置
- 插入位置在光标所在行所有文本的 **最** 前面
- 然后切换到插入模式

## 总结

- 我们这次深入了i命令

- - i在当前的光标之前插入
    - I在本行文本的最前面插入

- 还有一些常用的编辑命令

- - .重做
    - u撤销
    - ctrl+r还原

- 关于插入，还有什么讲究吗？🤔

- 我们下次再说！*



# vim - 8 - # 追加文本

## 追加文本

## 回忆上节课内容🤔

- 我们这次深入了i命令

- - i在当前的光标之前插入
    - I在本行文本的最前面插入

- 还有一些常用的编辑命令

- - .重做
    - u撤销
    - ctrl+r还原

- 关于插入，还有什么讲究吗？🤔

![force quit](https://i0.hdslb.com/bfs/article/2e2024d2b32df86d260796dcd3a7f2672512a45c.png@942w_636h_progressive.webp)

## 类似的命令

- 还有没有和插入相关的的命令呢？？🤔
- 相类似的命令一定在手册的同一个地方！🤨
- 我们得还在插入命令的附近找找

## 插入命令

- 首先我们找到插入命令的帮助📕
- `:help insert`
- 简写为 `:h i`

![force quit](https://i0.hdslb.com/bfs/article/cfdc68e56471c29f69646fa4f75f1a3de8e98ddc.png@942w_707h_progressive.webp)

**我们向上翻可以找到 `a` 命令。**

## 追加文本

![force quit](https://i0.hdslb.com/bfs/article/a582859aaa2b69608febc1ea466fb6258b0e2424.png@942w_710h_progressive.webp)

- `i` 和 `a` 都是 `Insert mode commands`

- 插入位置

- - `i` 是 `before cursor` 在光标前插
    - `a` 是 `after cursor` 在光标后插

- 对应命令

- - `i` 意思是 `insert`
    - `a` 意思是 `append`

## 切换模式

- 我们可以a进入插入模式

- esc回到正常模式

- 然后反复切换a、esc

- 观察左下角提示

- - 左下角有`--插入--` 就是插入模式
    - 左下角啥都没有就是正常模式

- 这就和i、I很像

## 重复、撤销、重做

- 我们可以i进入插入模式
- 输入 `oeasy 空格`
- ctrl+c回到正常模式
- 按几次.重复一下插入操作
- u可以撤销
- ctrl+r可以重做

## 练习

- 如果我有个网页源文件如下图
- 光标在当前绿色的位置
- 如果我想在上个感叹句之后插文字，应该用什么命令呢？

![force quit](https://i0.hdslb.com/bfs/article/b564f314e428b90b867838bc4ddf2fdd98b442e3.png@942w_713h_progressive.webp)

- 应该用 `i`
- 在当前的光标之前插入
- 如果我想在整行文本之前插入呢？应该用什么？
- 用 `I`
- 在光标所在行文本的最前面插入
- `:h I`

## 继续练习

- 但如果我的光标在下图的位置呢？
- 我想在叹号后面插入内容

![force quit](https://i0.hdslb.com/bfs/article/8a48986823fbd2fd2117e424d9b06ecdd13483ad.png@906w_312h_progressive.webp)

- 这个时候应该用 `a`
- `after cursor` 在光标之后所在的叹号之后插入文字
- 如果我想在本行最后插入呢？
- 用 `A` 在本行 **最后** 插入
- `:h A`
- 就像用 `I` 在本行最前面插入一样

## 追加写入

- 如果我们保存了当前文件 `oeasy.log`

- 然后退出了 vi

- 然后重新进入 vi

- 在一个未命名文件中写一些东西，比如

- - `oeasyo2zo3z`

- `:w >> oeasy.log`

- - 这就是用追加的方式去写这个log文件
    - log中的东西还都有
    - 最新的追加在最后

- 与 `:w oeasy.log` 对比

- - `:w oeasy` 是覆盖写入
    - `>>` 意味着追加写入

- 试试追加

- - 我们可以新建一个
    - 然后追加一些东西写入`oeasy.txt`
    - 然后我们看看这个`oeasy.txt`
    - 是不是写进去了

## 总结

- 除了 `i`、`I` 在前面插入文本之外
- 我们了解到 `a`、`A` 可以在行末插入文本
- `a` 也可以从正常模式切换到插入模式

![force quit](https://i0.hdslb.com/bfs/article/bf2ca21b60192d430ee0a717747f54606d5ccc90.png@942w_636h_progressive.webp)

- `a` 插在光标之后
- `A` 插在本行最后
- 关于插入，还玩点儿什么吗？🤔
- 我们下次再说！*



# vim - 9 - # 换行插入

## 插入新行

## 回忆上节课内容🤔

- 上上次是 `i`、`I` 在光标前面插入

- 又加了 `a`、`A` 可以在光标后面插入

- - `a` 是在光标后插入
    - `A` 是在当前行最后插入

![force quit](https://i0.hdslb.com/bfs/article/bf2ca21b60192d430ee0a717747f54606d5ccc90.png@942w_636h_progressive.webp)

- 关于插入，还有什么命令吗？🤔
- 我们继续去查阅 help

:h i

## 我们发现有这样一组命令

![force quit](https://i0.hdslb.com/bfs/article/d9e39fbef20c647400a2f295619779b9cb8d1dc7.png@942w_710h_progressive.webp)

## 看起来的意思是

- `o` 在

- - 当前行 **下面** 插入一个空行
    - 然后切换到插入模式

- `O`

- - 在当前行 **上面** 插入一个空行
    - 然后切换到插入模式

- 一个上面 👆，一个 👇

## **上方** 插新行

![force quit](https://i0.hdslb.com/bfs/article/b55bb54086fe87f49ce9e8949ace157cf8d07bef.png@942w_719h_progressive.webp)

- 当前绿色的光标在第6行中间

- - 如果不显示行号，就输入 `:set nu`
    - 当前模式是正常模式

- 如果我按下o

- - 就会在第 7 行插入一个新行
    - 并且模式进入插入模式

- 按ctrl+c

- - 可以回正常模式

- o、ctrl+c

- - 可以反复切换

## **下方** 插新行

- u回到最初

- 回到第 6 行中间位置

- 我按下O

- - 就在第 6 行插入一个空行
    - 原来的第 7 行，变成了第 6 行
    - 并把模式改为输入模式

## 回忆以前学的切换

- i、I和a、A
    都可以进入插入模式

- - i在光标前插入
    - I在本行最前插入
    - a在光标后插入
    - A在本行最后插入

- ctrl+c退回到正常模式

- 现在又加了o、O

- - o本行下方插入一个新行
    - O本行上方插入一个新行

- 再练练重复、撤销、重做

- - 按几次.重复插入操作
    - u可以撤销
    - ctrl+r可以重做

## 保存并退出

- 用 `:wq` 保存并退出

- - `:w` 是保存
    - `:q` 是退出
    - 和在一起就是 `:wq`
    - 保存并退出

- 我们可以使用 `:help :wq` 查看帮助

![wq](https://i0.hdslb.com/bfs/article/f79a9e9bca3af8616baa90a097f53b69cd98dc47.png@942w_711h_progressive.webp)

## 总结

- 我们这次学了两个新的东西 `o` 和 `O`
- `o` 是在当前行下方插入新行
- `O` 是在当前行上方插入新行
- 这样我们就有大小写的 `i`、`a`、`o` 可以从正常模式切换到输入模式了。

![ism](https://i0.hdslb.com/bfs/article/82529a92e206721427b1368440a7f8740fcf9748.png@942w_636h_progressive.webp)

- 我们还把 `:w`、`:q` 合成了 `:wq`
- 现在基本上简单的编辑没有什么问题了
- 下一步就是提高效率，用最快的方式在屏幕上移动
- 怎么做呢？
- 我们下次再说！*



# vim - 10 - # 插入新行

插入新行

## 回忆上节课内容🤔

- i、I在前面插入文本
- a、A在后面插入文本
- o、O换行插入文本
- o其实是A回车
- O其实是ko
- O也是kA回车

![ism](https://i0.hdslb.com/bfs/article/82529a92e206721427b1368440a7f8740fcf9748.png@942w_636h_progressive.webp)

## 模式切换小技巧

- 比如你在一句话的中间，并处于插入模式，此时你想要写下一行

- - 从插入模式到正常模式要用esc
    - 但是esc距离基本起手势太遥远了
    - 可以用ctrl+c来替代
    - 左手小拇指ctrl+c
    - 然后A回车

- 有没有更有效率的方法呢？

![insertnormal](https://i0.hdslb.com/bfs/article/e572bed6a1d00236cacc7db4a4195658b54e5c35.png@942w_956h_progressive.webp)

## 插入-普通模式

- 可以ctrl+o进入插入普通模式
- 然后执行o继续进行插入
- `插入普通模式` 就是让你执行一次 `普通模式` 的命令
- 然后继续保持在 `插入模式`
- `插入普通模式` 相关帮助在 `:h Normal` 的 `intro.txt` 中查到

## 下素材

\#首先找个素材，找个一个网页下载下来wget github.com/overmind1980#然后看看下载了个啥ls#最后用vim打开这个网页vim overmind1980

![web](https://i0.hdslb.com/bfs/article/1c1f85537f3c6f75fa0df6d8c043323b1b3ebf9b.png@942w_705h_progressive.webp)

- 下好了之后打开
- 把手放到键盘上

## 命令分布

我们首先看看正常模式下的命令键盘图

GIF

![help move](https://i0.hdslb.com/bfs/article/0cfcae47854e492ed03c1ff8bc727efb85a690cc.gif@1s.webp)

- 基本上个按键都有对应的命令
- 命令可以分为大写和小写两种
- `iao` 进入插入模式（已经解锁）
- `hjkl` 进行移动（已经解锁）

## 起手势

![help move](https://i0.hdslb.com/bfs/article/29d3e116bd613b65d180e96fcac834ef086f5f36.png@942w_629h_progressive.webp)

- 记不住命令怎么办？

- 淘宝可以搜索 vim 的键盘膜或者贴纸

- 但我感觉没用

- - 字太小
    - 伤屏幕
    - 依赖性

- 还得靠自己熟练之后自然记忆

- - 左手食指放在f
    - 右手食指放在j

- 不管是游泳、弹琴、跑步还是打乒乓球

- - 正确的基本姿势会减少运动伤害
    - 让你的上限更高
    - 肌肉记忆沉淀下来，逐渐变为某些标准

- 这些标准是每个新手都要遵循的

- - 这可不是简单的循规蹈矩
    - 而是体会着前人的智慧和经验

- 这会让你后期更厉害

## 移动命令

![help move](https://i0.hdslb.com/bfs/article/fad77232134a1f95b29f5675c97502cb38d11726.jpg@942w_522h_progressive.webp)

- 起手势是盲打的基本姿势

- 手轻轻放在中间那行上方一点点

- 我们知道由于历史的原因 `hjkl` 对应着移动的命令

- 正常模式下

- - 有必要把右手四指基本位从 `jkl;` 移动到 `hjkl` 吗？

## 保持起手势

- 我认为没有必要改变盲打姿势

- - 右手食指是可以控制两个方向位的
    - 继续保持起手势

- `hjkl` 右手默认位使用概率非常大

- 保持指尖的敏感性

- - 手指会比眼睛更早知道打错字了
    - 还有更多神奇的移动命令等待你来解锁

![hjkl](https://i0.hdslb.com/bfs/article/0824aab6dced6c94bbc106e9c08eb02c2862d140.png@330w_309h_progressive.webp)

## 强制起手式

- 打开当前用户的vim配置文件

vi ~/.vimrc

- 在前面添加上四句

- - `map <Left> <Nop>`
    - `map <Right> <Nop>`
    - `map <Up> <Nop>`
    - `map <Down> <Nop`>

- map是按键映射

- - 我们把上下左右方向键映射为<Nop>
    - 就是什么也不做
    - 保存并关闭vim
    - 然后我们发现上下左右方向键都不好用了

## 总结

- 我们这次强化了起手势
- 回忆了基本的移动方式 `hjkl`
- 除 `hjkl` 外,还有什么移动命令效率更高吗？
- 我们下次再说！*

# vim - 11 - # 向前向后

## 向前向后

## 回忆上节课内容🤔

![hjkl](https://i0.hdslb.com/bfs/article/0824aab6dced6c94bbc106e9c08eb02c2862d140.png@330w_309h_progressive.webp)

- 我们上次强化了起手势🧘
- 回忆了基本的移动方式 `hjkl`
- 除 `hjkl` 外,据说还有更厉害的移动方式
- 是什么呢？

## 下素材

\#这个素材，我们下载过，重温一下wget github.com/overmind1980#然后看看下载了个啥ls#最后用vim打开这个网页vi overmind1980

![web](https://i0.hdslb.com/bfs/article/1c1f85537f3c6f75fa0df6d8c043323b1b3ebf9b.png@942w_705h_progressive.webp)

## 使用帮助学习

- 其他的移动命令应该和 `hjkl` 离得不远

- 可以使用 `:h h`先找到  `h` 的帮助📕

- - 注意是 `:h h` ，而不是 `:h :h`
    - `:h h` 查找的是 正常模式下h命令的帮助手册
    - `:h :h` 查找的是 命令行模式下 `:h` 命令的帮助手册

- 找到这个文件叫做 `motion.txt`

- 对应的位置叫做 `2.Left-right motion`

![hh](https://i0.hdslb.com/bfs/article/ab8d03a2001a3a4d44a742931d500f8a1aeb6b1f.png@942w_654h_progressive.webp)

- 点击上图可放大

## 在帮助中查找单词

- 我希望按照`单词`进行移动

- - 使用 `/word`
    - 查找 `motion.txt` 中关于 `word` 的单词
    - 单词的英文是 `word`
    - 在`vim`打开的 `motion.txt` 帮助手册中

- 找到这个命令叫做 `w`

- 退出帮助 `:q` 试试 `w`

![hh](https://i0.hdslb.com/bfs/article/43a948de1d9121b4352964314bd8e14f3fdd63a0.png@942w_672h_progressive.webp)

## word

![hh](https://i0.hdslb.com/bfs/article/3ac4a76aa0e3145b69090fec9a6292a6e6bab035.png@864w_168h_progressive.webp)

- `w` 可以移动到下一个单词的开头
- `w` 比 `l` 效率要高好多
- 让我们在环境中爽起来➡️➡️➡️
- `w` `w` `w`...
- 但是只有向前，没有回去吗？🤔

## 搜索 backward🔙

- 可以使用 `:h w`先找到 `w` 的帮助
- 还是 `motion.txt`
- 可以使用 `/backward` 查找向前之类的单词
- 找到我们需要的命令 `b`

![backward](https://i0.hdslb.com/bfs/article/1cd1e394efe44b2a2e68b7ce35fe328bbb50cecc.png@942w_686h_progressive.webp)

## backward

![backward](https://i0.hdslb.com/bfs/article/d4cb79033ed28a6ae68d95136d0f9295e86c31b0.png@900w_219h_progressive.webp)

- `b` 就是向前一个单词
- `b` 来到前一个单词的词头
- 有来就有去
- 有阴就有阳
- 我们可以使用 `w` 和 `b` 反复横跳🤸

## 总结

- 我们这次学了向前一个单词
- w
- 意思是 `word`

![backward](https://i0.hdslb.com/bfs/article/3ac4a76aa0e3145b69090fec9a6292a6e6bab035.png@864w_168h_progressive.webp)

- 还学习了向后一个单词
- b
- 意思是 `backward`

![backward](https://i0.hdslb.com/bfs/article/d4cb79033ed28a6ae68d95136d0f9295e86c31b0.png@900w_219h_progressive.webp)

- 这俩命令都落在单词的第一个字母
- 还有什么好玩的命令吗？🤔
- 下次再说 *



# vim - 12 - # 词头词尾

## 词头词尾

## 回忆上节课内容🤔

- 我们这次学了向前一个单词
- w
- 意思是 `word`

![backward](https://i0.hdslb.com/bfs/article/3ac4a76aa0e3145b69090fec9a6292a6e6bab035.png@864w_168h_progressive.webp)

- 还学习了向后一个单词
- b
- 意思是 `backward`

![backward](https://i0.hdslb.com/bfs/article/d4cb79033ed28a6ae68d95136d0f9295e86c31b0.png@900w_219h_progressive.webp)

- 这俩命令都落在单词的第一个字母
- 还有什么好玩的命令吗？🤔

## 动手练习

- 我们可以一路向前
- 也可以反复横跳
- w、b附近还有什么？🤔
- 去 `:h w` 附近再转悠转悠

## 查询帮助

- 我们看到w、b中间有个e

- 说是

- - Forward to the end of word [count] inclusive.
    - Does not stop in an empty line.

- 意思

- - 向前到单词的结尾
    - 空行不停留
    - 直到这个文档的尽头
    - 也不停留~~~

- e对应单词时 `end`

- 我们来试一下🤪

## 跳到词尾

![e2](https://i0.hdslb.com/bfs/article/6e7173734232a9bdfa56b530a2208fd408c7ea26.png@807w_555h_progressive.webp)

- 我们可以看到e是向 `前` 跳到 `本词尾`
- 而w是向 `前` 跳到 `下词头`
- b则是向 `后` 跳回到 `上词头`
- 如果我的光标不在 `本词头` 的位置，又如何呢？

## 光标位于词中

![e3](https://i0.hdslb.com/bfs/article/99c9c9bd7ac2cae37c43431ab5fa7bb0ad0f3ad7.png@603w_555h_progressive.webp)

- 我们可以看到，如果光标位于 `词中` 时

- e不变，还是跳到 `本词尾`

- w还是跳到 `下词头`

- 而b有变化，向 `后` 跳没变，但是跳回到了 `本词头`

- w、b

- - 都是跳到 `词头`
    - 一个向 `前` 一个向 `后`

- e是向 `后` 跳到 `词尾`

- 如果我想向前跳到词尾呢？

## 向前跳到词尾

- ge向前跳到词尾

![图片描述](https://i0.hdslb.com/bfs/article/a21fa304a1ab4f2408357a2c3afc63039e3408da.png@942w_386h_progressive.webp)

![图片描述](https://i0.hdslb.com/bfs/article/28af0ace3778ab8c062db4ffdc1afb1a25cab161.png@942w_261h_progressive.webp)

## 连续跳跃

- `wbe` 比 `hjkl` 效率高得多
- 但是还可以更高 🤸
- 方法就是使用数字
- 从帮助中，我们可以发现可以选择使用 `[count]` 次数

![e](https://i0.hdslb.com/bfs/article/bca88eb1baa5bb5187513aa62f2487f011e74f99.png@942w_563h_progressive.webp)

- 意思就是可以向前 n 个单词

## 跳起来吧🤾‍♀️

![count](https://i0.hdslb.com/bfs/article/0c94a6d355f94007a685a06b261460ea972b0ee1.png@510w_474h_progressive.webp)

- 在方向前面加上数字

- - `3b`、`5e` 这样都可以

- 甚至 `hjkl` 都可以使用

- - 比如 `4h`、`10l`

- 这样快得多！！！✊

## 总结

- 我们这次学习了e
- e代表`end` 词尾
- 我们了解到在词中时，b退到本词头
- 还可以成倍的跳跃
- 但是当前单词和我的理解有点不一样啊？
- 我想直接跳到href属性，怎么办🤔
- 下次再说 *

# vim - 13 - # 大词小词

## 大词小词

## 回忆上节课内容🤔

- 我们上次学习了e
- e代表 `end` 词尾

## 自有跳跃

- 还可以成倍次数的跳跃 🤸

![count](https://i0.hdslb.com/bfs/article/0c94a6d355f94007a685a06b261460ea972b0ee1.png@510w_474h_progressive.webp)

- 但其实我是想以一个一个属性地跳跃，有没有方法呢？

## 查询帮助

- 没思路的话我们还是得继续查询 `:h w`
- 除了w之外
- 还有一个W
- 小 `w` 对应 `word`
- 大 `W` 对应 `WORD`
- 都是什么意思？
- 继续查询呗！！️📕
- `:h word`
- 关于大小词的介绍还是在 `motion` 里面



## 对比分析

![count](https://i0.hdslb.com/bfs/article/8c19f5dbef208ab1a32bc1176241a793c6533bb0.png@731w_264h_progressive.webp)

- 可以看到小w认为 `=`、`"` 都是 `word` 的分割字符
- 大W认为 `=`、`"` 都不是 `WORD` 的分割字符
- 只有空格、tab、换行是 `WORD` 的分割字符。
- 这个W还是很舒服的，直接就可以跳属性了
- 爽🫖

## 相关移动命令

![WEB](https://i0.hdslb.com/bfs/article/2a7cc05be5107e6b4468e9b950dc592d91057af2.png@809w_417h_progressive.webp)

- 不光是w有大词小词

- e、b也有大词这回事儿

- - E向前到下一个 `大` 词尾
    - B向后到上一个 `大` 词头

- 大词的分割字符还是空格、tab、换行

- 仔细观察上图

## 总结

- 我们这次了解了 `大词` 和 `小词`

- - `小词` 就是我们常规意义的词，被 `=`、`"` 等标点分开的词
    - `大词` 里面包括了 `=`、`"` 等标点，只能被空格、tab、换行分割

- W、E、B都可以有大词移动

- 但如果我想一步就跳到行头或行尾

- 这不一步登天么？

- 可能么🤔

- 下次再说 *



# vim - 14 - # 行头行尾

## 行头行尾

## 回忆上节课内容🤔

- 我们这次了解了 `大词` 和 `小词`

- - 只能被空格、tab、换行分割
    - 被 `=`、`"` 等标点分开的词
    - `小词` 就是我们常规意义的词
    - `大词` 里面包括了 `=`、`"` 等标点

- W、E、B都可以有大词移动

![WEB](https://i0.hdslb.com/bfs/article/2a7cc05be5107e6b4468e9b950dc592d91057af2.png@809w_417h_progressive.webp)

- 但如果我想一步就跳到行头或行尾
- 这不一步登天么？
- 可能么🤔

## 查阅文档📕

- 还是从 `:h w`，开始查找起
- 还是在 `motion` 里面查找
- 应该和W都属于左右移动的部分
- 找到这样两个命令

![WEB](https://i0.hdslb.com/bfs/article/09e0eb29c4ebd3cacca9b3c3c031e8010de66fe1.png@942w_375h_progressive.webp)

## 行首和行尾

![WEB](https://i0.hdslb.com/bfs/article/98ca7f29e4b59ac2e8c11a53845203f6341b451e.png@750w_306h_progressive.webp)

- ^，也就是shift+6

- - 作用是移动到行首
    - 或者说移动到本行第一个非空字符

- $，也就是shift+4

- - 作用是移动到本行行尾

- `^`、`$` 也分别对应正则表达式中的 `开头` 和 `结尾`

## 深入细节

- 如果本行开头第一个字符是空格

- - 那^无法到第一个字符啊？
    - 如果我就想去第一个字符
    - 无论他是空格还是tab
    - 应该怎么办呢？

- 这个命令应该离 `^` 不远

- 应该也在 `motion` 的 左右移动部分

- 找到了 `0`

![WEB](https://i0.hdslb.com/bfs/article/a46da20b2757694170792f05e9269054e36cb095.png@704w_306h_progressive.webp)

## 行头区别

- ^是到本行第一个非空字符
- 0是到本行第一个字符，不管是不是空格

![图片描述](https://i0.hdslb.com/bfs/article/ce6a1ae8b871e1978bf7d71c359b27f8cf2cd3d7.png@942w_321h_progressive.webp)

- 那结尾如果有空格会如何呢？

## 结尾细节

- 相关命令肯定也在左右移动这部分
- 找到 `g_`

![toEnd](https://i0.hdslb.com/bfs/article/4534a93c54b06b90fb67749d9a4f6c9c691cd802.png@885w_390h_progressive.webp)

- g_是到本行最后一个非空字符
- 两个按键要依次按下
- $跳到本行最后一个字符，即使他是空格

## 总结

- 我们这次学会了直接跳到开头和结尾

- 最重要的就是 `^`、`$`

- - ^到开头
    - $到结尾

- 还有什么好玩的吗？🤔

- 下次再说 *



# vim - 15 - # 行内查找

## 行内查找

## 回忆上节课内容🤔

- 上次学了直接跳到开头和结尾

- 最重要的就是 `^`、`$`

- - ^到开头
    - $到结尾

- I

- - 相当于^i

- A

- - 相当于$a

![WEB](https://i0.hdslb.com/bfs/article/98ca7f29e4b59ac2e8c11a53845203f6341b451e.png@750w_306h_progressive.webp)

## 查找帮助

- 还有什么呢?

- 还是继续在 `motion` 里面

- - ^、$之后找

- 还是在左右移动这里面发现有个f

- 看起来是查找某个字符的样子

![WEB](https://i0.hdslb.com/bfs/article/ad7548128a4dde3936d576c1f5ec68d28d8beffc.png@942w_401h_progressive.webp)

## 查找字符

![图片描述](https://i0.hdslb.com/bfs/article/e8466ee00ad635eee14c47558b9fcad045a80e35.png@942w_152h_progressive.webp)

- 看起来就像

- - f谁就跳到谁那里

- 我们来试一下

- 先下载个素材

\#下载素材git clone http://github.com/overmind1980/vimtutorial.git# 进入目录cd vimtutorial#需要注意这次用无配置文件的方式启动vivi -u NONE oeasy.java

## 行内查找

![findo](https://i0.hdslb.com/bfs/article/2987c0380cbde683cc101b7b487a67500905a0bc.png@942w_338h_progressive.webp)

- 通过fo

- 直接跳到了到了右边邻近的的 `o` 字符

- f的意思是

- - `find` 查找
    - 并让光标跳跃过去

- o的意思是

- - 字符 `o`
    - 查的不是别的
    - 是字符 `o`

- 前面还有 `o`

- - 想要找下一个咋办？

- 还能咋办？

- - 查帮助呗！
    - 一定在 `f` 附近

## 继续查找

![findhelp](https://i0.hdslb.com/bfs/article/00ed8b65dce06d39fd2e3d751c2cba7b624e9b77.png@942w_189h_progressive.webp)

- 帮助说;
- 可以让查找继续
- 我们来试试

## 动手练习

![findnext](https://i0.hdslb.com/bfs/article/83a73839089652bd50858c54a0060efdf132b821.png@942w_338h_progressive.webp)

- 好像真的可以
- 小拇指直接落下去就可以
- 查找范围到本行末尾，不能跨行
- 帮助里，还有个和;配对的,是干什么用的？
- 试试

## 反向继续查找

![findnext](https://i0.hdslb.com/bfs/article/d556f075fcea0fa70eb5213246fed290269bd433.png@942w_338h_progressive.webp)

- 中指向下找到,
- 确实可以让他反向
- 搜索范围还是被限制在了本行
- 帮助里面还提到的F是干什么用的？

## 反向跳跃

![图片描述](https://i0.hdslb.com/bfs/article/5f70038546897389de4cf4f08429e75c0d496dd9.png@942w_300h_progressive.webp)

- F和f一样
- 都是行内跳跃
- 但是F是反向跳跃

## 反向跳跃练习

![findnext](https://i0.hdslb.com/bfs/article/96ce803cda78c025594ad49bb787e03585875765.png@942w_338h_progressive.webp)

- 这个时候如果;

- - 就是继续反向查找
    - 保持跳跃的方向不变
    - 只要是方向不变就是;
    - 保持小拇指的感觉

- 方向改变的话

- - 就是,
    - 体验中指的感觉

- 帮助里面还提到了 `[count]`

- - 这个怎么用

## 跳跃查找

- 回忆 `[count]`

- - 这东西是翻子
    - 可以翻倍
    - `3w` 就是跳跃3个小词
    - `4j` 就是向下4行

- f2o肯定不行

- - 因为f2查找到 `2` 字符
    - o下方插入一个空行，并切换到插入模式

- 2fo

- - 找到第 `2` 个 `o`

- ;

- - 保持查找方向不变
    - 继续向前

- ,

- - 反向查找`o`

- 2;

- - 保持查找方向不变
    - 向前移动到第 `2` 个 `o`

- 2,

- - 反向查找
    - 第 `2` 个 `o`

![2fo](https://i0.hdslb.com/bfs/article/0b46f4a941dc032e1aaa14c8389a67d7ce2c04c5.png@942w_338h_progressive.webp)

## 总结

- 跳跃

- - 向前跳跃是f
    - 向后跳跃是F

- 继续

- - 保持方向是;
    - 改变方向是,

- 可以加上 `[count]` 来加速

- 还有什么好玩的吗？🤔

- 下次再说 *

# vim - 16 - # 行内贴靠

## 行内贴靠

## 回忆上节课内容🤔

![findo](https://i0.hdslb.com/bfs/article/2987c0380cbde683cc101b7b487a67500905a0bc.png@942w_338h_progressive.webp)

- 跳跃

- - 向前跳跃是f
    - 向后跳跃是F

- 继续

- - 保持方向是;
    - 改变方向是,

- 可以加上 `[count]` 来加速

- 还有什么好玩的吗？🤔

## 动手

\#这次还是用无配置的方式启动vi -u NONE oeasy.java

- `:h f` 继续查找周围的命令

- f旁边还有

- - t
    - T

- 这两个是干什么用的？

- 我们来看一看👀

## 查看帮助

![helpt](https://i0.hdslb.com/bfs/article/73baf2787d099e781eca3a408addf16e8c42adcf.png@942w_587h_progressive.webp)

- 含义不同

- - f对应的单词是 `find` 找到
    - t对应的单词是 `till` 贴靠

- 位置不同

- - f光标直接跳到查找的字符上
    - t光标跳到查找字符的前一个字符上，贴靠着查找字符

## 试一试

![helpt](https://i0.hdslb.com/bfs/article/c3d451171ab24e3e4a26dcf292ef4b9ce74b9e79.png@344w_428h_progressive.webp)

- fe是把光标移动到 `e` 上面
- te是把光标移动到 `e` 之前的字符上面
- ;还可以继续吗？
- 好像不行，怎么办？

## 继续移动

- 直接下一个是不行的

- 因为已经到达了 `e` 前一个的位置

- 那我们可以

- - `till` 下一个 `e`
    - `till` 下一个 `e`
    - 先l把光标移动到 `e` 上面
    - 然后小拇指直接落在;
    - 再l把光标移动到 `e` 上面
    - 再小拇指落;

- 在;的过程中

- - 重复的操作仍然是 `till`
    - `till` 的对象仍然是 `e`

![tillgoon](https://i0.hdslb.com/bfs/article/8f850f6b97aac451e6f685c94feebefab2462152.png@942w_462h_progressive.webp)

- 我们是否可以反方向,呢？

## 继续反向 till

![tillgoon](https://i0.hdslb.com/bfs/article/f6cb0d7684cf6d04d8789f7b40407081709fc38b.png@942w_476h_progressive.webp)

- ,改变查找方向

- - 模式仍然是 `till` 模式
    - 字符仍然是 `e`
    - 找到左边最近的 `e` 的前一个字符的位置
    - 还想继续不可能

- 还是因为已经到达了 `e` 的前一个字符的位置

- - 于是要向左到 `e`
    - 这样就可以继续向左查找了

## 直接反向

![tillgoon](https://i0.hdslb.com/bfs/article/fbaad38d8b1c1413d8c16f9e53f00341efe01184.png@942w_311h_progressive.webp)

- T向左进行贴靠
- ;保持方向
- ,改变方向
- 反向的反向就是正向

![图片描述](https://i0.hdslb.com/bfs/article/49aaa3fbff367f66e46c13cdc399a07cf5c3f3f9.png@942w_140h_progressive.webp)

## 翻倍

- 2to`till` 第2个 `o`
- ;保持查找方向不变，继续向前 `till` 下一个 `o`
- ,反向 `till` 上一个 `o`
- 2;保持查找方向不变，向前 `till` 到第 2 个 `o`
- 2,改变方向，`till` 第 2 个 `o`

![tillgoon](https://i0.hdslb.com/bfs/article/5a423566ae56368b92579ca226b648dc7f1cbf9d.png@942w_368h_progressive.webp)

## 总结

- 贴靠

- - 向前贴靠是t
    - 向后贴靠是T

- 继续

- - 保持方向是;
    - 改变方向是,

- 可以加上 `[count]` 来加速

- 行内左右移动好像，到这里接结束了？后面还有什么呢？

- 下次再说 *

# vim - 17 - # 向上向下

## 向上向下

## 回忆上节课内容🤔

- 和 `f` 相关的是跳到

- - 向 `前` 跳到是f
    - 向 `后` 跳到是F

- 和 `t` 相关的是贴靠

- - 向 `前` 贴靠是t
    - 向 `后` 贴靠是T

- 和 `小写` 相关的是 `向前`

- - `向前` 跳跃是f
    - `向前` 贴靠是t

- 和 `大写` 相关的是 `向后`

- - `向后` 跳跃是F
    - `向后` 贴靠是T

- 和继续 `查找方向` 相关的是;、,

- - `保持方向` 是;
    - `改变方向` 是,

## 向上向下

- 本次启动的时候还是无参数模式

- `:set nocompatible` 设置为不兼容 `vi`

- - 意思是使用 `vim`的方式处理命令

- `motion` 的 `左右移动` 之后是 `上下移动`

- - j是向下 👇
    - k是向上 👆
    - 5j就是让光标向下👇 5 行
    - 5k就是让光标向上👆 5 行
    - 可以使用回车换行
    - 也可以使用方向键向上或向下
    - 更常见的还是j、k，因为他们基于基本位置
    - 继续向下翻

![updown](https://i0.hdslb.com/bfs/article/f81a29c7f4dc2a3176d83b9daac70fef5aeec4e5.png@942w_513h_progressive.webp)

## 上下行首

![updown](https://i0.hdslb.com/bfs/article/d2bae3de1d3cb89d11481c11543b24c6dad4df57.png@942w_276h_progressive.webp)

- 加号 `plus` 对应+

- - 对应键盘shift+=

- 减号 `minus` 对应-

- 上下行跳到行首

- - +向 `下` 并且到行 `首` 非空字符
    - -向 `上` 并且到行 `首` 非空字符

- 对应关系

- - +相当于j^
    - -相当于k^

## 首行尾行

![updown](https://i0.hdslb.com/bfs/article/30f7a404db5e1f53a7ff72200e4b470b8bd3198c.png@942w_492h_progressive.webp)

- gg对应 `首行`

- G对应 `尾行`

- 如果文章很长的话，直接跳就很方便

- 一个G直接就到了 `Ground`

- 想回开头的话可以用gg

- - 不知道为什么这两个字母格外熟练
    - 熟练的让人心痛！

- 另外还有一个组合 `Go`

- 比如追加一个很长的配置文件的话Go

- - `G` 直接到最后
    - `o` 在下面一行插入

- 两个按键 `Go` 起来

- ctrl+c回到正常模式

- `gg` 就回开头

- - 重来一局

## 自动缩进

- 当然也不都是痛苦回忆

- gg配G是我见过最方便的自动缩进方式

- - gg=G从首行到尾行自动缩进
    - 这个文件可能有 500 行,
    - 但是一把就全都缩进好了

- 不只是程序、网页、css、配置文件都可以自动缩紧

- - 这样整理代码就非常迅速了

- 程序员更多的时候工作在 normal 模式

- - 被当作默认模式的原因。
    - 浏览、搜索、跳跃、复制、粘贴
    - 真正聚焦下来写代码再切换到插入状态。
    - 其他编辑器永远只有一个插入状态
    - 其实是浪费了很多键盘功能的
    - 这也是 Normal 模式被称作 Normal 正常模式

- gg=G这非常爽！！！🤪

![updown](https://i0.hdslb.com/bfs/article/5d4ba38a6cb5bcfb5119ecf599aee0d0f90a9080.png@942w_968h_progressive.webp)

## 总结

- 上下行

- - 向 `下` 是j👇
    - 向 `上` 是k👆

- 上下行首

- - 向 `下` 到行首非空字符+
    - 向 `上` 到行首非空字符-
    - 这些 `motion` 都可以加上 `[count]` 来翻倍

- 首尾行

- - 首行是gg
    - 尾行是G
    - gg=G是全部自动缩进
    - G好像还有其他用法?

- 什么用法呢?

- 下次再说 *

# vim - 18 跳到某行

## 跳到某行

## 回忆上节课内容🤔

- 上下行

- - 向 `下` 是j👇
    - 向 `上` 是k👆

- 上下行首

- - 向 `下` 到行首非空字符+
    - 向 `上` 到行首非空字符-
    - 这些 `motion` 都可以加上 `[count]` 来翻倍

- 首尾行

- - 首行是gg
    - 尾行是G
    - gg=G是全部自动缩进
    - G好像还有其他用法?

- 什么用法呢?

- 先用 `无配置` 的 `vi` 打开 `oeasy.java`

## 直接跳转到某行

![updown](https://i0.hdslb.com/bfs/article/30f7a404db5e1f53a7ff72200e4b470b8bd3198c.png@942w_492h_progressive.webp)

- 直接跳到某行Goto Line

- - 2G跳到第`2`行
    - 3G跳到第`3`行
    - 4G跳到第`4`行
    - gg跳到第`1`行
    - G跳到最后一行

- 这个真的很方便

- - 尤其编译报错某行出问题的时候
    - 直接就 `Goto` 过去了

- 如果行数多了

- - 怎么才能使到我要去第几行呢？
    - 这就需要显示行号

## 显示行号

- `:set number` 是显示行号

- - `:set` 是命令，可以设置各种属性
    - `number` 是 `:set` 的参数option
    - 是一个负责显示行号的开关属性

- 我们可以通过 `:h :set` 来查看各种属性

- - 这些帮助手册都在 `options.txt` 中

![updown](https://i0.hdslb.com/bfs/article/05ca8ae2ef8b5b645d61ddffa5511c7e0ff575e3.png@942w_87h_progressive.webp)

- 我们不但可以打开 `number` 开关

- - `:set number` 打开 `number`开关
    - 显示行号

- 也可以关闭`number`开关

- - `number` 前面加上 `no` 代表关闭该开关
    - `:set nonumber` 关闭 `number`，不显示行号

- 简写

- - `:se[t] nu[mber]` 可简写为 `:se nu`
    - `:se[t] nonu[mber]` 可简写为 `se nonu`

## 显示相对行号

- 我们不但可以显示绝对的行号

- 也可以显示相对的行号

- 也在 `options.txt` 这文件里

- 这个开关叫做 `relativenumber`

- - 相对行号
    - `:set relativenumber`

![updown](https://i0.hdslb.com/bfs/article/080d886253a508eddf894bfd79ec2c27d54197ad.png@942w_711h_progressive.webp)

- 可以看到当前光标位置对应 `0` 行

- - 向上👆的行号是从当前行行计算的
    - 向下👇的行号也是从当前行计算的
    - 这样上下运动就会更精确一点
    - `4j` 就能知道光标落在下面标 `4` 的那行
    - `5k` 就能知道光标落在上面标 `5` 的那行

- 如果我同时设置 `se nu` 会如何呢？

- - 当前行显示绝对行号，上下部分显示相对行号

- 相对行号简写

- - `set relativenumber` 简写为 `se rnu`
    - `set norelativenumber` 简写为 `se nornu`

## 行命令模式跳转

![updown](https://i0.hdslb.com/bfs/article/080d886253a508eddf894bfd79ec2c27d54197ad.png@942w_711h_progressive.webp)

- 我们还可以使用行命令的模式跳转

- - `:30` 跳到第 `30` 行
    - `:40` 跳到第 `40` 行
    - `:40` 跳到第 `50` 行
    - `:6000000` 跳到结尾，如果整篇文字没有 `6000000` 行的话

- 如何知道当前文件有多少行呢？

- - 还记得 `:f[ile]` 吗？
    - 快捷键是ctrlg

## 显示位置

![updown](https://i0.hdslb.com/bfs/article/37e69eee5b8df74cc0501e5844f4b7e84a00d3e3.png@942w_714h_progressive.webp)

- 我们可以通过ctrlg看到：

- - 文件名
    - 当前行号
    - 总行数
    - 当前位置百分比
    - 当前列位置

## 总结

- 跳转到行号

- - `200G`

- 设置行号选项

- - 显示行号 `:se nu`
    - 显示相对行号 `:se rnu`

- 如何用命令行跳转 `:100`

- 但是我如何有的时候记不住到底跳到多少行

- 能否做个标记留个记号呢？

- 下次再说 *

# vim - 19 - 使用标记

## 使用标记

## 回忆上节课内容🤔

- 跳转到行号

- - `200G`

- 设置行号选项

- - 显示行号 `:se nu`
    - 显示相对行号 `:se rnu`

- 如何用命令行跳转 `:100`

- 但是我如何有的时候记不住到底跳到多少行

- 能否做个标记留个记号呢？

## 跳回原地

- 如果我使用G跳转到最终行

- 然后我想要回到跳转之前的位置

- - 不只是G对应的跳转包
    - 还括行跳转、搜索等

- 那这个跳前位置在哪里呢？

- - 我们可以使用 **``** 回到跳转之前的位置
    - ` 位置在键盘 **1** 前面
    - 这个字符就是我们的反引号
    - 叫做 `open single quote chararcter`
    - 可以试着玩玩

- 跳过来再跳过去

- 反复横跳

- 但是这个只能在两个位置之间来回来去的跳

![图片描述](https://i0.hdslb.com/bfs/article/00c4b87163941cff039834e70e1de4dade75e5a2.png@942w_149h_progressive.webp)

- 我想要跳到更久之前的位置
- 怎么办呢？

## 跳转列表

- 所有曾经的跳转都在跳转列表里面

- 比如我们从

- - 第一行跳到 `33` 行
    - 然后再跳到以 ^The 开头的行

![图片描述](https://i0.hdslb.com/bfs/article/2432f5716dda84a9f2c9ff1abd6a8990ba138f47.png@942w_354h_progressive.webp)

- CTRL-O 跳转到

- - Older position
    - 上一次
    - 上一次的上一次

- CTRL-I 跳转到

- - 下一次
    - 下一次的下一次

![图片描述](https://i0.hdslb.com/bfs/article/a0794ad62d0b14d3a242261c8c68479a8dc83756.png@942w_267h_progressive.webp)

- 这里跳转的位置我们使用了 `标记 mark`

## 查询帮助

![图片描述](https://i0.hdslb.com/bfs/article/5f6defe4b4587b03d726c65843523a722c482182.png@942w_750h_progressive.webp)

- 使用 `h(elp) m(arks)` 查询关于标记的帮助

- - 可以使用 `ma` 来做一个标记 `a`
    - 然后可以用 `'a` 或者 `a 进行跳转

## 进行定义并进行试验

- `:se nu` 设置显示行号

- 使用 `ma` 把当前光标的位置做一个标记 `a`

- 然后G跳转到最终行

- 这个标记你在文档里面看不见

- `:marks` 来查看所有标记

- - 注意这个 mark 都是包含行和列的具体位置的
    - a 对应795行 6列

![图片描述](https://i0.hdslb.com/bfs/article/b608a1b6d0aa993beb829097b5393e2b00bf6c60.png@942w_750h_progressive.webp)

## 其他标记

- `ma` 是我们自己定义的 `a` 标记
- 其他的标记是什么意思呢？
- 我们可以用 `:h ''` 来看 `''` 的含义

![图片描述](https://i0.hdslb.com/bfs/article/189fad690c4cf97da7f64ce7f8de50e9de8f4d3c.png@942w_563h_progressive.webp)

## 更多标记

- `''` 是上次跳转操作光标所在的位置
- `'"` 是上次退出当前文件的位置
- `'[` 是上次编辑（删除修改等）的开始位置
- `']` 是上次编辑（删除修改等）的结束位置
- `'.` 是上次编辑（删除修改等）的最后的操作位置

![图片描述](https://i0.hdslb.com/bfs/article/a625d379f595cb1a46335e5e5e8290c9556dd0bb.png@786w_516h_progressive.webp)

- 那么，这个大写、小写、数字的标记有什么不同呢？

## 标记细节

![图片描述](https://i0.hdslb.com/bfs/article/6f223be13dda61442019927a9d2648454ffe3330.png@942w_507h_progressive.webp)

- 小写 `a-z` 可以标记本文件内部的位置坐标
- 大写 `A-Z` 可以跨文件标记位置坐标
- 数字 `0-9` 在配置文件 `.viminfo` 中，可以保留标记
- 我们还可以用 `:delm(arks) a` 来删除 `a` 标记

## 总结

- 定义标记 a `ma`

- 删除标记 a `:delm a`

- 跳转到标记 a `'a`

- - `a 跳到 a 对应的行和列
    - 'a 跳到 a 对应的行

- 查看所有标记 `:marks`

- 各种标记类型

- - `''` 是上次跳转操作光标所在的位置
    - `'"` 是上次退出当前文件的位置
    - `'[` 是上次编辑（删除修改等）的开始位置
    - `']` 是上次编辑（删除修改等）的结束位置
    - 小写 `a-z` 可以标记本文件内部的位置坐标
    - 大写 `A-Z` 可以跨文件标记位置坐标
    - 数字 `0-9` 在配置文件 `~/.viminfo` 中，可以保留标记

- 每次都需要ctrl+g显示坐标

- 能否一直显示坐标呢？

- 下次再说 *

# vim - 20 - 显示标尺

## 显示标尺

## 回忆上节课内容🤔

- 定义标记 a `ma`

- 删除标记 a `:delm a`

- 跳转到标记 a `'a`

- - `a 跳到 a 对应的行和列
    - 'a 跳到 a 对应的行

- 查看所有标记 `:marks`

- 各种标记类型

- - `''` 是上次跳转操作光标所在的位置
    - `'"` 是上次退出当前文件的位置
    - `'[` 是上次编辑（删除修改等）的开始位置
    - `']` 是上次编辑（删除修改等）的结束位置
    - 小写 `a-z` 可以标记本文件内部的位置坐标
    - 大写 `A-Z` 可以跨文件标记位置坐标
    - 数字 `0-9` 在配置文件 `~/.viminfo` 中，可以保留标记

- 每次都需要ctrl+g显示坐标

- 能否一直显示坐标呢？

## 显示当前位置

\#首先用无模式让vi编辑一下/etc/passwdvi -u NONE /etc/passwd

- ctrl+g

- 或者 `:f[ile]`

- 可以在最下面一行

- - 看到当前编辑的文件
    - 以及文件的位置

![图片描述](https://i0.hdslb.com/bfs/article/c18893dfa3c69e2f3edc51ed86cc00cd7f6c841d.png@942w_737h_progressive.webp)

## 显示标尺

- 想一直显示光标位置的话

- - 就需要一个标尺
    - `标尺` 是一个`开关option`

- 什么是开关呢？

- - 就是可以设置开或者关的地方

- `标尺` 开关的名称是 `ruler` 尺子📏

- - 可以打开标尺
    - 也可以关闭标尺

- 这个开关如何开合呢？

## 进行设置

- `ruler` 标签可以用 `:set` 这样的方式进行设置

- - `:se[t] ru[ler]` 就可以设置标尺可见
    - `:se[t] noru[ler]` 就可以设置标尺不可见

- `number` 标签也可以用 `:set` 这样的方式进行设置

- - `:se[t] nu[mber]` 就可以设置行号
    - `:se[t] nonu[mber]` 就可以设置行号不可见

- 也可以两个一起开启

- - `:se nu ru`

- 或者两个一起关闭

- - `:se noru nonu`

- 都是一些蓝布棉门帘

![图片描述](https://i0.hdslb.com/bfs/article/6b29bcf8264f35b12a2fd458c4e79bd8fe1321a3.png@942w_827h_progressive.webp)

## 关于开关

- 开关就是 `options`

- - 可以设置当前文档是否显示标尺
    - 也可以设置当前文档是否自动换行
    - 开关和我们编辑的文档没有直接关系
    - 但是决定着目前显示的状态

- 可以使用 `:options`

- - 打开 `options.txt` 查看 `所有` 的开关
    - `/ruler` 在当前文件中查找 `ruler` 这个开关

![图片描述](https://i0.hdslb.com/bfs/article/58da66922f0b728bbbef6808ec6e783eb552c3f2.png@942w_573h_progressive.webp)

- 那我怎么知道 `ruler 开关`当前状态?

## 查看开关

- 查看开关状态？

- 可以通过？来查看开关状态

- - `:set number?`
    - `:set ruler?`

- 可以试试

![图片描述](https://i0.hdslb.com/bfs/article/a92e8b3cd9106090ef816be6a183ae1824003c03.png@942w_60h_progressive.webp)

- 如果我想把开关复位到初始状态
- 应该怎么做？

## 复位开关&

- 复位开关状态&

- 直接把开关复位为默认值

- - `:set number&`
    - `:set ruler&`

![图片描述](https://i0.hdslb.com/bfs/article/11dfa77a9eb70c17ba038fa8e518a18ae75e498e.png@942w_80h_progressive.webp)

## 标尺细节

- `:options` 可以得到一行的简单解释
- 如果想要更详细的信息
- 也可以通过 `:h 'ruler'` 找到这个选项开关的细节

![img](https://i0.hdslb.com/bfs/article/f197df2eb9df123f3865399ba392dbfcfac92dfe.png@942w_711h_progressive.webp)

## 标尺细节

![img](https://i0.hdslb.com/bfs/article/8bcced87845e4fdb411f51d2dc7e4eb3ba06cfed.png@900w_236h_progressive.webp)

- 在右下角可以看到标尺 📐
- 标尺把光标位置，在 `80*24` 屏幕 📟 中明确标注
- 用逗号,分割开 `行号` 和 `列号`
- `行号` 的显示开关是 `:se nu`
- `列号` 就是当前光标所在列的序号

## 跳转

- 跳转到行

- - 29G命令跳转到第29行
    - `:33` 快速跳转第33行

- 跳转到列

- - 19|
    - 用命令跳转到第19列

![img](https://i0.hdslb.com/bfs/article/7dd205cf3b413215bf8838c09659663eb60f6cf0.png@942w_713h_progressive.webp)

## 标尺细节

- 在标尺的右边写着一些文字

- - 有时在 `顶端`，文件第 1 行在屏幕顶端
    - 有时在 `底端`，文件最后 1 行在屏幕底端
    - 有时在 `全部`，文件很短一屏幕就全显示

![img](https://i0.hdslb.com/bfs/article/6e1f59e74c1aad3bd2971807bbbc03b8df532d88.png@942w_230h_progressive.webp)

## 显示命令

- 用 `:set showcmd` 可以在标尺左边看见所用的命令

- - `show` 显示
    - `cmd` 命令

- 19G命令跳转行号

- 一个字符一个字符地按下

- 观察变化

- 这样我们就可以看到命令输入的情况

![图片描述](https://i0.hdslb.com/bfs/article/64dced2dccca9026c19dad5476d6f3cbe4279f0b.png@942w_441h_progressive.webp)

## 用百分比方式跳转

- 在行列号后面有个百分比
- 有时是百分比，比例为光标行号除以文件总行号
- 可以使用29%跳到整个文件 `29%` 的位置

![图片描述](https://i0.hdslb.com/bfs/article/354a232c6906985014044fab97c6dd501198f25f.png@942w_173h_progressive.webp)

## 设置历史记录数量

- `:set history=100`
- 这样可以通过键盘上下找到曾经执行的命令
- `:h 'history'`

![图片描述](https://i0.hdslb.com/bfs/article/c7925ee0167008dff63281dee9d26fd9a43b4b0b.png@942w_269h_progressive.webp)

## 总结

- 我们这次研究了标尺

- 标尺

- - 开启 `se ru`
    - 关闭 `se noru`

- 行号

- - 开启 `se nu`
    - 关闭 `se nonu`

- 命令位置

- - 开启 `se showcmd`
    - 关闭 `se noshowcmd`

- 跳转

- - 用29G跳转行号
    - 用19|跳转列号
    - 用29%跳到整个文件 29% 的位置

- 还有什么好玩的么？🤔

- 下次再说 *

# vim - 21 - 状态横条

## 状态横条

## 回忆上节课内容🤔

- 我们上次研究了标尺

- 标尺

- - 开启 `se ru`
    - 关闭 `se noru`

- 行号

- - 开启 `se nu`
    - 关闭 `se nonu`

- 命令位置

- - 开启 `se showcmd`
    - 关闭 `se noshowcmd`

- 跳转

- - 用29G跳转行号
    - 用19|跳转列号
    - 用29%跳到整个文件 29% 的位置

## 准备环境

\# 下载素材git clone http://github.com/overmind1980/vimtutorial.git#进入目录cd vimtutorial#还是从最简单的vim开始设置起vi -u NONE oeasy.java

## 设置光标行

- 来看一个开关option

- 光标行 `cursorline`

- - 光标 `cursor`
    - 行 `line`

- `:set cursorline`

![图片描述](https://i0.hdslb.com/bfs/article/3fddaf55e1c93ce2c4738a4eab74161443c48b20.png@942w_188h_progressive.webp)

- `h 'cursorline'`

- - 给 `cursorline` 加了单引号
    - 说明 `cursorline` 是一个属性 `option`

![图片描述](https://i0.hdslb.com/bfs/article/982f8dbe99e5a5788d39585bd9c80ad74f811600.png@942w_212h_progressive.webp)

## 设置光标列

- 有行就有列

- 光标行 `cursorcolumn`

- - 光标 `cursor`
    - 行 `column`

- `:set cursorcolumn`

![图片描述](https://i0.hdslb.com/bfs/article/d11a11dcd1eeb24faa5129334d8ae91d2741f1f9.png@942w_411h_progressive.webp)

- `h 'cursorcolumn'`

- - 给 `cursorcolumn` 加了单引号
    - 说明 `cursorcolumn` 是一个属性 `option`

![图片描述](https://i0.hdslb.com/bfs/article/e9fb0cdfad910657ac6187880f8953a87f86dc02.png@942w_309h_progressive.webp)

## 改变底下的状态横条

- 有了行列位置

- 再配合标尺ruler

- 光标位置就很明确了

- 在 `:h ruler` 的时候

- 偶然发现了一个新天地 `statusline`

- - `statusline` 意思是状态横条
    - 在倒数第 2 行
    - `statusline` 也是一个可以 `set` 的东西
    - 我们来查看一下手册
    - `:h statusline`
    - 好像可以直接给 `statusline` 赋值
    - 我直接赋一个 `oeasy`

- `:set statusline=oeasy`

- 然后还需要设置 `laststatus`

- - 设置 laststatus = 0，不显式状态行
    - 设置 laststatus = 1，仅当窗口多于一个时，显示状态行
    - 设置 laststatus = 2，总是显式状态行

- `:set laststatus=2`

## statusline上可以放什么呢？

- `:h 'statusline'`

![img](https://i0.hdslb.com/bfs/article/ad8f13622788e98dd973b5bb83bbf69327c48f44.png@942w_704h_progressive.webp)

## 显示属性

- 除了字符串常量之外是否能显示一些别的属性呢？

- - 继续翻帮助手册
    - 找到相关的 `items`
    - 各种 `items` 有不同的属性（数字、文本、标志）
    - 每个 `item` 对应一个字母
    - 这个字母需要通过 `%` 来进行转义
    - `F` 对应文件名

- `:set statusline=[oeasy]%F`

- - 此时，状态条就显示 `[oeasy]当前文件名`

![img](https://i0.hdslb.com/bfs/article/51b206814142ab28a9c9dbf4218824b42398a006.png@942w_708h_progressive.webp)

## 标志属性

- 继续翻看属性

- - `Flag` 是标志位
    - `m` 是一个关于是否已经修改的标志位
    - 把 `%m` 追加进入 `statusline`

- `:set statusline=[oeasy]%F%m`

- 修改文件后会显示未保存的 `[+]`

- - 观察效果

- 保存后 `[+]` 会消失

- - 暗中观察...

![img](https://i0.hdslb.com/bfs/article/fe96d91c18a315a714f9a1ee5996b671463b722d.png@942w_708h_progressive.webp)

## 数值属性

- 查到状态栏细节

- - `N` 代表 `Number` 代表 `item` 是一个数值类型
    - 行号 `l`、列号 `c`、百分比 `p` 都是数值类型
    - 用 `[`、`]` 把数值型变量分开
    - `%%` 可以把 `%` 转义显示出来

- `:set statusline=[oeasy]%F%m[%l,%c]%p%%`

![img](https://i0.hdslb.com/bfs/article/c2c67a8efeff559e367c95ce914a34dcd378e04e.png@942w_710h_progressive.webp)

- 状态栏数值还可以随着光标变化😆

## 控制宽度

![img](https://i0.hdslb.com/bfs/article/86469b07ec7d7317320d540a0b355e57e616632f.png@942w_486h_progressive.webp)

- 可以用格式来控制宽度
- `%-0{MinWidth}.{MaxWidth}{item}`
- `%-040.40F`就是用 `40` 的固定宽度显示`F`
- 如果超过范围的话就会把前面部分隐藏
- `:set statusline=[oeasy]%-040.40F%m[%l,%c]%p%%`
- 一行总共 `80` 字符
- 后面的部分怎么办？

## 成组

![img](https://i0.hdslb.com/bfs/article/011fa487a3a2d7e8b05e7246e8f5d7381c286bb4.png@942w_450h_progressive.webp)

- 我们可以把行和列组成一个 `items group`

- 用 `(`、`)` 来封装这个组

- - 标尺组的宽度固定为10
    - 用 `%` 对 `(`、`)` 进行转义
    - `:set statusline=%([%l,%c]%)`
    - 这样就可以统一设置这个标尺组的宽度
    - `:set statusline=%-010.10([%l,%c]%)`

- 同理文件名和文件是否修改也可以编成一组

- - `:set statusline=%(%F%m%)`

## 最终整合

![img](https://i0.hdslb.com/bfs/article/ad2c70c19d676ab6bdb077383b6787ec7beae15e.png@942w_713h_progressive.webp)

- 最终整合总共分为三部分

- - 文件 `%-040.40(%F%m%)`
    - 标尺 `%-030.30([%l,%c]%)`
    - 比例 `%p%%`

- 关于状态横条还有一个总开关

- - `:set laststatus=0` 关闭
    - `:set laststatus=2` 开启

## 总结

- 我们这次了解到了状态横条

- - 通过转义表示 `item`
    - 控制 `item` 宽度的方法
    - 将 `item` 成组的方法
    - 还有一个总开关 `laststatus`

- 但是每次都要写很长的一段话来配置很麻烦啊

- 我们能否写一个配置文件，让 `vim` 每次自动配置好呢？🤔

- 下次再说 *



# vim - 22 - 配置文件

## 配置文件

## 回忆上节课内容🤔

- 我们上次了解到了状态横条

- - 通过转义表示 `item`
    - 控制 `item` 宽度的方法
    - 将 `item` 成组的方法
    - 还有一个总开关 `laststatus`

- 但是每次都要写很长的一段话来配置很麻烦啊

- 我们能否写一个配置文件，让 `vim` 每次自动配置好呢？🤔

![img](https://i0.hdslb.com/bfs/article/ad2c70c19d676ab6bdb077383b6787ec7beae15e.png@942w_713h_progressive.webp)

## 配置文件

\#首先打开原来的配置文件，~代表用户文件夹vi ~/.vimrc#可以用/statusline找到状态条的写法

![img](https://i0.hdslb.com/bfs/article/e186af3ca99916bc8702bfb4357976e274cb15c4.png@942w_717h_progressive.webp)

## ~/.vimrc

- 可以发现 `~/.vimrc` 就是 `vi` 的 `配置文件`
- 如果这个配置文件找不到了 `vi` 会变成什么样子呢？
- 试试！👊

\#原配置文件改名mv ~/.vimrc ~/.vimrc_old#重新书写配置文件vi ~/.vimrc

## 书写配置文件

- 配置文件清空后

- - 配置信息全丢
    - 没关系，从头写

- 首先设置一个状态栏在 `~/.vimrc` 里面写两句话

- - `set statusline=oeasy`
    - `set laststatus=2`
    - 注意这里就不用 `:` 了

- 保留并退出

- 重新编辑 `vi ~/.vimrc`

- 发现状态栏已经生效🤪

- 更新状态栏

- - `set statusline=%-040.40(%F%m%)%-030.30([%l,%c]%)%p%%`
    - `set laststatus=2`
    - `set ru nu sc`

![图片描述](https://i0.hdslb.com/bfs/article/5298d194c8c0577f2fe8fb94639b9a25ecf194c2.png@942w_251h_progressive.webp)

- `:h options` 查询更多实用开关

## 各种实用开关

- `set number` 显示行号
- `set relativenumber` 显示相对行号
- `set cursorline` 光标所在的当前行高亮
- `set cursorcolumn` 光标所在的当前行高亮
- `set nocompatible` 使用 `vim` 模式，不与 `Vi` 兼容
- `syntax on` 打开语法高亮
- `set showmode` 在底部显示，当前所处模式
- `set showcmd` 命令模式下，在底部显示键入指令
- `set mouse-=a` 纯键盘操作
- `set encoding=utf-8` 使用 utf-8 编码
- `set autoread` 硬盘文件变化后，自动读取
- 把上述这些存储到 `~/.vimrc` 之后，以后这些配置就会自动起作用了
- 也可以去 `github` 搜索 `.vimrc` 找到关于配置的更多信息

## 查询开关 `option` 细节

- 查询某个设置的帮助可以加上单引号

- - `:h 'number'` 可以查找 `number` 相关的设定
    - `:h 'mouse'` 可以查找 `mouse` 相关的设定
    - `:h 'autoread'` 可以查找 `autoread` 相关的设定

![图片描述](https://i0.hdslb.com/bfs/article/87b1211594501f7aa01b18d782832dff9a0b39d1.png@942w_419h_progressive.webp)

## 最终的设定

- `set statusline=%-040.40(%F%m%)%-030.30([%l,%c]%)%p%%`
- `set laststatus=2`
- `set ruler`
- `set number`
- `set showcmd`
- `set nocompatible`
- `set showcmd`
- `set showmode`
- `set history=100`
- 你能把他们的含义都说清楚吗？🤪

## 总结

- 找到配置文件的位置 `~/.vimrc`

- - 了解各种配置开关
    - 修改配置文件并应用

- 不过这个颜色究竟是怎么配置的呢？🤔

- 下次再说 *

# vim - 23 - 配置文件

## 配置文件

## 回忆上节课内容🤔

- 我们上次找到配置文件的位置 `~/.vimrc`

- - 了解各种配置开关
    - 修改配置文件并应用

- 这次想了解和配色方案相关的内容

## colorscheme

- `vi ~/.vimrc.old` 中发现 `colorscheme` 属性

![图片描述](https://i0.hdslb.com/bfs/article/d81660c14a8494d4b91cfc22b0eb5de951687738.png@942w_735h_progressive.webp)

- 可以选择 `blue` 试试
- `:colorscheme blue`

## 智能提示

- 配色方案 `colorscheme` 的提示是怎么来的？

- 如果没有提示的话

- `:set wildmode?` 看一下

- - 默认是 `longest,list,full`

- 如果`:set wildmod=`

- - 智能提示就没有了

- `:set wildmode=longest,list,full`

- - 又会出现

- 还可以调出菜单 `:set wildmenu`

- - 再`:colorscheme` tab就没有用了
    - 如果 `:set nowildmenu` 就没有菜单了
    - tab其实就是 `wildchar`
    - 用来获取提示的

![图片描述](https://i0.hdslb.com/bfs/article/7521d10270e5331e368ff89954e4172b3e11e34f.png@924w_189h_progressive.webp)

## 选择配色方案

- 在命令行模式中输入 `:colorscheme` tab

- - 看到提示的配色方案
    - 用tab列出可选项
    - 然后选择一个配色方案

- 其实各种颜色可以来一个个的试试

## 配色方案举例

![img](https://i0.hdslb.com/bfs/article/4aee698bcc1a5bebbf382ae6529b4cd89ebea7b5.png@942w_2124h_progressive.webp)

- 你觉得哪个好看呢？

## 色彩模式选择

- 都试了一遍，觉得 `murphy` 或 `blue` 还行
- `:set t_Co?` 查看当前色彩模式
- `:set t_Co=256` 色彩模式设置为 256 色
- `:set t_Co&` 色彩模式设置为默认
- 观察颜色的细微变化
- `:h 't_Co'` 查询帮助

![图片描述](https://i0.hdslb.com/bfs/article/f8dc7b767868b7a7c1082d00ec74f4255d8c4106.png@942w_426h_progressive.webp)

- `t` 是 `terminal终端`

- `Co` 是 `Color颜色`

- 我们把这些写进配置文件 `~/.vimrc`

- - `set t_Co=256`
    - `colorscheme blue`

## 颜色模式的作用

- 这对于软件界面改变很大

- - 我们可以比较清晰地看到关键字、字符串、函数名等
    - 但是对于编写的程序和文本本身的内容
    - 并没有什么影响

- 只是比较好看的蓝布棉门帘

## 配置文件

- `set statusline=%-040.40(%F%m%)%-030.30([%l,%c]%)%p%%`
- `set laststatus=2`
- `set ruler`
- `set number`
- `set showcmd`
- `set nocompatible`
- `set showcmd`
- `set showmode`
- `set history=100`
- `set t_Co=256`
- `colorscheme blue`

## 更多细节

- `:h colorscheme` 可以找到配色方案的帮助

![img](https://i0.hdslb.com/bfs/article/cd7a239421fbd153301229a16002dc8163fa8b67.png@942w_630h_progressive.webp)

## 配色文件夹

\#找到vim的位置whereis vim#找到colors的位置find /usr/share/vim -name "colors"

![img](https://i0.hdslb.com/bfs/article/e811ebfd3b4068249d9ffd9d8603ab4521c565b3.png@942w_176h_progressive.webp)

## 网上寻找合适的配色方案

![图片描述](https://i0.hdslb.com/bfs/article/e41c1dabf41537d5e1c58593efb37902c79954d5.png@942w_740h_progressive.webp)

- 网址是 https://vimcolors.com/
- 选到合适的配色之后可以进入 `github` 去下载相应的配色文件
- 把下载的 `.vim` 文件放进 `colors` 文件夹就可以了
- 使用 `:colorscheme XXX` 应用该配色方案

## 下载颜色方案

\#下载颜色方案git clone https://github.com/gryf/wombat256grf.git#放到相应文件夹里sudo cp ./wombat256grf/wombat256grf.vim /usr/share/vim/vim81/colors#运行vi oeasy.java

- `:colorscheme wombat256grf`
- 颜色设置成功

## 把当前配色方案输出到 html

- `:TOhtml`

- 可以把当前的配色方案输出为网页格式

- - `:w oeasy.html`

![图片描述](https://i0.hdslb.com/bfs/article/80faca0d040ddc1f7e87486ac934c322df95a2dd.png@942w_653h_progressive.webp)

- 转化过程是一个vim文件

- - 也可以直接运行
    - `:source $VIMRUNTIME/syntax/2html.vim`

## 增加自己的配色方案

![img](https://i0.hdslb.com/bfs/article/21fb4e89089baa1644e213b1461a8f770c83ea40.png@942w_326h_progressive.webp)

\#找到colors的位置cd /usr/share/vim/vim81/colors#列出所有配色方案ls#复制出自己的配色方案sudo cp murphy.vim oeasy.vim

## 总结

- 这次我们研究了配色方案

- - 找到了 `colors` 的位置
    - 下载并应用了颜色方案
    - 制作了自己的配色方案

- 下面我想修改配色方案的颜色🤔

- - 最后在vim中尝试 `:colorscheme oeasy`
    - 是否能成功？？？

- 下次再说 *



# vim - 24 - 自定颜色

## 自定颜色

## 回忆上节课内容🤔

- 这次我们研究了配色方案

- - 找到了 `colors` 的位置
    - 下载并应用了颜色方案
    - 制作了自己的配色方案

- 下面我想修改配色方案的颜色🤔

- - 是否能成功？？？

## 首先得有自己的颜色方案

![img](https://i0.hdslb.com/bfs/article/21fb4e89089baa1644e213b1461a8f770c83ea40.png@942w_326h_progressive.webp)

\#找到colors的位置cd usr/share/vim/vim81/colors#列出所有配色方案ls#复制出自己的配色方案sudo cp murphy.vim oeasy.vim#查看配色方案信息sudo vi oeasy.vim

## 修改配色方案

![img](https://i0.hdslb.com/bfs/article/7e5385e3e6e40550e44a158063c62572665e8bde.png@942w_710h_progressive.webp)

- 前 5 行是注释

- 第 7 行取消原来的配色

- 第 8 行设置背景

- 第 9-11 行重设语法高亮

- 第 12 行命名此配色方案，可以修改为 `oeasy`

- 第 14 行开始设置各种高亮组的颜色

- 我们先修改第一个高亮组 `Normal`

- - 注释`Comment`
    - 常量`Constant`等
    - `Normal`的意思是`一般文字`
    - 这类的文字都属于这个高亮组
    - 与此类似的还有

## 改变 Normal 高亮组颜色

- 首先把配色方案名称改为 `oeasy`
- 找到 `Normal` 组
- 把 `Normal` 组的背景色`ctermbg` 改为 `blue`
- 把 `Normal` 组的前景色 `ctermfg` 改为 `yellow`
- `:w` 保存配色文件
- `colorscheme oeasy` 重新设定配色文件

![img](https://i0.hdslb.com/bfs/article/5103c07be70d0b1175a96713ca6c6da56a05b03a.png@942w_714h_progressive.webp)

## 查看配色

- `:hi Normal` 可以查看 `Normal` 组的配色
- `:hi` 可以查看当前色彩方案所有的配色
- `xxx` 就是效果预览

![img](https://i0.hdslb.com/bfs/article/f77d42b43502d32a8ed25375ec2ee25075bdf02f.png@942w_689h_progressive.webp)

## 配色细节

- `hi` 是 `highlight` 的缩写
- `:h hi` 可以查询帮助

![图片描述](https://i0.hdslb.com/bfs/article/fec2d1f5d428f55d6ef5c790b3bb9a885dbf82d8.png@942w_482h_progressive.webp)

## 字体特征

- `:hi StatusLine`
- `:hi StatusLine cterm=bold`
- `:hi StatusLine cterm=bold,italic`
- `:hi StatusLine cterm=bold,italic`
- `:hi StatusLine cterm=bold,italic,underline`
- `:hi StatusLine`

![图片描述](https://i0.hdslb.com/bfs/article/d1b3d71dafc7497ecc8e56fda111a7db36b07aa1.png@942w_617h_progressive.webp)

- `term`

- - 意思是`terminal`
    - 效果之间可以加逗号
    - 对应黑白终端
    - 在此无效

- `cterm`

- - bold 加粗
    - underline 下划线
    - italic 倾斜
    - NONE 取消任何效果

## 设置颜色

- `hi StatusLine`

- `hi StatusLine ctermfg=red ctermbg=blue`

- `hi StatusLine`

- `ctermfg`

- - 意思是`c`olor `ter`minal `f`ore `c`olor
    - 前景色设置
    - ctermfg=white

- `ctermbg`

- - 意思是`c`olor `ter`minal `b`ack `c`olor
    - 被景色设置
    - ctermfg=red

- `gui`相关的属性呢

- - 与`gui`相关
    - 当前终端中无效果

- 颜色对应的色号是来自系统的ansi对应的颜色值

## 定义光标所在行的颜色效果

- 设置光标行高亮显示
- `:set cursorline`
- `:h 'cursorline'`
- `:hi CursorLine`
- `:hi CursorLine ctermbg=red ctermfg=white`
- `:hi CursorLine`
- 随着光标的运动，CursorLine 也会移动

## 定义光标所在列的颜色效果

- 设置光标行高亮显示

- `:set cursorcolumn`

- `:h 'cursorcolumn'`

- `:hi CursorColumn`

- `:hi CursorColumn ctermbg=red ctermfg=white`

- `:hi CursorColumn`

- 随着光标的运动，CursorColumn 也会移动

- 如果有换行问题的话

- - `:set nowrap`

![图片描述](https://i0.hdslb.com/bfs/article/85d204ec4237959c7d2c5631428d791e2bc85f41.png@942w_774h_progressive.webp)

## 自定义颜色名

- 定义 `oeasy` 组

- - `:hi oeasy ctermbg=white ctermfg=red`

- 查看 `oeasy` 组

- - `:hi oeasy`

- 应用 `oeasy` 组

- - `:set statusline=%#oeasy#%F%*`

![图片描述](https://i0.hdslb.com/bfs/article/d741d31c63f2656dcf5195feb2eb22287680c599.png@942w_219h_progressive.webp)

## 配置文件

- `set statusline=%-040.40(%F%m%)%-030.30([%l,%c]%)%p%%`
- `set laststatus=2`
- `set ruler`
- `set number`
- `set showcmd`
- `set nocompatible`
- `set showcmd`
- `set showmode`
- `set history=100`
- `set t_Co=256`
- `colorscheme blue`
- `set cursorline`
- `hi CursorLine ctermbg=red ctermfg=white`
- `set cursorcolumn`
- `hi CursorColumn ctermbg=red ctermfg=white`

## 总结

- 我们这次深入了配色方案

- - 修改了方案中的具体配色
    - 建立了自己的配色
    - 应用了自己的配色

- 配置里面还有什么好玩的吗？🤔

- - 用来用去就是红绿蓝
    - 可以有更多颜色吗？

- 下次再说 *

# vim - 25 - 更多颜色

## 更多颜色

## 回忆上节课内容🤔

- 我们上次深入了配色方案
- 定义了自己的配色方案 `oeasy`
- 建立了自己的配色 `oeasy`
- 在状态栏应用了自己的配色

![图片描述](https://i0.hdslb.com/bfs/article/d741d31c63f2656dcf5195feb2eb22287680c599.png@942w_219h_progressive.webp)

## 明确能用的颜色

- 先胡乱地尝试一下修改颜色代码

- - `hi Normal ctermfg=1`
    - `hi Normal ctermfg=2`
    - `hi Normal ctermfg=3`

- 首先看看有多少能用的颜色

- - `:set t_Co?`

- 设置为 256 色的有颜色终端（cterm）显示模式

- - `:set t_Co=256`

- 那么这 256 种颜色都有什么呢？

- 我们尝试把他显示出来

## 显示某种颜色

- 显示某种颜色

echo -e "\033[48;5;1moeasy[0m"echo -e "\033[48;5;2moeasy[0m"echo -e "\033[48;5;3moeasy[0m"echo -e "\033[48;5;4moeasy[0m"echo -e "\033[48;5;5moeasy[0m"

![图片描述](https://i0.hdslb.com/bfs/article/c5f5f8246c5345c5772372b086ad6d4d2f54b933.png@942w_363h_progressive.webp)

## 尝试把所有颜色遍历出来

\#!/bin/bashfor c in {0..255}do   printf "\033[48;5;"$c"m%5d\033[0m" $cdone

- 保存并运行当前程序
- `:w|!sh %`

![图片描述](https://i0.hdslb.com/bfs/article/46e34707195737222808e9f1dfdf0293618366d4.png@942w_378h_progressive.webp)

- 确实符合ansi的规则
- 这不废话么？🤪

## 修改确认

- `:hi Normal ctermbg=196`
- `:hi Normal ctermbg=214`
- `:hi Normal ctermbg=124`
- 经过确认颜色基本能够对应上
- 这样我们就可以使用全部256种颜色了
- 哈哈哈哈
- 开心😁

## 更多颜色

- 当我打开了下载的color文件
- 就是上上次从vimcolors.com下载的
- git clone https://github.com/gryf/wombat256grf.git
- 发现了这个

![图片描述](https://i0.hdslb.com/bfs/article/e89765b1efe6b63a7cba72f3aea87e5270ca5948.png@942w_539h_progressive.webp)

- 看起来我们可以使用rgb颜色编码方式！！
- 怎么做的呢？看代码

## 转化过程

- 需要在代码里定义从rgb颜色模式到ansi颜色模式的转化函数
- 首先把rgb拆分为三个本地的分量

![图片描述](https://i0.hdslb.com/bfs/article/fe6618fb6eadf24831af3c8c74e9aa1cbbc92638.png@942w_441h_progressive.webp)

- 如果三个分量相等

![图片描述](https://i0.hdslb.com/bfs/article/3ccf628de11df999e19bc9d1c4a9a0575439d104.png@942w_452h_progressive.webp)

- 映射到相应具体的灰阶的值

![图片描述](https://i0.hdslb.com/bfs/article/addd9fd5a020fba1d71ffa771274d29b18cb111e.png@942w_236h_progressive.webp)

- 彩色怎么办呢？

## 彩色映射

![图片描述](https://i0.hdslb.com/bfs/article/4c073edb4cd79dece44d77fa4fdc95cde8d601ea.png@942w_432h_progressive.webp)

- rgb三个分量已经得到了
- 得到近似颜色

![图片描述](https://i0.hdslb.com/bfs/article/1c19e1180f0329ed589f8355478a4c5bc2c90d2e.png@942w_237h_progressive.webp)

- 然后再得到彩色的值

![图片描述](https://i0.hdslb.com/bfs/article/52b8aa5413eecaef118ad5914fc130648ea05d9c.png@942w_137h_progressive.webp)

- 这样我们就可以使用rgb颜色了
- 而且不论我们使不使用颜色映射
- 都可以用代码当前的配色方案直接生成颜色网页

## 生成网页

![图片描述](https://i0.hdslb.com/bfs/article/e7c57c8117b14f405a271f41d1739ece57160b2c.png@942w_683h_progressive.webp)

- 可以用自定义的颜色方案生成网页

- - `:TOhtml`
    - 或者 `:source $VIMRUNTIME/syntax/2html.vim`

- 然后在浏览器里打开他

![图片描述](https://i0.hdslb.com/bfs/article/cf6d75a5310c0ae47ce44e13f868f0bf2494b796.png@942w_860h_progressive.webp)

- `:firefox %`

## 总结

- 这次了解了颜色的细节

- 设置 256 色模式

- - `:set t_Co=256`

- 然后确定了具体的各种颜色

- 还可以生成网页

- 还有什么好玩的么？🤔

- 下次再说 *

# vim - 26 - 缩进设置

## 缩进设置

## 回忆上节课内容🤔

- 这次了解了颜色的细节

- 设置 256 色模式

- - `:set t_Co=256`

- 然后确定了具体的各种颜色

- 还可以生成网页 `:TOhtml`

- 还有什么好玩的么？🤔

![图片描述](https://i0.hdslb.com/bfs/article/46e34707195737222808e9f1dfdf0293618366d4.png@942w_378h_progressive.webp)

## 缩进设置

![图片描述](https://i0.hdslb.com/bfs/article/36de21171d77855acf6c3edddf89019407b61fbd.png@942w_419h_progressive.webp)

- 在正常模式下

- - 使用 `<<` 可以向前缩进
    - 使用 `>>` 可以向后缩进
    - =可以让当前行自动缩进

- 使用gg=G

- - 可以从头自动缩进到结尾

- 这超爽🤪

## 显示缩进

- 我们编程的时候会遇到缩进

- - 这缩进究竟是 `空格` 呢？还是 `tab` 呢？
    - 要把 `空格` 和 `tab` 区别开来

- `:set list` 使得列表生效

- - tab会被显示为 `^I`
    - 行尾会显示 `$`

![图片描述](https://i0.hdslb.com/bfs/article/ae42478427addf45deb13bdc50134d8a76e516d8.png@942w_233h_progressive.webp)

- `:set nolist` 使得列表失效

- - tab会被显示为空格缩进

![图片描述](https://i0.hdslb.com/bfs/article/14e4315a2b5bd7cb4f2d31f50f6ea7b8742f5900.png@942w_234h_progressive.webp)

- 但是好像缩进看起来只有两格了
- 与实际不符
- 能修改么？

## 定制 tab 显示

- 把特殊字符作为 `listchars` 组显示出来

- `:set listchars`

- 设置 `listchars`

- `:set listchars=eol:$,tab:>-,space:_`

- - `tab` 对应 `>-`
    - `>` 是开头
    - `-` 在后面补位

![图片描述](https://i0.hdslb.com/bfs/article/3a1289cb2c20259d05c89bfcf25e4c6329365d16.png@942w_477h_progressive.webp)

- `space` 对应 `_`
- `eol` 对应 `$`
- `:h listchars`可以查看相关手册

## 空格颜色

- `:hi SpecialKey ctermfg=DarkRed guifg=grey70`

- - 设置 `listchars` 相应的颜色
    - 设置得特殊一点

![图片描述](https://i0.hdslb.com/bfs/article/502c84f83380f779d7210509409f5b10a11af221.png@942w_914h_progressive.webp)

## 最终效果

![图片描述](https://i0.hdslb.com/bfs/article/cea0650763a686c832fc6d5ac60e1a34b069b4c4.png@707w_732h_progressive.webp)

- 建议统一能用 tab 的时候就用 tab
- 减小文件容量

![图片描述](https://i0.hdslb.com/bfs/article/a8378179d18d3c772799e97fede1977ed0a8abea.png@942w_227h_progressive.webp)

## 基础

- shiftwidth值是整个缩进的基础

- `:set shiftwidth=4`

- - `shiftwidth` 是一个基础的值，对应
    - 按下 `>>` 缩进的宽度
    - 按下tab缩进的宽度
    - 退格或者删除 `\t` 时缩进的宽度

- 一般 `tabstop`、`softtabstop` 都与他相同

- - 一般都是 4
    - 如果 `shiftwidth` 是 0 的话
    - 就按照 `tabstop` 来

## 解释 tab 宽度

- `tabstop` 是 `读取文件` 时用到的
- 读到 `\t` 字符时
- 解释他对应多少个空格的宽度
- 一般都是 4 个空格

![图片描述](https://i0.hdslb.com/bfs/article/25347bb49710b1e326a6d543ace602d67d96b58c.png@942w_471h_progressive.webp)

## softtabstop 处理空格的数量

- 如果 `softtabstop` 等于 0

- - 特性取消，一切按照 `tabstop` 来

- 如果 `tabstop=4`、`softtabstop=8`

- - 可以试试，能看出来
    - 1 次删除空格 8 个
    - 看起来像删了两个 tab
    - 一次插入 8 个位置
    - 看起来像插了两个 tab
    - 按下tab时
    - 要删除 tab 时

- 当他是负数的时候 `shiftwidth` 起作用

- 所以说 `shiftwidth` 是基础

![图片描述](https://i0.hdslb.com/bfs/article/0f6cb4388fc639b1cc2d0ebfc74587cb7be1ccf5.png@942w_525h_progressive.webp)

## 扩展 tab

- `:set expandtab`

- - 可以把输入的 `tab` 变成`空格`

- 设置好之后，在正常模式下

- - \>>
    - 或者在插入模式下tab的时候
    - 都看不到 `>---`，而是直接变成空格 `_`

- 反之 `:set noexpandtab` 之后

- - 插入的 `tab` 都还是 `>---`

- `:h expandtab` 可以查看相关手册

- - `expandtab` 可以简写为 `et`

![图片描述](https://i0.hdslb.com/bfs/article/3b98b4de15091c93254d88e7e839c472289cf66a.png@942w_281h_progressive.webp)

- 那已经存在的tab怎么办呢？

## 强制拓展

- `:retab!`
- 把已经存在的 tab 强制扩展成为空格

![图片描述](https://i0.hdslb.com/bfs/article/b09d1aa6b54d33b9426ea7b19d7b0f5279f07474.png@942w_471h_progressive.webp)

- 转过去之后
- 没有转回来的命令
- 慎重吧
- 我觉得tab挺好的

## 回车之后自动缩进

- `:set autoindent`

- - 可以简写为 `:set ai`
    - 添加与上一行一致的缩进
    - 取消为 `:se noai`

- `:set smartindent`

- - 简写为 `:se si`
    - 在 `autoindent` 的基础上根据 `{`、`}` 来调整本行缩进
    - 取消为 `:se nosi`
    - 需要保证 `:se nopaste`

- `:set cindent`

- - 根据类似于 c、java 的代码动态调节缩进
    - 见到 `if` 之类的可以自动缩进
    - 取消为 `:set nocindent`

![图片描述](https://i0.hdslb.com/bfs/article/8ca6987fd37ce42e2ea72f40100d2e3a3709c0a4.png@942w_297h_progressive.webp)

## 整体设定为

- `:set noexpandtab`
- `:set shiftwidth = 4`
- `:set tabstop =4`
- `:set softtabstop=4`
- `:set autoindent`
- 简写为 `:set noet sw=4 ts=4 sts=4 ai`
- 这都个人喜好
- 没有绝对规定

## 总结

- 这次了解了缩进的各种方式

- 正常模式下用 `<<` 缩进

- 插入模式下用 `tab` 缩进

- 有关于缩进对应空格数的参数

- - expandtab
    - shiftwidth
    - tabstop
    - softtabstop
    - autoindent

- 不同的文件类型可以对应不同的缩进吗？？🤔

- - python、java缩进4个
    - html、css可以缩进2个

- 下次再说 *

# vim - 27 - 文件类型

## 文件类型

## 回忆上节课内容🤔

- 上次了解了缩进的各种方式

- - 正常模式下用 `<<` 缩进
    - 插入模式下用 `tab` 缩进
    - 显示缩进情况 `:set listchars=eol:$,tab:>-,space:_`

- 有关于缩进对应空格数的参数

- - expandtab
    - shiftwidth
    - tabstop
    - softtabstop
    - autoindent

- 简写为 `:set noet sw=4 ts=4 sts=4 ai`

- 不同的文件类型可以对应不同的缩进长度吗？？🤔

## 检测文件类型

![图片描述](https://i0.hdslb.com/bfs/article/4440a39f16e04162106f07f2d5357196587190a6.png@942w_630h_progressive.webp)

- 首先需要检测文件类型

- `:filetype` 可以设置当前文件类型检测信息

- - `:filetype on` 检测文件扩展名
    - `:filetype off` 取消检测文件扩展名

- 如果是`.c`

- - 并且`:filetype on`
    - 就可以检测文件类型为 `.c`
    - 那我怎么知道 `filetype` 是什么呢？

- `:set filetype?`

- - 结果是 `filetype=c`

- 但是如何单独设置 `.c` 文件缩进为 `8` 呢？

## 文件类型缩进设置

- 我们书写一个 `demo.c`
- 可以发现这个文件 tab 是对应着 4 个空格的

![图片描述](https://i0.hdslb.com/bfs/article/e8d938586ac787d98fd1219954ab51beda684081.png@576w_426h_progressive.webp)

- 如果想单独设置 `.c` 文件类型的缩进的话

- - 需要打开文件类型缩进的开关
    - `:filetype indent on`

## 找到缩进配置文件

- 系统的配置文件的位置在 `/usr/share/vim/vim81/indent/`

- - `c` 缩进为 `8`
    - `java` 缩进为 `4`
    - `html` 缩进为 `2`
    - `c` 对应 `c.vim`
    - `java` 对应 `java.vim`
    - `html` 对应 `html.vim`
    - 不同的文件类型可以设置不同的缩进
    - 找到了 `/usr/share/vim/vim81/indent/c.vim` 就可以设置`c`的缩进

- 在最后加上

- - `:set et sw=8 ts=8 sts=8 ai`

- 然后退出并重新打开 `demo.c`

- 再gg=G

- 就可以按照新设置的 `/usr/share/vim/vim81/indent/c.vim`来重新控制缩进了

## 更改文件类型

![图片描述](https://i0.hdslb.com/bfs/article/2905008f46ec5262c2d6fa83b29764096be224f0.png@942w_707h_progressive.webp)

- 我们打开 `demo.c` 时,系统会检测他的文件类型

- 但是如果我们非要 `硬` 要说他是一个 `java` 文件会如何呢？🤪

- `:set filetype=java`

- 文件对于 `include` 之类的语法高亮消失了

- gg=G

- 让文件缩进的数量变回了 `4`

- - 按照`java`文件缩进的要求来做

- 高亮可以根据文件类型而不同么？🤔

## 文件类型语法高亮

\#找出所有的java.vim文件sudo find / -name "java.vim" 

- 找出所有和 java 有关的文件

![图片描述](https://i0.hdslb.com/bfs/article/df4453b36dffbb2dbe4795456d61424993989724.png@942w_150h_progressive.webp)

- 在 `indent` 下的 `java.vim` 负责缩进

- 在 `syntax` 下的 `java.vim` 负责语法高亮

- 语法高亮的设置在

- - `/usr/share/vim/vim81/syntax/`下面

![图片描述](https://i0.hdslb.com/bfs/article/dd4a4fe016615b1db4f71e648b445866801fc81f.png@942w_689h_progressive.webp)

- `:syntax on` 可以设置关键词高亮，这个是所有语法高亮的根开关

## 文件类型的插件

- 除此之外，也可以加载 `java` 文件类型的的插件 `plugin`

- - 文件类型插件可以设置一键编译运行、跳转到函数定义之类的
    - 前提是 `:set filetype plugin on`

- 文件类型插件的设置在

- - `/usr/share/vim/vim81/ftplugin/`下面
    - ftplugin = FileType Plugin

- 回忆文件类型缩进和语法

- - 在 `indent` 下的 `java.vim` 负责缩进
    - 在 `syntax` 下的 `java.vim` 负责语法高亮

- 在 `ftplugin` 下的 `java.vim`

- - 负责针对 `java文件类型` 的插件

## 命名规则

- 除了对于每个用户都好使的高亮、缩进和插件之外
- 用户还可以设置只对于自己好使的高亮、缩进和插件

![图片描述](https://i0.hdslb.com/bfs/article/26b79f29c16c1d25f29c3604908c5d7019e7893a.png@942w_482h_progressive.webp)

- 以 `java` 语言的插件来举例

- 系统通用文件夹

- - `/usr/share/vim/vim81/ftplugin/java.vim`
    - `/usr/share/vim/vim81/ftplugin/java_xxx.vim`
    - `/usr/share/vim/vim81/ftplugin/java/xxx.vim`

- 用户专用文件夹

- - `~/.vim/ftplugin/java.vim`
    - `~/.vim/ftplugin/java_def.vim`
    - `~/.vim/ftplugin/java/header.vim`

- 上面是命名的规则

- - java 对应的就是 filetype

## 文件夹不存在？

- 如果没有文件夹的话就要新建

- - `:!mkdir -p ~/.vim/ftplugin`
    - 注意是 `ftplugin` 而不是 `plugin`
    - `plugin` 里面的插件全部都被加载
    - `ftplugin` 里面的插件根据文件类型加载

## 尝试分文件类型进行控制

- 保存后

- 打开 java 文件时

- - 第三行 set statusline=[oeasy-java]%F%m
    - 状态栏告诉我这是 java 文件

- 打开 css 文件时

- - 状态栏告诉我这是 css 文件
    - 第三行 set statusline=[oeasy-css]%F%m

- 都设置好之后

- 分别打开java文件和css文件

![图片描述](https://i0.hdslb.com/bfs/article/781a06336f8b63f0772d25c453d0a9f5175c8194.png@942w_1298h_progressive.webp)

## 强行指定

![图片描述](https://i0.hdslb.com/bfs/article/68ade2dfcb991936d65394d8dfb0a17d228882b0.png@750w_213h_progressive.webp)

- 如果我偏说 `css` 文件是 `java` 文件会如何呢？

- - 可以注意到状态栏的变化
    - 由于不同文件类型 `filetype` 的 `syntax` 文件不同
    - 用 `css` 的语法去标注 `java` 的高亮组
    - 所以高亮显示的状态也不同

## 总结

- 根据扩展名我们可以设置某些特定类型文件的配置

- 相关文件类型的设置放在相应的文件夹里

- 文件类型缩进文件夹

- - `/usr/share/vim/vim81/indent/`

- 文件类型语法高亮文件夹

- - `/usr/share/vim/vim81/syntax/`

- 文件类型插件文件夹

- - `~/.vim/ftplugin/java.vim`
    - `~/.vim/ftplugin/java_def.vim`
    - `~/.vim/ftplugin/java/header.vim`
    - `/usr/share/vim/vim81/ftplugin/java.vim`
    - `/usr/share/vim/vim81/ftplugin/java_xxx.vim`
    - `/usr/share/vim/vim81/ftplugin/java/xxx.vim`
    - 系统通用文件夹
    - 用户专用插件文件夹

- 在 文件夹`~/.vim/ftplugin`中 的 `html.vim` 的设置

- - 只针对 `html`
    - 包括文件的缩进、配色、语法高亮、行号、状态栏等

- `:filetype indent on` 文件类型缩进生效

- `:filetype syntax on` 文件类型语法高亮生效

- `:filetype plugin on` 文件类型插件生效

![图片描述](https://i0.hdslb.com/bfs/article/ca374ce37ec8d749b74af587f373eb30f3979837.png@942w_294h_progressive.webp)

- 还有什么好玩的吗？🤔
- 下次再说 *

# vim - 28 - 水平移动

## 水平移动

## 回忆上节课内容🤔

- 根据扩展名我们可以设置某些特定类型文件的配置

- 相关文件类型的设置放在相应的文件夹里

- 文件类型缩进文件夹

- - `/usr/share/vim/vim81/indent/`

- 文件类型语法高亮文件夹

- - `/usr/share/vim/vim81/syntax/`

- 文件类型插件文件夹

- - `~/.vim/ftplugin/java.vim`
    - `~/.vim/ftplugin/java_def.vim`
    - `~/.vim/ftplugin/java/header.vim`
    - `/usr/share/vim/vim81/ftplugin/java.vim`
    - `/usr/share/vim/vim81/ftplugin/java_xxx.vim`
    - `/usr/share/vim/vim81/ftplugin/java/xxx.vim`
    - 系统通用文件夹
    - 用户专用插件文件夹

- 在 文件夹`~/.vim/ftplugin`中 的 `html.vim` 的设置

- - 只针对 `html`
    - 包括文件的缩进、配色、语法高亮、行号、状态栏等

- `:filetype indent on` 文件类型缩进生效

- `:filetype syntax on` 文件类型语法高亮生效

- `:filetype plugin on` 文件类型插件生效

![图片描述](https://i0.hdslb.com/bfs/article/353c484437bc634ca4ab3337f5e5ff184eaccb81.png@942w_294h_progressive.webp)

## 素材文件

- 首先我们打开一个绕口令

- - `git clone http://github.com/overmind1980/vimtutorial.git`
    - `vi -u NONE raokouling.txt`
    - 打开绕口令
    - 需要单行的长度超过 80 个字符

- 设置不换行

- - `:set nowrap`

- 设置状态条

- - `:set statesline=%f-[%l,%c]`
    - `:set laststatus=2`

- 把模式设置为非兼容

- - `:set nocompatible`

![图片描述](https://i0.hdslb.com/bfs/article/4c7000e31f8e216e422ce907450183882503a96a.png@942w_710h_progressive.webp)

## 横向滚动

- 一路l到屏幕的尽头
- 到 [1,80] 时候再按下l
- 整个屏幕发生横向滚动
- 然后光标移动到屏幕中心位置
- 光标坐标显示为 [1,81]
- 如果要回来的话也需要移动到左边缘
- 然后再按h️
- 整个屏幕滚动回来了

![图片描述](https://i0.hdslb.com/bfs/article/461b59486b4eb681f7b80ad8bf525ca130185388.png@942w_1479h_progressive.webp)

- 反复横跳

## 横滚幅度

- 横滚的幅度可以通过 `sidescroll` 来控制

- - 默认 0 是横向屏幕 80 字符的一半 40 字符
    - 如果我设置为 10 的话
    - 在最右边缘再向右的话，屏幕位置滚动 10 个字符
    - 从 [1,80] 到 [1,81] 的时候发生

- `:h sidescroll`

![图片描述](https://i0.hdslb.com/bfs/article/dcf9b18c89b3de6b147e018605a1d511bee5b4bd.png@942w_1479h_progressive.webp)

- 我们如果把 `sidescroll` 变成 1，屏幕横滚就会很柔和🤪
- 还是设置回10吧
- 反复横跳

## 横滚留位

- 每次我们的横滚都是在屏幕边缘发生的

- 能否到达边缘之前就能看见那边有什么？

- `:h sidescrolloff`

- - 默认是 0，到边缘才滚动
    - 如果我们设置为 20
    - 到 [1,60] 的时候,距离有边缘有 20
    - 这个时候l️整个屏就会向右`滚动幅度`
    - 也就是 `sidescroll` 所对应的 `10`

![图片描述](https://i0.hdslb.com/bfs/article/e07ed25631d01367866fce7fb52ab16e37f29473.png@942w_1479h_progressive.webp)

- 把 `sidescrolloff` 设置成 99，光标在横向总在中心位置🤪

## 横滚屏快键

![图片描述](https://i0.hdslb.com/bfs/article/f4eba49dc443796ed74e5d2d4694c16c258e65cc.png@942w_342h_progressive.webp)

- 其实横向滚动我们用的比较少
- 但在一屏中滚动比较常见

## 屏内跳转

![图片描述](https://i0.hdslb.com/bfs/article/9d23a762b6a588a68f8d2841d56548ec94956642.png@942w_270h_progressive.webp)

- 可以参照全屏跳转

- 前面加个 g

- - g0 就是跳到屏幕第一个字符
    - g^ 就是本屏幕内第一个非空字符
    - gm 跳到屏幕中间
    - gM 跳到整个文本中间
    - g$ 跳到屏幕末尾

## 自动换行

- 如果一行太长了我们可以让他 `:set wrap` 自动换行
- `:h wrap` 可以查看帮助手册📕
- `:set nowrap` 可以取消自动换行

![图片描述](https://i0.hdslb.com/bfs/article/7f7d88defb58a54b4e7617586910ae5b0b5336b3.png@942w_711h_progressive.webp)

## 向上一行

- 我们一般用j、k上下移动
- 但是如果自动换行之后，这上下就不只是一行了
- 先把行号显示出来 `:set nu`
- 我们可以通过gj、gk来自动换行的一行内上下移动

## 换行字符

- 我在行头句尾的时候

- 如果我想按方向键h、l换行

- - 结果是有效的

- 如果我用BackSpace

- - 结果是有效的

- 但是有的机器上，却无效

- 为什么呢？

- 这是一个属性option

- - `whichwrap`

- 先看看这个东西现在的值

- - `:set whichwrap?`

![图片描述](https://i0.hdslb.com/bfs/article/1a8592018520323a89c8f885c6075234275d35c6.png@789w_72h_progressive.webp)

- 把他设置回默认的值

- - `:set whichwrap&`
    - `&` 表示设置为默认值
    - 然后再观察现状

![图片描述](https://i0.hdslb.com/bfs/article/e1cf3fca49b6a29faeac77f754f662514aef8b65.png@432w_54h_progressive.webp)

- b,s 是什么意思呢

## 选项细节

- `:h 'whichwrap'`

![图片描述](https://i0.hdslb.com/bfs/article/d835cb05e6b22e7938967c37f8d21014bc9523d2.png@942w_477h_progressive.webp)

- 默认只有两个

- - b 是 <BackSpace> 退格
    - s 是 <Space> 空格

- 理论上h、l不好使

- `vi oeasy.java`

- - 重新用vi打开
    - h、l好使
    - 那他是在那里设置了h、l呢？

## 查找根源

vim ~/.vimrc

- `/whichwrap`

![图片描述](https://i0.hdslb.com/bfs/article/9f77e54f6ce960d88186039bb6eb3fa05606e112.png@942w_789h_progressive.webp)

## 总结

- 我们这次了解了横向滚动的相关信息

- - 横滚幅度 - `sidescroll`
    - 横滚留位 - `sidescrolloff`
    - 自动换行 - `wrap`

- gj、gk可以逐行上下移动

- 可以控制切换行的控制键 `whichwrap`

- 这就是横向移动的内容

- 不过程序中一般一行不会超过80个字符

- 纵向移动更为普遍

- 纵向移动有什么好玩的吗？🤔

- 下次再说 *

# vim - 29 - # 垂直翻页

## 垂直翻页

## 回忆上节课内容🤔

- 我们上次了解了横向滚动的相关信息

- - 横滚幅度 - `sidescroll`
    - 横滚留位 - `sidescrolloff`
    - 自动换行 - `wrap`

- gj、gk可以逐行上下移动

- 可以控制切换行的控制键 `whichwrap`

- 这就是横向移动的内容

- 不过程序中一般一行不会超过80个字符

- 纵向移动更为普遍

- 纵向移动有什么好玩的吗？🤔

- 我们先下载个长点的文档

- - http://users.csc.calpoly.
    - `git clone http://github.com/overmind1980/vimtutorial.git`

- 然后用无模式的方式打开他

- `vi -u NONE tomsawyer.txt`

## 边缘移动

- 首先设置非兼容 `:set nocompatible`
- 然后设置显示行号 `:se nu`
- 23G到 23 行
- j再向下的时候
- 屏幕发生滚动，光标位置如图

![图片描述](https://i0.hdslb.com/bfs/article/cb9711e757e8326a25120b15e2274b060c0c05f1.png@942w_1425h_progressive.webp)

## 上下留边

- 上下留边的话就要用 `:set scrolloff=2`
- 这样的话上下翻动的话，都会有 `2` 行的预留
- `:h scrolloff` 查看帮助
- `s`[croll]`o`[ff] 管的纵向保留边距
- 俗称留天留地

![图片描述](https://i0.hdslb.com/bfs/article/be923edff008ee1a4b615e19db474d8e20a7b742.png@942w_1425h_progressive.webp)

## 留边细节

- `scrolloff` 是一个 `option`
- 可以设定最小值
- 还可以查询细节 `:h 'scrolloff'`

![图片描述](https://i0.hdslb.com/bfs/article/b0b73c2c10eda7193ef770afad68fa815b9c9a6f.png@942w_356h_progressive.webp)

- `scrolloff` 管的是 `纵向` 留天留地

- `sidescrolloff` 管的是 `横向` 留天留地

- 也可以用 `HML` 命令测试一下

- - H到当前屏幕能到的最上行 High
    - M到当前屏幕正中 Middle
    - L到当前屏幕能到的最下行 Low

## 上下翻页

![图片描述](https://i0.hdslb.com/bfs/article/4c0ee375aaa9f0aa2807c634e1d855e4b6334960.png@942w_707h_progressive.webp)

- 在 `scroll.txt` 可以找到 `:h CTRL-F`

- - 使用ctrl+f可以向下走
    - `f` 的含义是 `forward` 向下走
    - 同理`b` 的含义是 `backward` 向上走
    - ctrl+b可以向上走

- 在翻页之前加上数字 [count] 可以实现一次翻 10 页

- - 如10ctrl+f
    - 或10ctrl+b
    - 注意观察cmd的位置

## 向上 N 行

- 我们可以用ctrl+e向下 1 行

- ctrl+e和j的不同是

- - ctrl+e光标所在文件位置不变，整个屏幕向上，除非到了边缘，光标位置才改变
    - j是屏幕整个位置不变，光标位置向下，除非到了边缘，屏幕位置才改变

![图片描述](https://i0.hdslb.com/bfs/article/88b149bff43882a99e24e5f27125d70b7e362247.png@942w_707h_progressive.webp)

- 同理可以ctrl+y屏幕向下移动
- 他们都可以使用 `[count]` 来翻倍

## 翻过半屏

- ctrl+d可以向下走 翻半屏 d 代表 Down
- ctrl+u可以向上走 翻半屏 u 代表 Up
- 默认翻的是半屏，但是也可以通过 `scroll` 来设置
- `:set scroll=5` 来明确翻的行数
- 翻页的时候，光标在屏幕的相对位置不变，屏幕整体向上或向下移动

![图片描述](https://i0.hdslb.com/bfs/article/563e138e69d813718baaa54d4ad36aabc54ebb0f.png@942w_639h_progressive.webp)

## 总结

- 这次我们主要讲的翻页

- `:set scrolloff=2` 控制留天留地

- 上下翻页(这个最常用)

- - ctrl+f屏幕向上走一屏
    - ctrl+b屏幕向下走一屏

- 上下移屏一行

- - ctrl+e屏幕向上走一行
    - ctrl+y屏幕向下走一行

- 上下移屏一段

- - ctrl+u向上走半屏
    - ctrl+d向下走半屏
    - 移动数量和 `scroll` 相关

- 上述翻页都可以用 `[count]` 翻倍

- 如果想屏幕相对文件位置不动

- - 只移动光标

- 可以么？🤔

- 下次再说 *
    vimtutorial是oeasy制作的的一套关于vim的教程
    Github地址→https://github.com/overmind1980/vimtutorial
    Gitee地址→https://gitee.com/overmind1980/vimtutorial
    蓝桥实验楼地址→https://www.lanqiao.cn/teacher/courses/2840 邀请码FJWYIMGB

# vim - 30 - # 屏位行号

屏位行号回忆上节课内容🤔上次我们主要讲的翻页`:set scrolloff=2` 控制上下留天留地上下翻页（这个最常用）ctrl+f向下一屏ctrl+b向上一屏上下移屏一行ctrl+e屏幕向上一行ctrl+y屏幕向下一行上下移屏一段ctrl+u向上半屏ctrl+d向下半屏移动数量和 `scroll` 相关上述翻页都可以用 `[count]` 翻倍屏幕位置`:h H` 可以找到在屏幕位置不动时，移动光标的办法H- `Head` 移动到屏幕的顶端M- `Middle` 移动到屏幕的中间L- `Low` 移动到屏幕的底部会保持屏幕位置不变,把光标移动到允许的高中低位置

![图片描述](https://i0.hdslb.com/bfs/article/00751bcf20548da4c5dc8f24a0ea944f33e7de99.png@942w_524h_progressive.webp)

到达底端

![图片描述](https://i0.hdslb.com/bfs/article/44be3fa336ad302fa6ce83cf92d761ef6adf3ca2.png@942w_714h_progressive.webp)

L无法到底?`:set scrolloff?``:set scrolloff=0`L到底计算偏移2H会移动到距离屏幕最顶端 第2行 的位置3L会移动到距离屏幕最底端 倒数第3行 的位置

![图片描述](https://i0.hdslb.com/bfs/article/3dec949d09236f2e11cbbbdd17533bcc1fd63abc.png@942w_567h_progressive.webp)



## 光标固定

- `:h zt`

- - 可以光标保持当前位置，移动屏幕，让光标出现在顶部

- zt

- - 出现在光标在屏幕顶部
    - `top`
    - 光标在函数名上
    - 直接看到函数的函数体

- zz

- - 光标在屏幕中间

- zb

- - 光标出现在屏幕底部
    - `bottom`

- 光标位置受到 `scrolloff` 影响

## 总结

- 上次讲的翻页

- 这次先让屏幕位置固定，移动光标

- - H- `Head` 移动到屏幕的顶端
    - M- `Middle` 移动到屏幕的中间
    - L- `Low` 移动到屏幕的底部

- 然后让光标固定，移动屏幕的位置

- - zt- `top`
    - zz- 光标在屏幕中间
    - zb- `bottom`

- 还有什么快速移动的方法吗？🤔

- 下次再说 *

# vim - 31 - # 文字区块

## 文字区块

## 回忆上节课内容🤔

- 上上次讲的翻页

- 上次先让屏幕位置固定，移动光标

- - H- `Head` 移动到屏幕的顶端
    - M- `Middle` 移动到屏幕的中间
    - L- `Low` 移动到屏幕的底部

- 然后让光标固定，移动屏幕的相对位置

- - zt- `top`
    - zz- 光标在屏幕中间
    - zb- `bottom`

## 逐段移动



```javascript
#首先下载文本找到tomsawyer.txtgit
clone http://github.com/overmind1980/vimtutorial.git
#然后把文本打开
cd vimtutorial
vi tomsawyer.txt
```



- 使用大括号

- }

- - 让光标向后移动一段

- {

- - 让光标向前移动一段

- 段落是用回车符区分的一段段的文字

- 可以使用 `[count]` 翻倍

- `:h }` 来查看文档

![图片描述](https://i0.hdslb.com/bfs/article/7e17f761aaa2323cb77426c6942693f03fdd1445.png@942w_168h_progressive.webp)

## 逐句移动

- 使用小括号

- )

- - 让光标向后移动一句

- (

- - 让光标向前移动一句

- 句子是靠 `.` 区分的文字块

- 可以使用 `[count]` 翻倍

- `:h )` 来查看文档

![图片描述](https://i0.hdslb.com/bfs/article/aca683559d41da7c3a14744029d08ae4afbc5a6e.png@942w_195h_progressive.webp)

## 总结

- 这次内容很简单，主要针对文本类素材

- 移动段落

- - {向前
    - }向后

- 移动句子

- - (向前
    - )向后

- 如果我想在程序中快速移动

- 怎么办呢？🤔

- 下次再说 *

# vim - 32 - # 函数跳转

## 程序移动

## 回忆上节课内容🤔

- 上次内容很简单，主要针对文本类素材

- 移动段落

- - {向前
    - }向后

- 移动句子

- - (向前
    - )向后

- 如果我想程序中快速移动

- 怎么办？🤔



```javascript
#首先下载文本找到tomsawyer.txt
git clone http://github.com/overmind1980/vimtutorial.git
#然后把文本打开
cd vimtutorial
vi oeasy.java
```



## 括号间跳转 %

- 当我们的鼠标在小括号内部时

- - 我们可以使用 `%` 跳转到括号对的前半部分
    - 然后我们可以使用 `%` 在这对儿括号的两个位置指间跳转
    - 比如在 `public static void main(String[] args)` 中的 小括号`(` 上

- 这个 `%` 不但对于小括号有用，对于成对的大括号、中括号也都有用

- - 对于c语言的 /   ...   / 注释的头尾 ୧(﹒︠ᴗ﹒︡ )୨有用
    - 对于 #if，#ifdef，#else，#elif，#endif 也有用
    - 这个 `%` 不支持 `[count]`

![图片描述](https://i0.hdslb.com/bfs/article/3eb90eda6bcbace9c3e6b5a06b448046e86a2466.png@942w_569h_progressive.webp)

## 小括号跳转

![图片描述](https://i0.hdslb.com/bfs/article/8d085d6c690431c119b877411a34ecf7fa051f04.png@942w_282h_progressive.webp)

- 方向

- - ]) 近挨着的下一个)
    - [( 进挨着的上一个(
    - [ 往上
    - ] 往下

- 如果是大括号呢？

## 括号跳转

![图片描述](https://i0.hdslb.com/bfs/article/8d1a56eae67833ad8a011167c38a4681919e53e7.png@942w_474h_progressive.webp)

- `[(` 跳转到上一个没配对的 `(`
- `])` 跳转到下一个没配对的 `)`
- `[{` 跳转到上一个没配对的 `{`
- `]}` 跳转到下一个没配对的 `}`
- 支持 `[count]`
- 向上就是[
- 向下就是]

## 函数中的跳转

![图片描述](https://i0.hdslb.com/bfs/article/7355389bc003294c79b4089623b0a9faa6a3cb40.png@942w_431h_progressive.webp)

- 方向

- - ]} 近挨着的下一个}
    - ]] 本块的最后一行
    - [{ 紧挨着的上一个{
    - [[ 本块的第一行
    - [ 往上
    - ] 往下

## 注释的头尾

- 注释跳转

- - `[/`、`[*`上一个注释`/*  .... */`的头
    - `]*`、`]/`下一个注释`/*  .... */`的头

![图片描述](https://i0.hdslb.com/bfs/article/9ecc6adbf06979d6a1aee667fad76ae1af5d07ff.png@942w_291h_progressive.webp)

## 函数间跳转

![图片描述](https://i0.hdslb.com/bfs/article/ff510113158df3f4283cb101f6cb6deb1a04fb2a.png@942w_594h_progressive.webp)


-函数跳转

\- `[m`下一个函数开头 - `[M`上一个函数结尾 - `]m`下一个函数开头 - `[M`上一个函数结尾 - 支持 `[count]`   - `3]m` 可以往下跳到第 `3` 个函数开头 - `[m`、`]m` 这两个其实还挺好用的

## 跳到定义

![图片描述](https://i0.hdslb.com/bfs/article/1f0bacbf4c7426de5fe74724bbc21208aaa38c29.png@942w_426h_progressive.webp)

- 找到本地定义
- gd - goto global declaration

![图片描述](https://i0.hdslb.com/bfs/article/5245f683f7368a6d7ef1044cdfadb2f5b91a9749.png@942w_401h_progressive.webp)

- 和 * 不一样的是它会往前找到第一个
- 在 `[[` 的范围内的第一个

## 没有配对的 #if 宏定义

- 这个是针对宏定义里面的内容来的

- - `[#` 上一个没有配对的 `#if`、`#else`
    - `]#` 下一个没有配对的 `#else`、`#endif`

![图片描述](https://i0.hdslb.com/bfs/article/6bca675fe6abadc861b4c11098818f787e4ba7c3.png@942w_236h_progressive.webp)

## 标签跳转



```javascript
#查找matchit.vim
sudo find / -name matchit.vim
# 把match.vim插件放到系统插件文件夹
cp /usr/share/vim/vim81/macros/matchit.vim /usr/share/vim/vim81/plugin
#打开一个网页
vi oeasy.html
```



![图片描述](https://i0.hdslb.com/bfs/article/a3ea14b00870801e3ca809f434bdb4e5ff031214.png@942w_87h_progressive.webp)

- 这个matchit可以支持标签的跳转
- 比如在 `<html>` 处按下 `%` 就可以到配对的 `</html>`
- 挺好玩的
- 试试吧 🤪

## 总结

- 括号间跳转

- - `[(` 跳转到上一个没配对的 `(`
    - `[)` 跳转到下一个没配对的 `)`
    - `[{` 跳转到上一个没配对的 `{`
    - `[}` 跳转到下一个没配对的 `}`
    - 成对括号间跳转 `%`
    - 不成对括号间跳转

- 函数间跳转

- - `]m` 下一个函数开头
    - `[m` 上一个函数结尾
    - `]M` 下一个函数开头
    - `[M` 上一个函数结尾

- `#if`、`#else`、`#endif` 没有配对的

- - `[#` 上一个没有配对的 `#if`、`#else`
    - `]#` 下一个没有配对的 `#else`、`#endif`

- 注释的头尾

- - `[/`、`[*` 上一个注释 `/*  .... */` 的头
    - `]*`、`]/` 下一个注释 `/*  .... */` 的头

- 如果我想快速找到某个东西怎么办呢？🤔

- 下次再说 *

# vim - 33 - # 查找文本

## 文字区块

## 回忆上节课内容🤔

- 括号间跳转

- - `[[ `跳转到`本块开头`
    - `]]` 跳转到`本块结尾`
    - `[{` 跳转到上一个没配对的 `{`
    - `]}` 跳转到下一个没配对的 `}`
    - 成对括号间跳转 `%`

- 函数间跳转

- - `]m` 下一个函数开头
    - `[m` 上一个函数开头
    - `]M` 下一个函数结尾
    - `[M` 上一个函数结尾

- `#if`、`#else`、`#endif` 没有配对的

- - `[#` 上一个没有配对的 `#if`、`#else`
    - `]#` 下一个没有配对的 `#else`、`#endif`

- 注释的头尾

- - `[/`、`[*`上一个注释`/*  .... */` 的头
    - `]*`、`]/`下一个注释`/*  .... */` 的头

- 这次我想自定义跳转，就是查找某些东西

## 查找帮助

- 用无模式打开 `tomsawyer.txt`

- - `vi -u NONE tomsawyer.txt`

- 开启行号 `:se nu`

- 按下/

- - 会在左下角显示
    - 就像 `:` 等待输入命令一样
    - 输入待搜索字符串
    - `/TOM` 会从光标位置向后查找 `TOM`
    - 然后光标跳转到 `TOM` 的位置

- 可以 `h /` 查阅手册

![图片描述](https://i0.hdslb.com/bfs/article/af474f9cca42f3903a5de850ec5d0aacca578173.png@942w_566h_progressive.webp)

## 设置高亮

- 设置高亮开关

- - `:set hlsearch`
    - 简写为 `:set hls`
    - 可以看到查找的单词已经高亮显示出来

- 设置高亮色

- - `:hi Search ctermbg=red ctermfg=black` 注意大小写
    - `/TOM` 再次搜索 `TOM`
    - 搜索结果会高亮显示

- 可以使用 `:h 'hls'` 查找搜索高亮手册

![图片描述](https://i0.hdslb.com/bfs/article/483a4615be2feb6e08f7bec0a4e3335bf5db2876.png@942w_713h_progressive.webp)

## 取消高亮

- 如果你看到高亮显示太乱

- - 你可以反过来设置一下
    - `:set nohlsearch` 把搜索高亮的开关关掉
    - 当然下次你要想显示的话
    - 就需要再次打开开关 `:set hls`

- 如果你只想要眼下这把关了高亮

- 下次搜索的时候还是高亮的话

- - `:noh[lsearch]`

- 注意这是执行一个命令，而不是设置一个开关

![图片描述](https://i0.hdslb.com/bfs/article/c866aaa3ef5ee3415a24f6baebe179de688cc358.png@942w_222h_progressive.webp)

## 正向反向

- 遍历匹配

- - n下一个匹配项
    - N上一个匹配项
    - n、N可使用 `count` 翻倍

- `:h n` 查阅相关手册

- 一路n

- - 可以显示查阅到文档结尾
    - 如果想要重头查询的话
    - 需要设置 `:set wrapscan`
    - 这样就可以重头开始再查一次了
    - `w[rap]s[can]` 可以简写为 `ws`
    - 关掉开关用 `:set now[rap]s[can]` 可以简写为 `:set nows`

![图片描述](https://i0.hdslb.com/bfs/article/c3e35fdb231d19f8844399dab5e8067556714d43.png@942w_707h_progressive.webp)

## 反向查询

- 使用?可以反向查询单词

- - 比如 `?TOM` 就可以从后往前查询 `TOM`

- 遍历匹配

- - 因为负负得正？🤪
    - n保持方向，从下往上查询下一个
    - N改变方向，从上往下查询下一个
    - 如果用 `?TOM` 配合N就是往前查找
    - 到头了 `wrapscan` 让他可以从头再来

## 回顾行内搜索

- 总结行内搜索规律

- - f正向，F反向
    - t正向，T反向
    - ;保持方向，,改变方向

- `[count]` 可翻倍

## 总结

- 这次是搜索

- - /正向，?反向
    - n保持方向，N改变方向
    - `hls` 让搜索结果高亮
    - `noh` 取消本次高亮
    - `wrapscan` 可以从头搜索

- 查找还有什么好玩的呢？

- 下次再说 *

# vim - 34 - # 查找进阶

## 查找进阶

## 回忆上节课内容🤔

- 上次是搜索，是全文搜索

- 和我们以前的行内有点像

- - /正向，？反向
    - n保持方向，N改变方向
    - `hls` 让搜索结果高亮
    - `wrapscan` 可以从头搜索
    - `noh` 取消本次高亮

## 实时搜索

- `:set incsearch`

- - 实时匹配搜索输入

- `:set noincsearch`

- - 不实时匹配搜索输入

![图片描述](https://i0.hdslb.com/bfs/article/7e811e89b7afd40958afb84e665285a7a5a8a909.png@942w_719h_progressive.webp)

## 大写小写

- 如果查找要忽略大小写的话

- - 就用 `ignorecase`
    - `:set ignorecase`
    - 简写为 `:se ic`
    - 取消为 `:se noic`

- `:se ic` 可以和 `:set smartcase` 智慧大小写配合

- - 如果搜索模式里面有 `大写字母` 就完全匹配
    - 如果没有 `大写字母` 就忽略大小写

- 还可以直接在搜索项里加开关

- - `/oeasy\c` 不区分大小写的 `oeasy`
    - `/oeasy\C` 区分大小写的 `oeasy`

- 具体可以 `:h ignorecase`

![图片描述](https://i0.hdslb.com/bfs/article/837fd04fb1bc24281611af0744e816a1f9a1116b.png@942w_710h_progressive.webp)

## 查找当前

- 如果我们在一个单词上面的时候

- - 按下*
    - 就是查找当前光标所在的单词
    - 这很适合查找某个函数名
    - 或者查找变量名的引用

- 继续遍历搜索

- - n保持方向
    - N改变方向

- \#

- - 向上进行查找

- *、#

- - 刚好是电话按键中的对称两个

![图片描述](https://i0.hdslb.com/bfs/article/094960ad9ca811bebe7df12009c5f02b3c2b018a.jpg@942w_630h_progressive.webp)

## 明确头尾的单词

- 如果我查找的是 `/as`

- - `as` 符合要求
    - `ask` 符合要求
    - `has` 也符号要求
    - `oeasy` 都符合要求

- 要以 `as` 为单词结尾

- - `/as\>`
    - `as` 符合
    - `has` 符合

- 要以 `as` 为单词开头

- - `/\<as`
    - `as` 符合
    - `ask` 符合

- 我们就要 `as` 这个单词

- - `/\<as\>`
    - 只有 `as` 符合

![图片描述](https://i0.hdslb.com/bfs/article/f61c9951ef07b11388bc8a439f73a31912ca35a5.png@942w_404h_progressive.webp)

## 快速不按单词查找

- 如果我们使用*的话

- - 是按照整个单词查找的
    - 比如放到 `as` 的 `a` 上
    - 就是说查到的一定得是个完整单词
    - `/\<as\>`

- 如何不按照单词查找呢？

- - `oeasy` 也符合要求
    - 比如放到 `as` 的 `a` 上，
    - g*、g#进行查找
    - 只要有 `as` 就算

![图片描述](https://i0.hdslb.com/bfs/article/1c783d22ba1a2a31cd059e325da75464f1ca8117.png@942w_285h_progressive.webp)

## 设置 vim

- 如果关于搜索高亮的这些设置你想每次打开 `vim` 就设置好
- 那需要设置当前用户的vim配置文件 `vi ~/.vimrc`
- G到文件的尾部
- o在下面新建一行
- `set hlsearch` 设置搜索高亮
- `set wrapscan` 设置从头搜索
- 然后重启这些配置就永远保存在你这个当前用户的 `vim` 里面了
- 当然，如果是实验楼重启新环境的话会消失

## 总结

- 实时搜索

- - `:set incsearch`

- 大写小写

- - `ignorecase`

- 查找当前单词

- - *正向按单词完全匹配
    - \#反向按单词完全匹配
    - g*正向不按单词匹配
    - g#反向不按单词匹配

- 继续查找

- - n保持方向
    - N改变方向

- 这个搜索可以做一些模糊匹配吗？

- 下次再说吧 *

# vim - 35 - # 正则表达

## 正则表达

## 回忆上节课内容🤔

- 实时搜索 `:set incsearch`

- 大写小写 `ignorecase`

- 查找当前单词

- - *正向按单词
    - \#反向按单词
    - g*正向不按单词
    - g#反向不按单词

- 继续查找

- - n保持方向
    - N改变方向

- 这个搜索可以做一些模糊匹配吗？

- 应该在哪里查询呢？

## 模式匹配

- `:h /` 可以找到关于搜索相关的帮助

- - 我们可以打开 `patterns.txt`
    - 找到关于比较简单的解释 `03.9` 的超链接位置
    - ctrl+]跳转文档

![图片描述](https://i0.hdslb.com/bfs/article/1e22f05dcda1d2191c2ec4705897362f337c7784.png@942w_714h_progressive.webp)

## 行头行尾

![图片描述](https://i0.hdslb.com/bfs/article/7c9fbd65d7f2fbce808e068e3ca991e29a97b90c.png@942w_705h_progressive.webp)

- `/include` 匹配所有的 `include`

- `^` 意味着行开头

- - `/^include` 只匹配 `include` 在行头的
    - `/^#` 只匹配 `#` 在行头的

- `$` 意味着行结尾

- - `/the.$` 只匹配 `the.` 在行尾的
    - `/^End$` 匹配行头接着 `End`，然后就是行尾的一行

- `:g/^$/d` 删除所有空行

- 行头行尾和词头词尾很像

- `^` 本身就是跳到行头

- `$` 本身就是跳到行尾

## 任意字符

- `.` 可以匹配任意字符，作为通配符来使用

- 比如 `/c.m`

- - 第一个字符为 `c`
    - 第二个字符为 `.` 就是任意字符
    - 第三个字符为 `m`

- 可以匹配 `company` 中的 `com`

- 也可以匹配 `camera` 中的 `cam`

![图片描述](https://i0.hdslb.com/bfs/article/08716767db47f17fa55d9fef6f23c935126a7233.png@942w_701h_progressive.webp)

## 任意字符

- `ter.` 匹配 `ter` 后面加一个字符

![图片描述](https://i0.hdslb.com/bfs/article/36ad0eaab697537e1c322d76cdb82f21b28a281e.png@942w_165h_progressive.webp)

- 如果想要正常匹配一个真的 `.`

- - `.`就不再代表任意字符了
    - 比如搜索 `/ter\.` 就是寻找 `ter.`
    - 就要加上一个反斜杠 `\`
    - 写做 `\.`
    - 使用反斜杠 `\` 转义之后

## 更多字符

- `.` 代表任意字符

- - `/c.m` 匹配 `c和m中间有一个字符` 的情况
    - `/c..m` 匹配 `c和m中间有两个字符` 的情况
    - `/c...m` 匹配 `c和m中间有三个字符` 的情况

- 如果我想查找 c 和 m 中间有任意多个字符怎么办？

- - `/c.*m` 在 `c` 和 `m` 中间出现 0 到任意多个 `.`（任意字符）
    - 如果我希望出现任意多次的是小写字母怎么办？
    - `/c[a-z]*m` 这样就是中间出现任意多个 `[a-z]小写字母` 了
    - 使用 `*` 通配符
    - `/a*` 意味着出现 0 到任意多个 a

- `:g/^s*$/d` 删除搜有只有空格和tab的行

- - `s`代表空格和tab

![图片描述](https://i0.hdslb.com/bfs/article/9a3fb33980ad05a2c6f6a3674ca65cc17a0c4979.png@942w_752h_progressive.webp)

## 词头词尾

- `^` 和 `$` 分别代表着行头和行尾
- 再回一下词头词尾
- 如果我想找出单词的开头结尾是某些字符的怎么办呢？

![图片描述](https://i0.hdslb.com/bfs/article/cd8e9eb69aa376e6ff60c7fb19596c7d66a1e6c2.png@942w_519h_progressive.webp)

- `\<` 意味着单词开头

- - `/\<a` 意味着 `a` 开头的单词

- `\>`意味着单词结尾

- - `/\>b` 意味着 `b` 结尾的单词

- `\<a[a-z]*\>b`

- - 意味着以 a 开头，b 结尾，ab 之间可能有零到任意多个字符的单词

## 搜索历史

- 我们使用 `*`、`#` 查找的时候就自动给加上这个词头词尾

- - 可以*之后
    - /
    - 配合上下方向键看到
    - 曾经的搜索记录

![图片描述](https://i0.hdslb.com/bfs/article/563fcc07502c0b523521363bbdd6c2bb18a3d392.png@942w_285h_progressive.webp)

## 推荐网站

- 推荐一个好玩的网站
- https://blog.robertelder.org/regular-expression-visualizer/
- 可以可视化的观察正则匹配的过程

## 总结

- 行头行尾

- - `^` 意味着行开头
    - `$` 意味着行结尾

- 任意字符

- - `.` 代表任意字符
    - `[a-z]` 代表任意小写字母

- 字符数量

- - `*` 代表 0 到任意多个前字符
    - `+` 代表 1 到任意多个前字符
    - `?` 代表 0 或 1 个前字符

- 行头行尾

- - `\<` 意味着单词开头
    - `\>` 意味着单词结尾

- 正则表达式的初步规则先介绍到这里

- 我们掌握了在 vi 中光标运动的各种方法

- 但如何编辑文本呢？🤪

- 下次再说 *

# vim - 36 - # 插入字符

## 插入字符

## 回忆上节课内容 🤔 正则表达式

- 行头行尾

- - `^` 意味着行开头
    - `$` 意味着行结尾

- 任意字符

- - `.` 代表任意字符
    - `[a-z]` 代表任意小写字母

- 字符数量

- - `*` 代表 0 到任意多个前字符
    - `+` 代表 1 到任意多个前字符
    - `?` 代表 0 或 1 个前字符

- 行头行尾

- - `\<` 意味着单词开头
    - `\>` 意味着单词结尾

- 我们掌握了在 `vi` 中光标运动的各种方法

- 但如何编辑文本呢？🤪

## 简单操作

ls -l > oeasy.txt ll > oeasy.txt vi oeasy.txt

- i进入插入模式
- 插入字符串 oeasy
- esc退回到命令模式
- 移动一下位置
- .是重做
- u是撤销

## 字符大小

![图片描述](https://i0.hdslb.com/bfs/article/1fbada2249e9b71277d0844eade1bc2466e9692d.png@750w_627h_progressive.webp)

- 修改默认字体大小

- - 编辑菜单 - 首选项
    - 外观选项卡
    - 字体大小调整为 40
    - 确认

## 插入字符

- i切换到插入状态

- - 输入ctrl+v
    - 然后再输入 `065`
    - 会插入一个 `A `字符

- 注意在 `插入` 状态下ctrl+v

![图片描述](https://i0.hdslb.com/bfs/article/ff4f36eed115813f5679501f6d4ea4a0a455d93d.png@942w_753h_progressive.webp)

## 查询帮助

- 查询帮助
- `:h i_ctrl-v` 表示查询 `i`nsert（插入状态下的），ctrl+v对应的操作
- 找到 `i_CTRL-V_digit` 超链接，ctrl+]进入

![图片描述](https://i0.hdslb.com/bfs/article/5e8c35d30fdd5833af09536ef0c4e90a78dbaa27.png@942w_518h_progressive.webp)

## 十进制 ascii 字符

- `065` 使用的是 `十进制`
- 对应十进制值为 `065` 的 ascii 字符 `A`
- 如下是ascii 的对应表格

![图片描述](https://i0.hdslb.com/bfs/article/d0bba1db3bd197ab2511b971bba5c38a9f278654.png@942w_1145h_progressive.webp)

## 插入 unicode 字符

![图片描述](https://i0.hdslb.com/bfs/article/8bd90f8594d5712e2dcebd7202e4daede3fda006.png@942w_213h_progressive.webp)

- 可以使用 https://unicode-table.com/cn/search/ 进行编解码转化

- 比如搜索 `♂`，可以找到 `2642` 😂

- 然后再输入状态下ctrl+v之后输入 `u2642` 就可以输入这个字符了

- 还有些什么好玩的字符吗？

- - ☯ 太极 u262F
    - ⚊ 阳爻 u268A
    - ⚋ 阴爻 u268B
    - ⚌ 太陽 u268C
    - ⚍ 少陰 u268D
    - ⚎ 少陽 u268E
    - ⚏ 太陰 u268F

- 用心找的话，还可以找到八卦和六十四卦

- 甚至各种生僻汉字

- 如果终端支持的话也可以显示emoji😊

## 二合字符

- vim还支持使用二合字符
- `h dig(raphs)`

![图片描述](https://i0.hdslb.com/bfs/article/5e25ae01907c07147a87424d6bb9111a4905cb6e.png@942w_699h_progressive.webp)

- i切换到插入状态（注意当前状态处于插入状态）

- - ©    Co    0xa9   169   COPYRIGHT SIGN
    - 可在上图中找到
    - 输入ctrl+k进入二合字符输入状态
    - 输入 `Co`（注意大小写）可得到 `©`

- 可以快速输入分数

- - ⅓    13    2153   8531   VULGAR FRACTION ONE THIRD
    - ⅔    23    2154   8532   VULGAR FRACTION TWO THIRDS
    - ⅕    15    2155   8533   VULGAR FRACTION ONE FIFTH
    - ⅖    25    2156   8534   VULGAR FRACTION TWO FIFTHS

- 可以输入编号

- - ⒈    1.    2488   9352   DIGIT ONE FULL STOP
    - ⒉    2.    2489   9353   DIGIT TWO FULL STOP
    - ⒊    3.    248A   9354   DIGIT THREE FULL STOP
    - ㈠    1c    3220   12832  PARENTHESIZED IDEOGRAPH ONE
    - ㈡    2c    3221   12833  PARENTHESIZED IDEOGRAPH TWO
    - ㈢    3c    3222   12834  PARENTHESIZED IDEOGRAPH THREE

- 可以输入正确或错误

- - ✓    OK    2713   10003  CHECK MARK
    - ✗    XX    2717   10007  BALLOT X

- 可以使用 `:digraphs` 查看 `二合字符` 列表

![图片描述](https://i0.hdslb.com/bfs/article/ffec93ed18661f3a17f6b39cf8dce9e6793923cc.png@942w_698h_progressive.webp)

## 寄存器计算

- 在插入状态下
- 输入ctrl+r
- 输入 `=3+3`（注意要有`=`）
- 得到结果 6
- 可以计算小数吗？你自己试试！
- 帮助文件在 `h i_ctrl-r_=`(插入状态下，ctrl+r之后输入 `=`)

## 总结

- 通过十进制的 ascii 值输入字符

- - 在输入模式下
    - 输入ctrl+v
    - 然后再输入 065

- 通过十六进制的 unicode 值输入字符

- - 在输入模式下
    - 输入ctrl+v
    - 然后再输入 `u2642` 就可以通过 `unicode` 编码输入字符

- 通过二合字符的方式插入

- - 在输入模式下
    - 输入ctrl+k
    - 输入 Co 可以得到 ©
    - 输入 13 可以得到 ⅓
    - `:digraphs` 查看二合字符列表

- 寄存器计算

- - 在插入状态下
    - 输入ctrl+r
    - 输入 `=3+3`（注意要有 `=`）
    - 得到结果 6

- 我们掌握了在 vi 中插入字符的各种方法

- 如何 vim 可以删除字符吗？🤔

- 下次再说 *


## VS Code 编辑器教程-基础篇

![vscode00](./media/vscode/vscode_00.png)


> 本文主要介绍 vscode 在工作中常用的快捷键及插件，目标在于提高工作效率
>
> 本文的快捷键是基于 Mac 的，windows 下的快捷键放在括号里 Cmd+Shift+P(Win Ctrl+Shift+P)


### 一、零基础、快速入门

> 有经验的可以跳过E`快速入门`或者大致浏览一遍

#### 1. 命令面板

> 命令面板是 vscode 快捷键的主要交互界面，可以使用`f1`或者`Cmd+Shift+P`(win Ctrl+Shift+P) 打开。

在命令面板中你可以输入命令进行搜索 (中英文都可以)，然后执行。

命名面板中可以执行各种命令，包括编辑器自带的功能和`插件`提供的功能。

所以一定要记住它的快捷键`Cmd+Shift+P`

![vscode01](./media/vscode/vscode_01.jpeg)

#### 2. 界面介绍

> 刚上手使用 vscode 时，建议要先把它当做一个文件编辑器 (可以打字然后保存)，等到有了一定经验再去熟悉那些快捷键

先来熟悉一下界面及快捷命令 (不用记)

![vscode02](./media/vscode/vscode_02.png)


#### 3. 在命令行中使用 vscode

如果你是 Windows 用户，安装并`重启系统`后，你就可以在命令行中使用 `code` 或者 `code-insiders`了，如果你希望立刻而不是等待重启后使用，可以将 VS Code 的安装目录添加到系统环境变量 `PATH`中

如果你是 mac 用户，安装后打开命名面板`Cmd+Shift+P`, 搜索`shell`命令, 点击`在PAth中安装code命令`，然后重启终端就 ok 了

![vscode03](./media/vscode/vscode_03.jpeg)


最基础的使用就是使用 code 命令打开文件或文件夹

`code 文件夹地址`,vscode 就会在新窗口中打开该文件夹

如果你希望在已经打开的窗口打开文件，可以使用`-r`参数

![vscode04](./media/vscode/vscode_04.gif)

vscode 命令还有其他功能，比如文件比较，打开文件跳转到指定的行和列，如有需要自行百度: bowing_woman:

**注意：**

在继续看文章之前记住记住打开命令面板的快捷键`Cmd+shift+P`(win 下是 Ctrl+shift+p)

### 二、代码编辑

> windows 下的快捷键放在括号里

### 光标的移动

#### 基础

1.  移动到行首 Cmd + 左方向键 (win Home)
2.  移动到行尾 Cmd + 右方向键 (win End)
3.  移动到文档的开头和末尾 Cmd + 上下方向键 （win Ctrl+Home/End）
4.  在花括号 {} 左边右边之间跳转 Cmd+Shift+ (win Ctrl+Shift+)

#### 进阶

1.  回到上一个光标的位置，Cmd+U(win Ctrl+U) 非常有用，有时候 vue 文件，你改了 html，需要去下面改 js，改完 js 又需要回去，这时候 Cmd+U 直接回
2.  在不同的文件之间回到上一个光标的位置 Control+- (win 没测试，不知道)，你改了 a 文件，改了 b 文件之后想回到 a 文件继续编辑，mac 使用`controls+-`

#### 文本选择

1.  你只需要多按一个 shift 键就可以在光标移动的时候选中文本
2.  选中单词 `Cmd+D` 下面要讲的多光标也会讲到 Cmd+D
3.  对于代码块的选择没有快捷键，可以使用`cmd+shift+p`打开命令面板，输入`选择括号所有内容`, 待会说下如何添加快捷键

![vscode05](./media/vscode/vscode_05.gif)

#### 删除

1.  你可以选中了代码之后再删除，再按 Backpack(是 backpack 吗) 或者 delete 删除, 但是那样做太 low 了
2.  所以，最 Geek 的删除方式是`Cmd+Shift+K` `(win Ctrl+Shift+K)`, 想删多少删多少，当前你可以使用`ctrl+x`剪切，效果一样的

![vscode06](./media/vscode/vscode_06.gif)


#### 代码移动

*   Option + 上下方向键 (win Alt + 上下)

![vscode07](./media/vscode/vscode_07.gif)


*   代码移动的同时按住 shift 就可以实现代码复制 Option+Shift + 上下

![vscode08](./media/vscode/vscode_08.gif)

#### 添加注释

注释有两种形式，单行注释和块注释 (在 js 中，单行注释 //, 块注释 /**/)

*   单行注释 `Cmd+/` （win Ctrl +/）
*   块注释 `Option+Shift+A`

注意：不同语言使用的注释不同

### 三、代码格式

#### 代码格式化

*   对整个文档进行格式化：`Option+Shift+F` (win `Alt+Shift+F`),vscode 会根据你使用的语言，使用不同的插件进行格式化，记得要下载相应格式化的插件
*   对选中代码进行格式化： `Cmd+K Cmk+F` win(`Ctrl+K Ctrl+F`)

#### 代码缩进

*   真个文档进行缩进调节，使用 Cmd+Shift+P 打开命令面板，输入`缩进`, 然后选择相应的命令
*   选中代码缩进调节：Cmd+] Cmd+[分别是减小和增加缩进 (win 下不知道，自行百度)

### 四、一些小技巧

*   调整字符的大小写，选中，然后在命令面板输入`转化为大写`或者`转化为小写`
    ![vscode09](./media/vscode/vscode_09.gif)

*   合并代码行，多行代码合并为一行，`Cmd+J`(win 下未绑定)
    
    ![vscode10](./media/vscode/vscode_10.gif)

*   行排序，将代码行按照字母顺序进行排序，无快捷键，调出命令面板，输入`按升序排序`或者`按降序排序`

![vscode11](./media/vscode/vscode_11.gif)

### 五、多光标特性

#### 使用鼠标：

按住`Option`(win `Alt`), 然后用鼠标点，鼠标点在哪里哪里就会出现一个光标

注意：有的 mac 电脑上是按住`Cmd`，然后用鼠标点才可以

![vscode11](./media/vscode/vscode_12.gif)

#### 快捷命令

1.  `Cmd+D` (win `Ctrl+D`) 第一次按下时，它会选中光标附近的单词；第二次按下时，它会找到这个单词第二次出现的位置，创建一个新的光标，并且选中它。(注：`cmd-k cmd-d` 跳过当前的选择)

![vscode13](./media/vscode/vscode_13.gif)

2.  `Option+Shift+i` (win Alt+Shift+i) 首先你要选中多行代码，然后按`Option+Shift+i`, 这样做的结果是：每一行后面都会多出来一个光标
    
![vscode14](./media/vscode/vscode_14.gif)


#### 撤销多光标

*   使用`Esc`撤销多光标
*   鼠标点一下撤销

### 六、快速跳转 (文件、行、符号)

#### 快速打开文件

`Cmd+P` （win Ctrl+P）输入你要打开的文件名, 回车打开

![vscode15](./media/vscode/vscode_15.gif)

这里有个小技巧，选中你要打开的文件后，按`Cmd+Enter`, 就会在一个新的编辑器窗口打开 (窗口管理，见下文)

![vscode16](./media/vscode/vscode_16.gif)

在 tab 不同的文件间切换，cmd+shift+[]

#### 行跳转

加入浏览器报了个错，错误在 53 行，如何快速跳转到 53 行

`Ctrl+g` 输入行号

![vscode17](./media/vscode/vscode_17.gif)

如果你想跳转到某个文件的某一行，你只需要先按下 “Cmd + P”，输入文件名，然后在这之后加上 “:” 和指定行号即可。

![vscode18](./media/vscode/vscode_18.gif)

#### 符号跳转

> 符号可以是文件名、函数名，可以是 css 的类名

`Cmd+Shift+O`(win Ctrl+Shift+o) 输入你要跳转的符号，回车进行跳转

win 下输入`Ctrl+T`，可以在不同文件的符号间进行搜索跳转

![vscode19](./media/vscode/vscode_19.gif)

#### 定义 (definition) 和实现 (implementation) 处

`f12`跳到函数的定义处

`Cmd+f12`(win Ctrl+f12) 跳转到函数的实现处

![vscode20](./media/vscode/vscode_20.gif)

#### 引用跳转

很多时候，除了要知道一个函数或者类的定义和实现以外，你可能还希望知道它们被谁引用了，以及在哪里被引用了。这时你只需要将光标移动到函数或者类上面，然后按下 `Shift + F12`，VS Code 就会打开一个引用列表和一个内嵌的编辑器。在这个引用列表里，你选中某个引用，VS Code 就会把这个引用附近的代码展示在这个内嵌的编辑器里。

![vscode21](./media/vscode/vscode_21.gif)

### 七、代码重构

当我们想修改一个函数或者变量的名字时候，我们只需把光标放到函数或者变量名上，然后按下 `F2`，这样这个函数或者变量出现的地方就都会被修改。

![vscode22](./media/vscode/vscode_22.gif)

### 参考链接

1. 官方教程(英文)：https://code.visualstudio.com/docs/introvideos/basics
2. 宇宙最强 vscode 教程（基础篇）：https://segmentfault.com/a/1190000017949680
3. https://www.jianshu.com/p/11554732b323
4. https://www.cnblogs.com/love-snow/articles/8835153.html
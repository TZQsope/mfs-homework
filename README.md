"# mfs-homework" 
# Visual Studio Code常用功能说明
  ## 快捷键说明
  Visual Studio Code是个牛逼的编辑器，启动非常快，完全可以用来代替其他文本文件编辑工具。又可以用来做开发，支持各种语言，相比其他IDE，轻量级完全可配置还集成Git感觉非常的适合前端开发。 所以我仔细研究了一下文档未来可能会作为主力工具使用。
  ### 主命令框
  1. 最重要的功能就是F1或Ctrl+Shift+P打开的命令面板了，在这个命令框里可以执行VSCode的任何一条命令，甚至关闭这个编辑器。
  2. 按一下Backspace会进入到Ctrl+P模式里
  3. 在Ctrl+P下输入>又可以回到Ctrl+Shift+P模式
  
  4.在Ctrl+P窗口下还可以
  * 直接输入文件名，跳转到文件
  * ? 列出当前可执行的动作
  * ! 显示Errors或Warnings，也可以`Ctrl+Shift+M
  * : 跳转到行数，也可以Ctrl+G直接进入
  * @ 跳转到symbol（搜索变量或者函数），也可以Ctrl+Shift+O直接进入
  * @:根据分类跳转symbol，查找属性或函数，也可以Ctrl+Shift+O后输入:进入

  ### 常用快捷键
   #### 编辑器与窗口管理
  1.同时打开多个窗口（查看多个项目）
 * 打开一个新窗口： Ctrl+Shift+N
 * 关闭窗口： Ctrl+Shift+W

2.同时打开多个编辑器（查看多个文件）
* 新建文件 Ctrl+N
* 文件之间切换 Ctrl+Tab
* 切出一个新的编辑器（最多3个）Ctrl+\，也可以按住Ctrl鼠标点击Explorer里的文件名
* 左中右3个编辑器的快捷键Ctrl+1 Ctrl+2 Ctrl+3
* 3个编辑器之间循环切换 Ctrl+`
* 编辑器换位置，Ctrl+k然后按Left或Right

### 代码编辑
#### 格式调整

 * 代码行缩进Ctrl+[ Ctrl+]
 * Ctrl+C Ctrl+V如果不选中，默认复制或剪切一整行
 * 代码格式化：Shift+Alt+F，或Ctrl+Shift+P后输入format code
 * 上下移动一行： Alt+Up 或 Alt+Down
 * 向上向下复制一行： Shift+Alt+Up或Shift+Alt+Down
 * 在当前行下边插入一行Ctrl+Enter
 * 在当前行上方插入一行Ctrl+Shift+Enter

#### 光标相关

  *  移动到行首：Home
  * 移动到行尾：End
  * 移动到文件结尾：Ctrl+End
  * 移动到文件开头：Ctrl+Home
  * 移动到定义处：F12
  * 定义处缩略图：只看一眼而不跳转过去Alt+F12
  * 移动到后半个括号 Ctrl+Shift+]
  * 选择从光标到行尾Shift+End
  * 选择从行首到光标处Shift+Home
  * 删除光标右侧的所有字Ctrl+Delete
  * Shrink/expand selection： Shift+Alt+Left和Shift+Alt+Right
  * Multi-Cursor：可以连续选择多处，然后一起修改，Alt+Click添加cursor或者Ctrl+Alt+Down 或 Ctrl+Alt+Up
  * 同时选中所有匹配的Ctrl+Shift+L
  * Ctrl+D下一个匹配的也被选中(被我自定义成删除当前行了，见下边Ctrl+Shift+K)
  * 回退上一个光标操作Ctrl+U

#### 重构代码

  * 找到所有的引用：Shift+F12
  * 同时修改本文件中所有匹配的：Ctrl+F12
  * 重命名：比如要修改一个方法名，可以选中后按F2，输入新的名字，回车，会发现所有的文件都修改过了。
  * 跳转到下一个Error或Warning：当有多个错误时可以按F8逐个跳转
  * 查看diff 在explorer里选择文件右键 Set file to compare，然后需要对比的文件上右键选择Compare with 'file_name_you_chose'.

#### 查找替换

  *  查找 Ctrl+F
  *  查找替换 Ctrl+H
  *  整个文件夹中查找 Ctrl+Shift+F
  *  匹配符：
  *  *to match one or more characters in a path segment
  *  ? to match on one character in a path segment
  * ** to match any number of path segments ,including none
  *  {} to group conditions (e.g. {**/*.html,**/*.txt} matches all html and txt files)
  *  [] to declare a range of characters to match (e.g., example.[0-9] to match on example.0,example.1, …

#### 显示相关

  1.  全屏：F11
  2.  zoomIn/zoomOut：Ctrl + =/Ctrl + -
  3.  侧边栏显/隐：Ctrl+B
  4.  侧边栏4大功能显示：
       *      Show Explorer Ctrl+Shift+E
       *      Show SearchCtrl+Shift+F
       *      Show GitCtrl+Shift+G
       *      Show DebugCtrl+Shift+D
  5.  Show OutputCtrl+Shift+U

### 其他

    自动保存：File -> AutoSave ，或者Ctrl+Shift+P，输入 auto
    
##  插件安装与卸载
### 安装
 F1 输入 extensions
 
![插件](https://nshen.net/image/vscode/29945359.png)

 点击第一个开始安装或升级，或者也可以 Ctrl+P 输入 ext install进入
### 卸载
点击第二个会列出已经安装的扩展，可以从中卸载


##  在VSCode中使用Git
第一步，下载git安装包，安装完git后配置环境变量 “D:\git\Git\cmd”，win+R打开cmd输入命令git验证是否安装成功，在任意路径下能进入git，说明环境变量设置生效。

第二步，打开vscode, 文件->首选项->设置 打开用户设置，配置git路径，如下所示
![Git](https://img-blog.csdn.net/20180708202535419?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3p1b2ZhbnhpdQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70)

为了方便，可以把vscode的终端配置成git,同样的在用户设置文件里进行操作类似操作
![Git1](https://img-blog.csdn.net/20180708204821294?watermark/2/text/aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3p1b2ZhbnhpdQ==/font/5a6L5L2T/fontsize/400/fill/I0JBQkFCMA==/dissolve/70)

重启vscode可看见配置效果。。。

接下来，打开本地存储python项目的文件夹，初始化存储，之后，该目录下会生成一个.git文件

在bash终端（该终端下也可以切换路径）输入命令   

git init

然后再输入提交命令（提交也只是提交到本地而已并不是提交到github上，只有push才是将代码提交到github上）

git commit -m "first commit"

会提示输入用户名和邮箱，按照提示输入相应命令（用户名邮箱即你注册github所用的账户和邮箱）

接下来连接github,命令为：（testGit是我在github上创建的一个仓库）

git remote add origin https://github.com/zuofanxiu/testGit 

{如果出现错误提示： fatal: remote origin already exists. 

解决方案为：先删除远程仓库，再重新连接，删除命令为 git remote rm/remove origin  }

最后  git push -u origin master

此时会弹出一个登陆框让你填写github的账户密码

{如果出现错误提示： fatal: HttpRequestException encountered

解决方案为：  https://blog.csdn.net/zy20120580223/article/details/79618880  }

也可以考虑让git记住密码，这样不用每次都填写，执行命令为：

git config --global credential.helper store

当然，上面所有在bash终端执行的命令行操作都可以使用vscode的窗口操作，那样更简单。

# 谭紫倩的作业库
> 码蜂社 前端基础班 作业答题库
**码蜂社和谭紫倩版权所有，转载请注明出处**

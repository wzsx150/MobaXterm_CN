#### MobaXterm 综合远程工具 汉化版
MobaXterm 是一款功能强大的终端模拟器和远程管理工具，专为 Windows 用户设计。
它集成了多种网络工具，包括 SSH、X11 服务器、RDP、VNC、FTP 和 SFTP，提供了一个便捷的界面来管理远程服务器和本地文件。
MobaXterm 还支持多标签页操作，允许用户同时连接多个会话，并提供丰富的插件和自定义选项，使其成为开发人员和系统管理员的理想选择。

- 这里是 MobaXterm 便携版的汉化版，仅是做了汉化，无其他修改，无任何病毒、木马、后门。
- 本人仅是对软件进行汉化，不对软件的功能和使用负责，请合法使用该软件。
- 部分杀毒软件会报毒，请自行决定是否要使用。

类似工具：Xshell、SecureCRT、WindTerm等。个人推荐 MobaXterm ，网工、IT运维人员必备。


#### 已汉化内容
- MobaXterm.exe 便携版几乎所有界面显示的内容，比如：各种文本、按钮、选项、设置、提示内容、弹窗等。
- MobaXterm.exe 便携版的帮助文档、更新日志等；
- MobaXterm.exe 便携版微调“关于”窗口的文字显示布局；
- MobaKeyGennew.exe 和 MobaKeyGen.exe 内置的密钥证书生成工具的几乎所有界面显示的内容，比如：各种文本、按钮、选项、设置、提示内容、弹窗等；
- MobaRTE.exe 内置的文本编辑器(文件比较工具)的几乎所有界面显示的内容，比如：各种文本、按钮、选项、设置、提示内容、弹窗等；
- MoTTYnew.exe 和 MoTTY.exe 内置的终端的右键菜单、设置菜单、弹窗等；


#### 无法汉化的地方
- MobaXterm.exe 点击“检查更新”，如果有新版，弹出的有新版本的提示的窗口的字串。因为这些字串来自服务器。
- FTP/SFTP 等会话连接，在记录的日志有些内容是对方服务器返回的消息，这些内容无法汉化。
- MoTTYnew.exe 和 MoTTY.exe 内置的终端界面显示的字符，包括一些提示性的输出、报错输出等等。因为终端界面可以设置不同编码方式显示，如果按照GB2312编码翻译，那么当设置终端字体使用UTF-8编码时，则会乱码。反之亦然，所以不能完美兼容各种情况，只能不汉化。


#### 注意事项
- 本汉化版和官方原版不能共用配置文件，如果想保留会话书签，可以将会话导出后，再在汉化版中导入。强烈建议不要和官方或者其他人汉化的版本共用MobaXterm.ini配置文件！！！
- 已经尽可能的汉化所有能汉化的地方，难免会有遗漏的地方（欢迎反馈，如果确实是遗漏的字串，后续会更新汉化）。
- 有些地方的字串是无法汉化。例如：MobaXterm.exe 更新时的(有新版的)弹窗是从服务器获取到的字符串，所以无法汉化。
- 有些翻译不生效，或者有问题，有一个原因是 %s 和 %d 等字符，在字符串的前后顺序和位置不对。所以要严格遵照原文的 %字符 的顺序和个数进行翻译。
- MobaXterm.exe 和 MobaRTE.exe 是Delphi程序。
- MobaXterm.exe 便携版程序中，有一个EXEFILE的资源目录，该目录下存放了多个资源文件，基本都是使用LZMA压缩的zip包，其中 MOBASE 和 XW 还使用了加密混淆。
- MoTTYnew.exe 有一些字符是输出到终端行中的，这些内容受字体和字符编码的影响，所以这些内容强烈建议不翻译，翻译了会出现乱码的问题。（如果要翻译，也建议转换成UTF-8编码的字符串，这样只能兼容UTF-8编码的显示）
- MobaRTE.exe -compfolders 命令可以打开文件比较工具。
- MobaXterm.exe --customizer 命令可以打开MobaXterm定制器。


#### MobaXterm.exe 的 EXEFILE 下资源文件介绍：
可以使用 Resource Hacker 类似工具提取
- BASEPROF：lzma，shell的profile脚本。
- CHANGELOG：txt，存放的软件当前版本的更新日志。【汉化重点】
- CUSTGLYPHS：zip.lzma，存放软件界面上的显示的小部件的图片文件。
- FLICO16、FLICO22、FLICO32、FLICO48、FLICO64：zip.lzma，存放软件界面上的各类小图标的文件（一种风格）。
- HOTKEYS：lzma，快捷键的备选项。
- ICONSOLD：zip.lzma，存放软件界面上的各类小图标的文件（另一种风格）。
- IMGEXTS：zip.lzma，存放各类文件的图标文件。
- IMPINGUI：zip.lzma，存放企鹅屏保的图片文件。
- IMTHEMES：zip.lzma，存放暗色和亮色两种主题的示例图片。
- LI：zip.lzma，存放最终用户许可协议的各个协议文件。
- MOBAFANTA：字体
- MOBAFIRA：字体
- MOBAFONT：字体
- MOBASE：encrypted.zip.lzma，存放运行过程中调用一些程序，主要是 MobAgent.exe、MobAgentnew.exe、MobaKeyGen.exe、MobaKeyGennew.exe、MobaRTE.exe、MobaSCP.exe、MobaSCPnew.exe、MoTTY.exe、MoTTYnew.exe 等文件。【汉化重点】
- SEPARAMS：lzma，存放各种会话的设置界面的参数内容（比如各个控件显示的文本等），是用于会话设置项的粘贴界面的选项。【汉化重点】
- SKINS：zip.lzma，存放主题和皮肤文件。
- TXTRES：zip.lzma，存放生成帮助文档（HTML格式）的一些文本和图片文件。【汉化重点】
- XW：encrypted.zip.lzma，存放一些程序，主要是 XWin_MobaX.exe、XWin_MobaX_*.exe 等文件。


#### 反馈
可能存在没有汉化的界面和内容，请上传截图和简单复现的方法，提交问题，我将随缘更新。


#### 感谢
- 感谢 anysoft 大佬的汉化教程和汉化资源，带我入门，受益匪浅。
- 感谢 RipplePiam 大佬制作的汉化版，参考了他的很多翻译。
- 感谢 wanfu 大佬的指点和非标宏。


Windows 下让 Vim 支持默认以标签页(又称页签，tabs)打开多个文件，
节省任务栏和系统资源，并提高打开文件的性能。

参考链接中的方法都需要手工删除注册表中对应项，我把这项工作交给了
计算机，写在注册表文件(.reg)中。


功能：
支持两种打开方式：
1. 双击文件；
2. 右键文件 -> Edit with Vim （快捷键 V）
均可将目标文件在最后一个新窗口的标签页中打开。

其中
edit.with.vim.tabs.reg
将 Vim 每次开启新窗口的方式，改为在新标签页中打开。

edit.with.vim.window.reg
把在新标签页中打开文件的方式，
改为在 Vim 新窗口中打开（即 Vim 默认方式）。


用法：
1. 注册表中的路径均是按照默认的安装路径来设置，如果你的 Vim
    安装在不同的目录，请修改注册表文件中对应的路径；
2. 保存后双击注册表文件，或右键菜单 -> 合并 即可。


参考：
Vimfaq - Ubuntu 中文
    http://wiki.ubuntu.org.cn/index.php?title=Vimfaq&variant=zh-cn
vi/vim使用技巧: 在标签页中打开文件 (windows)
    http://easwy.com/blog/archives/vim-tips-windows-open-file-in-tab/
如何通过使用注册项 (.reg) 文件添加、修改或删除注册表子项和值
    http://support.microsoft.com/kb/310516/zh-cn

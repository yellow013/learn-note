命令提示软件:

yum install epel-release -y

yum install bash-completion -y


光标移动:

ctrl + a -> 光标移动到行首(速记:\<a\>bcd...)
  
ctrl + e -> 光标移动到行尾(速记:\<e\>nd)
  
ctrl + left & right -> 光标左(右)移一个词


字符操作:

ctrl + u -> 删除当前光标前面的字符

ctrl + k -> 删除当前光标后面的字符

ctrl + w -> 删除光标前的一个词(速记:\<w\>ard)
  
alt  + d -> 删除光标后的一个词(注意是'alt', 不是'ctrl', 'ctrl+d'为退出此终端)

ctrl + y -> 撤销本次删除

其他:

ctrl + r -> 根据关键字搜索历史命令

ctrl + z -> 当前shell进程转入后台, 输入'fg'命令恢复最后一个进入后台的进程, 输入'jobs'命令可以查看所有转入后台的进程, 输入'fg + ?'可恢复指定后台进程

ctrl + s -> 隐藏回显

ctrl + q -> 显示回显

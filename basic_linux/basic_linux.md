## Linux基础

- Linux
    - Linux Logo    
    ![](https://upload.wikimedia.org/wikipedia/commons/3/35/Tux.svg)
    - Linux系统诞生于1991年，由芬兰大学上[Linus Torvalds](https://baike.baidu.com/item/%E6%9E%97%E7%BA%B3%E6%96%AF%C2%B7%E6%9C%AC%E7%BA%B3%E7%AC%AC%E5%85%8B%E7%89%B9%C2%B7%E6%89%98%E7%93%A6%E5%85%B9/1034429?fromtitle=Linus%20Torvalds&fromid=9336769&fr=aladdin)和后来陆续加入的众多爱好者共同开发完成
    ![](https://upload.wikimedia.org/wikipedia/commons/thumb/0/01/LinuxCon_Europe_Linus_Torvalds_03_%28cropped%29.jpg/220px-LinuxCon_Europe_Linus_Torvalds_03_%28cropped%29.jpg)
    - Linux是一个在网络上发起并维护的操作系统，天生具有服务器属性
    - Linux是一个开源软件
    - Linux内核和发行版: 基于内核不同厂商加入自己的程序、桌面等形成了不同的发行版
    - [主要的发行版](https://distrowatch.com/dwres.php?resource=popularity)：redhat系: CentOS、fedora、gentoo等；debian系: ubuntu等；Arch Linux: **manjaro**

- 文件系统
    - 目录结构  
    ![](http://www.runoob.com/wp-content/uploads/2014/06/003vPl7Rty6E8kZRlAEdc690.jpg)
        > - / 根目录
        > - /bin 所有用户命令目录
        > - /boot 系统启动文件目录
        > - /dev 外部设备存放目录
        > - /etc 系统配置文件存放目录
        > - /home 用户目录，一个用户一个home目录
        > - /lib 系统基本动态链接库目录
        > - /lost+found 非法关机产生的文件存放目录
        > - /media 自动识别设备（U盘、光驱等）挂载目录
        > - /mnt 临时挂载目录
        > - /root root用户目录
        > - /usr 应用程序安装目录
        > - /usr/bin 系统用户命令存放目录
    - 文件属性
        `-rw-r--r-- 1 cabbet cabbet 824 3月   2 19:05 basic_linux.md`
        > - -rw-r--r--
        >    1) -文件类型(-:二进制文件; d:目录; l:软连接文件)
        >    2) rw- r-- r--(文件权限:所有者、所属组、其他人; r:读, w:写, x:执行)
        > - 1: 文件链接数
        > - cabbet cabbet: 创建者 所属组
        > - 824: 文件大小(ls -h)
        > - 3月   2 19:05: 文件修改时间
    - 与window文件的一些区别
        > - 后缀名没有特殊含义（一些约定俗称的后缀除外）
        > - 一些特殊的符号 * ? 等均可用于文件和目录名，只有 / 除外
        > - 没有盘符的概念，只有硬盘挂载点
        > - 隐藏文件: 以.开头的文件或文件夹
    - 路径相关:
        > - / 表示根目录
        > - ~ 表示 /home/CurrentUser
        > - ./ 表示当前目录
        > - .. 表示当前目录上层目录
- 常用命令：
    - 命令常见格式
        `command [-options] [params]`
        eg: `ls -a /doc`
        > - 当有多个选项时，可以合并: `ls -ah /doc`
        > - 简化option: -a 等于 -all
    - 包管理命令
        > - debian系: apt
        > - redhat系: yum
        > - arch系: pacman, yaourt
    - 帮助命令
        > - man, info, help, [tldr](https://github.com/tldr-pages/tldr) 帮助命令
    - 文件目录
        > - ls list命令
        > - mkdir 创建目录
        > - cd 切换目录
        > - pwd 当前目录
        > - cp 拷贝
        > - mv 移动文件或目录
        > - rm 删除文件或目录
        > - touch 创建文件
        > - cat, [bat](https://github.com/sharkdp/bat), tac, less, more, head, tial 文件内容查看
        > - ln 链接命令
        > - find, locate, [fzf](https://github.com/junegunn/fzf) 文件搜索
        > - which, whereis 搜索命令所在的目录
        > - grep, [ag](https://github.com/ggreer/the_silver_searcher) 搜索文件内容
        > - chown 更改文件所有者
    - 用户相关
        > - useradd, userdel 新增、删除用户
        > - passwd 更改密码
        > - who, w 查看用户
        > - last, lastlog 用户登录信息
    - 网络相关
        > - ip addr 查看网卡信息
        > - ping 
    - 系统相关
        > - shutdow, reboot, poweroff
- 常用第三方软件
    - [Vim](https://coolshell.cn/articles/5426.html)
    
    ![](http://www.runoob.com/wp-content/uploads/2015/10/vi-vim-cheat-sheet-sch.gif)
    - zsh & [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh)
    - [tmux](https://github.com/tmux/tmux)

- 学习资源推荐
    - [鸟哥Linux私房菜](http://cn.linux.vbird.org/)
    - [兄弟连LInux视频](https://www.bilibili.com/video/av18156598?from=search&seid=8675515860890405969)

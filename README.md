# daemons-and-service-one-sample

part I - target
    这个项目给了一个在mac上将可执行文件打包成后台程序的样例；
part II - usage
    双击demo/s-work即可生成安装包demo/work.pkg,并且运行demo/work.pkg,安装完成后可在Monitor上看到后台进程s-work正在运行;
    后台进程随系统启动而启动，即使进程崩溃也会被系统重启；若要关闭该进程，请利用launchctl命令卸载和删除服务；
    已在macOS Sierra 10.12.6 完成测试；
part III - resume
    demo/root/System/Library/LaunchDaemons/s-work.plist 服务程序配置文件
    demo/root/usr/local/bin/s-work  命令（服务实体程序）
    demo/s-work 打包脚本
    demo/script/preinstall  安装程序安装之前执行的脚本文件
    demo/script/postinstall 安装程序安装之后执行的脚本文件
    demo/work.pkg   运行打包脚本生成的安装包程序
part IV - reference
    man launchctl，launchd.plist,pkgbuild
    "About Daemons and Services"
    -https://developer.apple.com/library/content/documentation/MacOSX/Conceptual/BPSystemStartup/Chapters/Introduction.html

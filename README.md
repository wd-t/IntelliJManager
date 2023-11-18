# 命令列表

- `-v`(`-version`)
- 无参数,显示此程序的版本和toolbox版本
- `-l`(`-list`)
- 无参数,显示计算机上所有已安装的JetBrains IDE
- `-s`(`-script`)
- 复制启动脚本到指定位置
- `-ip`(`-idepath`)
- 参数为IDE所在目录,也就是bin的上级目录,需和 `-cp` 命令一起使用
- `-cp`(`-cachepath`)
- 参数为IDE缓存所在目录,需和 `-ip` 命令一起使用,如果配置文件有效,则IDE的config文件夹和plugins文件夹将按配置文件的路径来指定
  可通于其他IDE,但可能会有错误出现
- `-sf`(`-savefile`)
- 参数为一个任意后缀的文件名,放在用户文件夹下.config/intellijmanager文件夹里,在与`-ip -cp`命令连用时可以保存配置配置到文件
  单独时使用时读取文件并和`-ip -cp`命令一样,不用重复指定路径,同样配置文件有效则使用配置文件里所指定的来
- `-c`(`-config`)
- 无参数,以toString()的方式打印配置文件，里面有统一的IDE配置缓存地址和插件地址
- `-o`(`-open`)
- 无参数,跟`-c`连用,打开配置文件
- `-nc`(`-notconfig`)
- 可跟`-sf -cp`连用,意为不用配置文件里所指定的路径配置
- `-i`(`install`)
- 修改toolbox里工具安装位置

##### 注意本程序比较依赖JetBrains Toolbox 2.0,使用前需安装
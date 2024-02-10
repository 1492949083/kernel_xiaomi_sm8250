## 项目简介
- LXC+KernelSU的K30Pro Android14内核源码
- 本内核仅在crdroid_10.1 Android14上测试过，其他版本未测试
- 我使用的Toolchain 来自 [这个链接](https://www.coolapk.com/feed/50019057?shareKey=N2UwZTA2MDhkNDcyNjVjNzllY2U~&shareUid=1302037&shareFrom=com.coolapk.market_14.0.1) 中的Docker镜像里.
- 由于我不懂一点C语言，所以这个项目别人编译起来可能会有些问题,比如 `make clean && make mrproper` 会清理掉`drivers/input/touchscreen`目录下的某些文件，导致编译失败，所以建议编译前先备份一下`drivers/input/touchscreen`目录下的文件


### AI立大功
- 90%的bug由AI修复,这个README.md也有一半是AI写的.
- 如果你提交了一个issue，也许AI会帮你修复...

### bug
- 有的时候wifi不会自动连接，需要重新开wifi.
- Docker 的 Bridge模式下容器无法访问外网,DNS超时,改用Host模式即可解决

##### 免责声明：
- 不太懂这些,说的不对请指正.
- 如果你的设备变砖了，我不负任何责任
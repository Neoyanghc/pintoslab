# 在QEMU虚拟机中安装pintos

1. 下载pintos源码

   ```shell
   git clone http://cs140.stanford.edu/pintos.git
   ```

2. 编译安装

   ```shell
   cd ~/pintos/src/threads
   make
   ../utils/pintos -- run alarm-multiple
   ```

3. 出现下面的截图就行了

   <img src="https://ws1.sinaimg.cn/large/006tKfTcly1g1oixm9uosj30zo0fyq9y.jpg" width="500">

   


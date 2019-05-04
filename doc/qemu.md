# QEMU虚拟安装

1. 下载源码

   ```shell
   git clone https://git.qemu.org/git/qemu.git
   cd qemu
   git checkout v2.10.0 # 使用2.10.0版本
   ```

2. 安装依赖库

   ```shell
   sudo apt-get install libsdl2-dev libsdl2-gfx-dev libsdl2-image-dev libsdl2-mixer-dev  libsdl2-net-dev libsdl2-ttf-dev
   ```

   ```shell
   sudo apt-get install build-essential flex bison cmake automake libtool gcc-multilib g++-multilib libpixman-dev libfdt-dev
   ```

3. 编译安装i386版本虚拟机

   ```shell
   mkdir build
   cd build
   ../configure --prefix=/usr/local/src/qemu --target-list="i386-softmmu" --enable-debug --python=/usr/bin/python2
   make
   sudo make install
   ```

4. 添加软连接

   ```shell
   cd /usr/local/src/qemu/bin/
   sudo ln -s qemu-system-i386 qemu 
   ```

   
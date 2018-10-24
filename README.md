Procedure


1. Get 64Bit Cross Compiler by
sudo apt-get install gcc-aarch64-linux-gnu g++-aarch64-linux-gnu


2. Build according to bcmrpi3_defconfig (Raspberry Pi 3B+)
make -j4 ARCH=arm64 KERNEL=kernel7 CROSS_COMPILE=aarch64-linux-gnu- bcmrpi3_defconfig

3. Do Modification of Kernel through menuconfig
make -j4 ARCH=arm64 KERNEL=kernel7 CROSS_COMPILE=aarch64-linux-gnu- menuconfig


4. Make Kernel
make -j4 ARCH=arm64 KERNEL=kernel7 CROSS_COMPILE=aarch64-linux-gnu-

5. Make Module files for this Kernel
make -j4 ARCH=arm64 KERNEL=kernel7 CROSS_COMPILE=aarch64-linux-gnu- modules

Reference (In Traditional Chinese Only)
https://blog.gtwang.org/iot/raspberry-pi-compile-linux-kernel/



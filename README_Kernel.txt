HOW TO BUILD KERNEL 3.0.3 ICS FOR U1(I9100)

1. How to Build
	- Get Toolchain (arm-eabi-4.4.3)

	- edit Makefile
		edit "CROSS_COMPILE" to right toolchain path(You downloaded).
		  EX)  CROSS_COMPILE= $(android platform directory you download)/android/prebuilt/linux-x86/toolchain/arm-eabi-4.4.3/bin/arm-eabi-
                  Ex)  CROSS_COMPILE=/usr/local/toolchain/arm-eabi-4.4.3/bin/arm-eabi-          // check the location of toolchain

	-	Extract kernel source
	$ make ARCH=arm u1_defconfig
	$ make
	
2. Output files
	- Kernel : /arch/arm/boot/zImage
	
3. build clean
	- make clean
	




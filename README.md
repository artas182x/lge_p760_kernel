Kernel Build
  - Clone git repo: git clone -u https://github.com/artas182x/lge_p760_kernel.git -b v20b
	
  - change directory to kernel root
	cd kernel_directory (default: lge_p760_kernel)

  - make configuration:
	make u2_p760_defconfig ARCH=arm
	
  - make kernel zImage:
	make ARCH=arm CROSS_COMPILE=../prebuilt/linux-x86/toolchain/arm-eabi-4.4.3/bin/arm-eabi- zImage

../prebuilt/linux-x86/toolchain/arm-eabi-4.4.3/bin/ is patch for arm toolchain (you must download it before)!

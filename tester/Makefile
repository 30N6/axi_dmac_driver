SYSROOT         = ../../../../../buildroot/output/staging
PKG_CONFIG_PATH = ${SYSROOT}/usr/lib/pkgconfig
CC              = arm-linux-gnueabihf-gcc
CFLAGS          += --sysroot=${SYSROOT} -std=gnu99 -Wall -Wextra -g -mfloat-abi=hard
LIBS            += -lpthread -liio -lm --sysroot=${SYSROOT} 

export PATH			:= /home/${USER}/gcc-linaro-7.3.1-2018.05-x86_64_arm-linux-gnueabihf/bin:${PATH}

axi_dmac_tester: axi_dmac_tester.o
	$(CC) $(LIBS) $(CFLAGS) -o axi_dmac_tester axi_dmac_tester.o


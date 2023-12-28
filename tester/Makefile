SYSROOT         = ../../../../../buildroot/output/staging
PKG_CONFIG_PATH = ${SYSROOT}/usr/lib/pkgconfig
CC              = arm-linux-gnueabihf-gcc
CFLAGS          += --sysroot=${SYSROOT} -std=gnu99 -Wall -Wextra -g
LIBS            += -lpthread -liio -lm --sysroot=${SYSROOT} 


axi_dmac_tester: axi_dmac_tester.o
	$(CC) $(LIBS) $(CFLAGS) -o axi_dmac_tester axi_dmac_tester.o

#arm-linux-gnueabihf-gcc -mfloat-abi=hard  --sysroot=../../../../../buildroot/output/staging -std=gnu99 -g -o axi_dmac_tester axi_dmac_tester.c -lpthread -liio -lm -Wall -Wextra
#arm-linux-gnueabihf-gcc --sysroot=../../../../../buildroot/output/staging -std=gnu99 -g -o axi_dmac_tester axi_dmac_tester.c -lpthread -liio -lm -Wall -Wextra

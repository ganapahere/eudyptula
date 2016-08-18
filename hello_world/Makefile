obj-m := hello_world.o
KERNELDIR ?= /lib/modules/$(shell uname -r)/build
PWD  := $(shell pwd)
default:
	$(MAKE) -C $(KERNELDIR) M=$(PWD) modules

clean:
	$(RM) .*.cmd *.o *.ko *.mod.c *.order *.symvers -r .tmp*

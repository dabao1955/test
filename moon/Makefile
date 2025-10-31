ifneq ($(KERNELRELEASE),)
obj-m += main.o
else
KDIR :=/home/user/test
PWD  :=$(shell pwd)
all:
	make -C $(KDIR) M=$(PWD) modules
clean:
	rm -f *.ko *.o *.mod.o *.symvers *.cmd  *.mod.c *.order
endif

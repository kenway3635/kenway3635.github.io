KERNEL_VERSION  := $(shell uname -r)
KERNEL_MODULES  := /usr/src/linux-headers-$(KERNEL_VERSION)
cc=gcc

obj-m += hello_world.o

all:
	$(MAKE) -C $(KERNEL_MODULES) M=$(shell pwd) modules

clean:
	$(MAKE) -C $(KERNEL_MODULES) M=$(shell pwd) clean
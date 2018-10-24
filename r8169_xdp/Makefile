#
# Makefile for the Realtek network device drivers.
#
 
#KERN_DIR = /usr/src/$(shell uname -r)
KERN_DIR = /lib/modules/$(shell uname -r)/build
 
all:
	make -C $(KERN_DIR) M=$(shell pwd) modules   
 
clean:                                  
	rm -rf modules.order *.o *.ko *.symvers .r8169* .tmp* .cach* *.mod.c
 
obj-m += r8169.o


obj-m := kvaser_usb.o
kvaser_usb-m := kvaser_usb_core.o kvaser_usb_hydra.o kvaser_usb_leaf.o

all:
	make -C /lib/modules/$(shell uname -r)/build M=$(shell pwd) modules

install:
	make -C /lib/modules/$(shell uname -r)/build M=$(shell pwd) modules_install

clean:
	make -C /lib/modules/$(shell uname -r)/build M=$(shell pwd) clean

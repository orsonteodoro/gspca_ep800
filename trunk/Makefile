obj-m = ep800.o
KVERSION = $(shell uname -r)
EXTRA_CFLAGS=-I/lib/modules/$(KVERSION)/build/drivers/media/usb/gspca
all:
	make -C /lib/modules/$(KVERSION)/build M=$(PWD) modules
clean:
	make -C /lib/modules/$(KVERSION)/build M=$(PWD) clean

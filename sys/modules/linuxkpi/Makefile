# $FreeBSD$
.PATH:	${.CURDIR}/../../compat/linuxkpi/common/src

KMOD=	linuxkpi
SRCS=	linux_kmod.c \
	linux_compat.c \
	linux_current.c \
	linux_kthread.c \
	linux_pci.c \
	linux_radix.c \
	linux_rcu.c \
	linux_tasklet.c \
	linux_idr.c \
	linux_usb.c

SRCS+=	bus_if.h \
	device_if.h \
	pci_if.h \
	vnode_if.h \
	usb_if.h \
	opt_usb.h

CFLAGS+= -I${.CURDIR}/../../compat/linuxkpi/common/include
CFLAGS+= -I${.CURDIR}/../../contrib/ck/include

.include <bsd.kmod.mk>

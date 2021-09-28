#	$OpenBSD: Makefile,v 1.2 2021/07/26 09:26:36 florian Exp $

PROG =	devd
SRCS =	devd.cc parse.y token.l

MAN =	devd.8 devd.conf.5

CPPFLAGS += -I${.CURDIR} -I.

CPPFLAGS += -Wno-missing-variable-declarations

CLEANFILES = y.code.c y.tab.d y.tab.o

LDADD += -levent -lutil

.include <bsd.prog.mk>

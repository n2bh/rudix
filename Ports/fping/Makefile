include ../../Library/GNU.mk

Title=		Fping
Name=		fping
Version=	3.10
Revision=	0
Site=           http://fping.org
URL=		http://fping.org/dist
Source=		$(Name)-$(Version).tar.gz
License=        BSD?

GnuConfigureExtra += --sbindir=$(BinDir)
GnuConfigureExtra += --enable-ipv4 --enable-ipv6

define test_inner_hook
$(BinDir)/fping -v | grep $(Version)
$(BinDir)/fping6 -v | grep $(Version)
endef

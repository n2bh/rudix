include ../../Library/GNU.mk

Title=		Apache Portable Runtime Utility
Name=		apr-util
Version=	1.5.1
Revision=	0
Site=		http://apr.apache.org/
URL=		http://www.apache.org/dist/apr/
Source=		$(Name)-$(Version).tar.bz2
License=	Apache License

LicenseFile=	$(BuildDir)/LICENSE

GnuConfigureExtra += --with-apr=/usr/bin/apr-1-config

define test_inner_hook
$(BinDir)/apu-1-config --version
endef

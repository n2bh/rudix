BuildRequires += $(LibDir)/libmemcached.la # libmemcached
Requires += org.rudix.pkg.libmemcached,libmemcached,libmemcachedinstall.pkg

include ../../Library/Python.mk

Title=		pylibmc
Name=		pylibmc
Version=	1.2.3
Revision=	2
Site=		http://pypi.python.org/pypi/pylibmc
URL=		http://pypi.python.org/packages/source/p/pylibmc/
Source=		$(Name)-$(Version).tar.gz
License=	Python License

ReadMeFile=	$(SourceDir)/README.rst
LicenseFile=	$(SourceDir)/LICENSE

define test_inner_hook
$(Python) -c 'import pylibmc'
endef

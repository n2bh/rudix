include ../../Library/Python.mk

Title=		Python Nose
Name=		python-nose
Version=	1.3.1
Revision=	0
Site=           https://github.com/nose-devs/nose
URL=		https://pypi.python.org/packages/source/n/nose/
Source=		nose-$(Version).tar.gz
License=        LGPL

ReadMeFile=	$(SourceDir)/README.txt
LicenseFile=	$(SourceDir)/lgpl.txt

UncompressedName=nose-$(Version)

define test_inner_hook
$(Python) -c 'import nose'
$(BinDir)/nosetests --version | grep $(Version)
endef

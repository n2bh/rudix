BuildRequires += $(BinDir)/fltk-config  # fltk

include ../../Library/GNU.mk

Title=		HTMLDOC
Name=		htmldoc
Version=	1.8.28
Revision=	0
#URL=		http://ftp.easysw.com/pub/htmldoc/$(Version)/
Site=		http://www.htmldoc.org/
URL=		http://www.msweet.org/files/project1/
Source=		$(Name)-$(Version)-source.tar.bz2
License=	GPL

ReadMeFile=	$(SourceDir)/README.txt
LicenseFile=	$(SourceDir)/COPYING.txt

MakeInstallExtra += prefix=$(DestDir)$(Prefix)
MakeInstallExtra += bindir=$(DestDir)$(BinDir)
MakeInstallExtra += mandir=$(DestDir)$(ManDir)
MakeInstallExtra += datadir=$(DestDir)$(DataDir)

define test_inner_hook
$(BinDir)/htmldoc --version | grep $(Version)
endef

define install_post_hook
install -m 755 $(BuildDir)/htmldoc/htmldoc.app/Contents/MacOS/htmldoc \
	$(DestDir)$(BinDir)/htmldoc
endef

define test_inner_hook
$(BinDir)/htmldoc --version | grep $(Version)
endef

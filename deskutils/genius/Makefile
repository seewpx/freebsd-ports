# Created by: Andrey Zakhvatov
# $FreeBSD$

PORTNAME=	genius
PORTVERSION=	1.0.25
CATEGORIES=	deskutils gnome
MASTER_SITES=	GNOME \
		http://ftp.5z.com/pub/genius/

MAINTAINER=	woodsb02@FreeBSD.org
COMMENT=	Arbitrary precision calculator for Gnome Desktop Environment

LICENSE=	GPLv3
LICENSE_FILE=	${WRKSRC}/COPYING

BUILD_DEPENDS=	rarian-sk-config:textproc/rarian
LIB_DEPENDS=	libamtk-5.so:x11-toolkits/amtk \
		libfontconfig.so:x11-fonts/fontconfig \
		libfreetype.so:print/freetype2 \
		libgmp.so:math/gmp \
		libmpfr.so:math/mpfr
RUN_DEPENDS=	rarian-sk-config:textproc/rarian

USES=		desktop-file-utils gmake gnome libtool pathfix pkgconfig \
		readline shared-mime-info tar:xz xorg
USE_GNOME=	cairo gnomeprefix gtksourceview4 vte3 intltool
USE_XORG=	x11 xext
GNU_CONFIGURE=	yes
CONFIGURE_ARGS=	--disable-extra-gcc-optimization \
		--disable-update-mimedb \
		--disable-scrollkeeper
INSTALL_TARGET=	install-strip
USE_LDCONFIG=	yes
INSTALLS_ICONS=	yes
INSTALLS_OMF=	yes

OPTIONS_DEFINE=		NLS
OPTIONS_SUB=		yes

NLS_USES=		gettext
NLS_CONFIGURE_ENABLE=	nls

CPPFLAGS+=	-I${LOCALBASE}/include
LDFLAGS+=	-L${LOCALBASE}/lib

.include <bsd.port.mk>

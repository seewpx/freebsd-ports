# Created by: ijliao
# $FreeBSD$

PORTNAME=	Gnome2-Canvas
PORTVERSION=	1.006
CATEGORIES=	x11-toolkits gnome perl5
MASTER_SITES=	CPAN/Gnome2 \
		SF/gtk2-perl/Gnome2_Canvas/${PORTVERSION}
PKGNAMEPREFIX=	p5-

MAINTAINER=	bofh@FreeBSD.org
COMMENT=	Allows a perl developer to use the GnomeCanvas widget with Gtk2-Perl

LICENSE=	GPLv2

BUILD_DEPENDS=	p5-ExtUtils-Depends>=0:devel/p5-ExtUtils-Depends \
		p5-ExtUtils-PkgConfig>=0:devel/p5-ExtUtils-PkgConfig \
		p5-Glib>=0:devel/p5-Glib \
		p5-Gtk2>=0:x11-toolkits/p5-Gtk2 \
		p5-Cairo>=0:graphics/p5-Cairo
RUN_DEPENDS=	p5-Glib>=0:devel/p5-Glib \
		p5-Gtk2>=0:x11-toolkits/p5-Gtk2

USES=		gnome perl5 pkgconfig
USE_GNOME=	libgnomecanvas
USE_PERL5=	configure

MAKE_JOBS_UNSAFE=	yes

.include <bsd.port.mk>

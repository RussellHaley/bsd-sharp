# Created by: Tom McLaughlin <tmclaugh@sdf.lonestar.org>
# $FreeBSD: head/x11-toolkits/libgdiplus/Makefile 412351 2016-04-01 14:33:55Z mat $

PORTNAME=	libgdiplus
PORTVERSION=	4.2
CATEGORIES=	x11-toolkits
MASTER_SITES=	http://download.mono-project.com/sources/${PORTNAME}/

MAINTAINER=	mono@FreeBSD.org
COMMENT=	GDI+ API for System.Windows.Forms in Mono

LIB_DEPENDS=	libtiff.so:graphics/tiff \
		libgif.so:graphics/giflib \
		libpng.so:graphics/png \
		libcairo.so:graphics/cairo

GNU_CONFIGURE=	yes
USES=		cpe gmake libtool:keepla pathfix pkgconfig
USE_GNOME=	glib20
USE_LDCONFIG=	yes
USE_XORG=	x11
CPPFLAGS+=	-I${LOCALBASE}/include
LDFLAGS+=	-L${LOCALBASE}/lib
INSTALL_TARGET=	install-strip
CPE_VENDOR=	mono-project

PLIST_FILES=	lib/libgdiplus.a \
		lib/libgdiplus.la \
		lib/libgdiplus.so \
		lib/libgdiplus.so.0 \
		lib/libgdiplus.so.0.0.0 \
		libdata/pkgconfig/libgdiplus.pc

.include <bsd.port.mk>

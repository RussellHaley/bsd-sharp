# New ports collection makefile for:	mono-addins
# Date created:				Aug 25 2008
# Whom:					Florent Thoumie <flz@FreeBSD.org>
#
# $FreeBSD: ports/devel/mono-addins/Makefile,v 1.3 2008/08/28 19:35:40 flz Exp $
#

PORTNAME=	mono-addins
PORTVERSION=	0.4
CATEGORIES=	devel
MASTER_SITES=	http://ftp.novell.com/pub/mono/sources/${PORTNAME}/

MAINTAINER=	flz@FreeBSD.org
COMMENT=	Mono framework to create extensible applications

LIB_PC_DEPENDS=	${LOCALBASE}/libdata/pkgconfig/mono.pc:${PORTSDIR}/lang/mono

BUILD_DEPENDS+=	${LIB_PC_DEPENDS}
RUN_DEPENDS+=	${LIB_PC_DEPENDS}

USE_BZIP2=	yes
GNU_CONFIGURE=	yes
USE_GMAKE=	yes
USE_GNOME=	gnomehack pkgconfig

OPTIONS=	GTK2 "Enable GTK support" on

MAN1=		mautil.1

.include <bsd.port.pre.mk>
.include "${.CURDIR}/../../lang/mono/bsd.mono.mk"

.if !defined(WITHOUT_GTK2) && !defined(WITHOUT_GUI) && !defined(WITHOUT_X11)
USE_GNOME+=	gtksharp20
CONFIGURE_ARGS+=	--enable-gui
PLIST_SUB=	OPT_GTK2=""
.else
CONFIGURE_ARGS+=	--disable-gui
PLIST_SUB=	OPT_GTK2="@comment "
.endif

.include <bsd.port.post.mk>
# Created by: Romain Tartiere <romain@blogreen.org>
# $FreeBSD: head/irc/smartirc4net/Makefile 387196 2015-05-23 23:59:42Z antoine $

PORTNAME=	smartirc4net
PORTVERSION=	1.0
CATEGORIES=	irc
MASTER_SITES=	https://smuxi.im/jaws/data/files/

MAINTAINER=	mono@FreeBSD.org
COMMENT=	Multi-layered IRC library

GNU_CONFIGURE=	yes
CONFIGURE_ENV=	ac_cv_path_MCS=${LOCALBASE}/bin/mcs
USES=		gmake mono pathfix pkgconfig

.include <bsd.port.mk>

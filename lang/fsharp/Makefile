# Created by: Phillip Neumann <pneumann@gmail.com>
# $FreeBSD: head/lang/fsharp/Makefile 412347 2016-04-01 14:08:37Z mat $

PORTNAME=	fsharp
PORTVERSION=	4.0.1.1
CATEGORIES=	lang

MAINTAINER=	mono@FreeBSD.org
COMMENT=	Functional and object-oriented language for the .NET platform

LICENSE=	APACHE20

BUILD_DEPENDS=	mono>=3.0:lang/mono
RUN_DEPENDS=	mono>=3.0:lang/mono

USE_GITHUB=	yes

USES=		autoreconf gmake mono pkgconfig
GNU_CONFIGURE=	yes

.include <bsd.port.mk>

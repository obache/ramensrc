# $NetBSD: Makefile,v 1.37 2021/04/29 23:30:13 thor Exp $

DISTNAME=	speex-1.2.0
PKGREVISION=	1
CATEGORIES=	audio
MASTER_SITES=	http://downloads.us.xiph.org/releases/speex/

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://www.speex.org/
COMMENT=	Open-source, patent-free voice codec
LICENSE=	modified-bsd

USE_LIBTOOL=		YES
GNU_CONFIGURE=		YES
PKGCONFIG_OVERRIDE=	speex.pc.in
USE_TOOLS+=		pkg-config

# previous versions of the package were called Speex
CONFLICTS=	Speex-[0-9]*

BUILDLINK_TRANSFORM+=	l:gnugetopt:getopt

.include "options.mk"

.include "../../devel/libgetopt/buildlink3.mk"
.include "../../multimedia/libogg/buildlink3.mk"

.include "../../mk/oss.buildlink3.mk"
.include "../../mk/bsd.pkg.mk"

# $NetBSD: Makefile,v 1.22 2020/08/17 20:17:54 leot Exp $

DISTNAME=	libXft-2.3.3
PKGREVISION=	1
CATEGORIES=	fonts x11
MASTER_SITES=	${MASTER_SITE_XORG:=lib/}
EXTRACT_SUFX=	.tar.bz2

MAINTAINER=	joerg@NetBSD.org
HOMEPAGE=	https://www.freedesktop.org/wiki/Software/Xft/
COMMENT=	Library for configuring and customizing font access

CONFLICTS+=	Xft2-[0-9]*

GNU_CONFIGURE=		YES
USE_LIBTOOL=		YES
USE_TOOLS+=		pkg-config
PKGCONFIG_OVERRIDE=	xft.pc.in

.include "../../devel/zlib/buildlink3.mk"
BUILDLINK_API_DEPENDS.fontconfig+=	fontconfig>=2.6
.include "../../fonts/fontconfig/buildlink3.mk"
.include "../../graphics/freetype2/buildlink3.mk"
.include "../../x11/libXrender/buildlink3.mk"
.include "../../x11/libX11/buildlink3.mk"
.include "../../x11/xorgproto/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"

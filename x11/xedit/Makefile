# $NetBSD: Makefile,v 1.4 2020/01/18 23:36:00 rillig Exp $

DISTNAME=	xedit-1.2.2
CATEGORIES=	editors x11
MASTER_SITES=	${MASTER_SITE_XORG:=app/}
EXTRACT_SUFX=	.tar.bz2

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://xorg.freedesktop.org/
COMMENT=	Simple text editor for X
#LICENSE=	modified-bsd AND x11 # XXX AND others

GNU_CONFIGURE=	yes
USE_TOOLS+=	pkg-config

MAKE_FLAGS+=	appdefaultdir=${PREFIX}/lib/X11/app-defaults

.include "../../x11/libXt/buildlink3.mk"
.include "../../x11/libXmu/buildlink3.mk"
.include "../../x11/libXaw/buildlink3.mk"
.include "../../x11/libX11/buildlink3.mk"
.include "../../devel/xorg-util-macros/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"

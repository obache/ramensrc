# $NetBSD: Makefile,v 1.16 2020/12/04 20:45:42 nia Exp $

PKGNAME=	${DISTNAME:S/^M/m/}
PKGREVISION=	2
DISTNAME=	Manifold-0.2.0
CATEGORIES=	sysutils
MASTER_SITES=	${MASTER_SITE_PYPI:=M/Manifold/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	https://pypi.python.org/pypi/Manifold
COMMENT=	SMF service manifest creation tool
LICENSE=	mit

DEPENDS+=	${PYPKGPREFIX}-genshi-[0-9]*:../../www/py-genshi

USE_LANGUAGES=	# none

PYTHON_VERSIONS_ACCEPTED=	27 # not yet ported as of 0.2.0

post-extract:
	${CHMOD} -R g-w ${WRKSRC}/*

.include "../../lang/python/distutils.mk"
.include "../../mk/bsd.pkg.mk"

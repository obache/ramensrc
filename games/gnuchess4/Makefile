# $NetBSD: Makefile,v 1.17 2020/01/18 23:32:01 rillig Exp $

DISTNAME=		gnuchess-4.0.pl80
PKGNAME=		gnuchess4-4.0.80
CATEGORIES=		games
MASTER_SITES=		${MASTER_SITE_LOCAL}

MAINTAINER=		pkgsrc-users@NetBSD.org
HOMEPAGE=		https://www.gnu.org/software/chess/chess.html
COMMENT=		The "classic" GNU chess

MAKE_JOBS_SAFE=		no

CONFLICTS=		gnuchess-4.*

GNU_CONFIGURE=		yes
CONFIGURE_DIRS=		src
BUILD_DIRS=		${CONFIGURE_DIRS}

INSTALLATION_DIRS=	bin ${PKGMANDIR}/man6 share/doc/gnuchess4

post-install:
	cd ${WRKSRC}/doc; ${INSTALL_DATA} \
		ARTICLE ARTICLE.2 CHESSTOOL FAQ HEURISTICS MOVE-GEN \
		README.font README.output \
		${DESTDIR}${PREFIX}/share/doc/gnuchess4

.include "../../mk/bsd.pkg.mk"

# $NetBSD: Makefile,v 1.26 2021/05/24 19:50:49 wiz Exp $

DISTNAME=	Hash-Case-1.05
PKGNAME=	p5-${DISTNAME}0
PKGREVISION=	2
CATEGORIES=	devel perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=Hash/}

MAINTAINER=	pkgsrc-users@NetBSD.org
#HOMEPAGE=	http://perl.overmeer.net/perlws2003-hash/0-0/
HOMEPAGE=	https://metacpan.org/release/Hash-Case
COMMENT=	Perl module that implements case-insensitive hashes
LICENSE=	${PERL5_LICENSE}

DEPENDS+=	p5-Log-Report>=0.26:../../devel/p5-Log-Report

PERL5_PACKLIST=		auto/Hash/Case/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"

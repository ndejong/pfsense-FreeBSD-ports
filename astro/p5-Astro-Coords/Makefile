# Created by: Sunpoet Po-Chuan Hsieh <sunpoet@FreeBSD.org>
# $FreeBSD$

PORTNAME=	Astro-Coords
PORTVERSION=	0.19
CATEGORIES=	astro perl5
MASTER_SITES=	CPAN
PKGNAMEPREFIX=	p5-

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Class for handling astronomical coordinates

LICENSE=	GPLv2+

BUILD_DEPENDS=	p5-Astro-PAL>=0:astro/p5-Astro-PAL \
		p5-Astro-Telescope>=0.71:astro/p5-Astro-Telescope \
		p5-DateTime>=0.76:devel/p5-DateTime
RUN_DEPENDS:=	${BUILD_DEPENDS}
TEST_DEPENDS=	p5-Test-Number-Delta>=0:devel/p5-Test-Number-Delta \
		p5-Test-Pod>=1:devel/p5-Test-Pod

NO_ARCH=	yes
USE_PERL5=	modbuild
USES=		perl5

.include <bsd.port.mk>

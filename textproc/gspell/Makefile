# Created by: Olivier Duchateau
# $FreeBSD$

PORTNAME=	gspell
PORTVERSION=	1.4.1
CATEGORIES=	textproc
MASTER_SITES=	GNOME
DIST_SUBDIR=	gnome3

MAINTAINER=	gnome@FreeBSD.org
COMMENT=	Spell checking for GTK+

LICENSE=	GPLv2

BUILD_DEPENDS=	valac:lang/vala \
		iso-codes>=3.57:misc/iso-codes
LIB_DEPENDS=	libenchant.so:textproc/enchant

USES=		gmake iconv libtool pathfix pkgconfig tar:xz
USE_GNOME=	atk cairo gdkpixbuf2 glib20 gtk30 introspection:build \
		libxml2 pango
GNU_CONFIGURE=	yes
USE_LDCONFIG=	yes
INSTALL_TARGET=	install-strip

CONFIGURE_ARGS=	--with-pkgconfigdir=${PREFIX}/libdata/pkgconfig

OPTIONS_DEFINE=	NLS
NLS_USES=	gettext-tools
NLS_CONFIGURE_ENABLE=	nls
OPTIONS_SUB=	yes

.include <bsd.port.mk>

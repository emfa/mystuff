COMMENT=	real-time, concurrent and distributed functional language

CATEGORIES =	lang

V=		23.0
MAJ_V=		23
DISTNAME=	otp_src_${V}
PKGNAME=	erlang-$V

PERMIT_PACKAGE=	Yes

HOMEPAGE=	http://www.erlang.org/
MASTER_SITES=	${HOMEPAGE}download/

DISTFILES=	${DISTNAME}-rc1${EXTRACT_SUFX} \
		otp_doc_man_${V}-rc1${EXTRACT_SUFX}

EXTRACT_ONLY=	${DISTNAME}-rc1${EXTRACT_SUFX}


COMPILER=	base-clang

CONFIGURE_STYLE=	gnu
CONFIGURE_ARGS+=	--without-jinterface	\
			--without-odbc		\
			--disable-hipe

USE_GMAKE=	Yes

WANTLIB=	c crypto kvm curses util m pthread

.include <bsd.port.mk>

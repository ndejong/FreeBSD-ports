# Created by: Yen-Ming Lee <leeym@FreeBSD.org>
# $FreeBSD$

PORTNAME=	gflags
PORTVERSION=	2.2.1
DISTVERSIONPREFIX=	v
CATEGORIES=	devel

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Commandline flags module for C++

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/COPYING.txt

CMAKE_ARGS=	-DGFLAGS_NAMESPACE:STRING=gflags
CMAKE_OFF=	REGISTER_INSTALL_PREFIX
CMAKE_ON=	BUILD_SHARED_LIBS BUILD_STATIC_LIBS BUILD_TESTING \
		INSTALL_HEADERS INSTALL_SHARED_LIBS INSTALL_STATIC_LIBS
TEST_TARGET=	test
USE_LDCONFIG=	yes
USES=		cmake pathfix shebangfix

USE_GITHUB=	yes

SHEBANG_FILES=	src/gflags_completions.sh

.include <bsd.port.mk>

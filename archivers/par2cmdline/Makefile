# Created by: Chris Larsen <darth@vader.dk>
# $FreeBSD: head/archivers/par2cmdline/Makefile 362027 2014-07-16 03:47:05Z adamw $

PORTNAME=	par2cmdline
CATEGORIES=	archivers
DISTVERSION=	0.8.0

USES=	autoreconf
USE_GITHUB=	yes
GH_ACCOUNT=	Parchive
DISTVERSIONPREFIX=	v

MAINTAINER=	ihatemyisp@gmail.com
COMMENT=	Tools for using Parity v2 Archive files

LICENSE=	GPLv2


GNU_CONFIGURE=	yes

PORTDOCS=	README
CONFLICTS=	par2cmdline-tbb-[0-9]*

PLIST_FILES=	bin/par2 bin/par2create bin/par2repair bin/par2verify

OPTIONS_DEFINE=	DOCS

post-install:
	@${MKDIR} ${STAGEDIR}${DOCSDIR}
	${INSTALL_DATA} ${WRKSRC}/README ${STAGEDIR}${DOCSDIR}

.include <bsd.port.mk>

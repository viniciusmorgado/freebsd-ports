PORTNAME=	blist
PORTVERSION=	1.3.6
PORTREVISION=	2
CATEGORIES=	devel python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}

MAINTAINER=	ports@FreeBSD.org
COMMENT=	Drop-in list replacement with better performance for large lists
WWW=		http://stutzbachenterprises.com/blist/

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

DEPRECATED=	Abandoned project, no consumers, no modern python support
EXPIRATION_DATE=	2025-04-03

USES=		python:3.9
USE_PYTHON=	autoplist distutils

do-test:
	@(cd ${WRKSRC} && ${PYTHON_CMD} ${PYDISTUTILS_SETUP} test)

post-install:
	${STRIP_CMD} ${STAGEDIR}${PYTHON_SITELIBDIR}/blist/*.so

.include <bsd.port.mk>

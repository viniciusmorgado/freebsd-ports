PORTNAME=	django-debug-toolbar
PORTVERSION=	5.2.0
CATEGORIES=	www python
MASTER_SITES=	PYPI
PKGNAMEPREFIX=	${PYTHON_PKGNAMEPREFIX}dj52-
DISTNAME=	django_debug_toolbar-${PORTVERSION}

MAINTAINER=	sunpoet@FreeBSD.org
COMMENT=	Configurable set of panels to display debug information
WWW=		https://django-debug-toolbar.readthedocs.io/en/latest/ \
		https://github.com/django-commons/django-debug-toolbar

LICENSE=	BSD3CLAUSE
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=	${PYTHON_PKGNAMEPREFIX}hatchling>=0:devel/py-hatchling@${PY_FLAVOR}
RUN_DEPENDS=	${PYTHON_PKGNAMEPREFIX}django52>=4.2.9:www/py-django52@${PY_FLAVOR} \
		${PYTHON_PKGNAMEPREFIX}sqlparse>=0.2.0:databases/py-sqlparse@${PY_FLAVOR}

USES=		python:3.10+
USE_PYTHON=	autoplist concurrent pep517

NO_ARCH=	yes

CONFLICTS_INSTALL=	${PYTHON_PKGNAMEPREFIX}*django-debug-toolbar

.include <bsd.port.mk>

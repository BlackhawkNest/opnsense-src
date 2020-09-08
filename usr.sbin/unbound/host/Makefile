# Vendor sources and generated files
LDNSDIR=$	${SRCTOP}/contrib/ldns
UNBOUNDDIR=	${SRCTOP}/contrib/unbound

.PATH: ${UNBOUNDDIR} ${UNBOUNDDIR}/smallapp ${UNBOUNDDIR}/doc

PROG=	unbound-host
SRCS=	unbound-host.c
CFLAGS+=	-I${UNBOUNDDIR} -I${LDNSDIR}
CFLAGS+=	-I${.CURDIR:H} -I${.CURDIR}
LIBADD=	unbound crypto ssl pthread
MAN=	unbound-host.1

.include <bsd.prog.mk>

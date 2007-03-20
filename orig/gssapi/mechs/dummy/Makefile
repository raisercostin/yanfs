#
# Copyright (c) 1999, 2007 Sun Microsystems, Inc.
# All Rights Reserved.
# 
# Redistribution and use in source and binary forms, with or without
# modification, are permitted provided that the following conditions 
# are met:
# 
# -Redistributions of source code must retain the above copyright notice,
# this list of conditions and the following disclaimer.
# 
# -Redistribution in binary form must reproduce the above copyright
# notice, this list of conditions and the following disclaimer in the
# documentation and/or other materials provided with the distribution.
# 
# Neither the name of Sun Microsystems, Inc. or the names of contributors
# may be used to endorse or promote products derived from this software
# without specific prior written permission.
# 
# This software is provided "AS IS," without a warranty of any kind. ALL
# EXPRESS OR IMPLIED CONDITIONS, REPRESENTATIONS AND WARRANTIES, INCLUDING
# ANY IMPLIED WARRANTY OF MERCHANTABILITY, FITNESS FOR A PARTICULAR
# PURPOSE OR NON-INFRINGEMENT, ARE HEREBY EXCLUDED. SUN AND ITS LICENSORS
# SHALL NOT BE LIABLE FOR ANY DAMAGES OR LIABILITIES SUFFERED BY LICENSEE
# AS A RESULT OF OR RELATING TO USE, MODIFICATION OR DISTRIBUTION OF THE
# SOFTWARE OR ITS DERIVATIVES. IN NO EVENT WILL SUN OR ITS LICENSORS BE
# LIABLE FOR ANY LOST REVENUE, PROFIT OR DATA, OR FOR DIRECT, INDIRECT,
# SPECIAL, CONSEQUENTIAL, INCIDENTAL OR PUNITIVE DAMAGES, HOWEVER CAUSED
# AND REGARDLESS OF THE THEORY OF LIABILITY, ARISING OUT OF THE USE OF OR
# INABILITY TO USE SOFTWARE, EVEN IF SUN HAS BEEN ADVISED OF THE
# POSSIBILITY OF SUCH DAMAGES.
# 
# You acknowledge that this software is not designed,licensed or intended
# for use in the design, construction, operation or maintenance of any
# nuclear facility.
#

PKGDIR=	com/sun/gssapi/dummy

include ../../../Makefile.common

CLASSES= Dummy DummyCtxt DummyName DummyCred

JFILES=	$(CLASSES:%=%.java)

all:	$(TFILE)
$(TFILE):	$(JFILES)
	$(JC) -d $(CDIR) $(JCFLAGS) $?
	@touch $(TFILE)


#
# Name mangling
#
# Properties key=value strings
M4DEF_PROP = -D NAMES=_K872D1AC
M4DEF_PROP += -D NAME=_K532D1BD
M4DEF_PROP += -D CONTEXT=_K1000A49
M4DEF_PROP += -D CRED=_K2102CC5

Dummy.java: Dummy.m4
	/usr/ccs/bin/m4 $(M4DEF_PROP) Dummy.m4 > Dummy.java 

# Service Provider Interface Context Class and its methods/interface
M4DEF_CTXTSPI = -D GSSCtxtSpi=C018FE95
M4DEF_CTXTSPI += -D _setInitOptions=_S235D9C1
M4DEF_CTXTSPI += -D _setAcceptOptions=_S90010CC
M4DEF_CTXTSPI += -D _setChannelBinding=_S9B00AB2
M4DEF_CTXTSPI += -D _getOptions=_S00027C3
M4DEF_CTXTSPI += -D _getLifetime=_S4080EED
M4DEF_CTXTSPI += -D _getMech=_S0200735
M4DEF_CTXTSPI += -D _getSrcName=_S000EEFF
M4DEF_CTXTSPI += -D _getTargName=_S011CEF9
M4DEF_CTXTSPI += -D _getDelegCred=_S0293FFA
M4DEF_CTXTSPI += -D _isInitiator=_S123049E
M4DEF_CTXTSPI += -D _isProtReady=_S1116FAA
M4DEF_CTXTSPI += -D _initSecCtxt=_S0E039DB
M4DEF_CTXTSPI += -D _acceptSecCtxt=_S80A2F2C
M4DEF_CTXTSPI += -D _getWrapSizeLimit=_S808028B
M4DEF_CTXTSPI += -D _wrap=_S1309AFD
M4DEF_CTXTSPI += -D _unwrap=_S1576D09
M4DEF_CTXTSPI += -D _getMIC=_S1513DBA
M4DEF_CTXTSPI += -D _verifyMIC=_S00256CF
M4DEF_CTXTSPI += -D _export=_S725B2DA
M4DEF_CTXTSPI += -D _importSecCtxt=_S0AC8F9E
M4DEF_CTXTSPI += -D _dispose=_S020B957

DummyCtxt.java: DummyCtxt.m4
	/usr/ccs/bin/m4 $(M4DEF_CTXTSPI) DummyCtxt.m4 > DummyCtxt.java


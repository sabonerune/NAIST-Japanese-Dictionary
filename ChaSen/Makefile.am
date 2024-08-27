# $Id: Makefile.am,v 1.25 2003/08/15 03:11:58 masayu-a Exp $
MKDICDIR      = @CHASEN_MKCHADIC_DIR@
dicdir        = @CHASEN_DIC_DIR@/@PACKAGE@
manual_files   = @CHASEN_MANUAL_FILES@
lexical_dic   = @CHASEN_LEXICAL_DIC@
gen_data      = @CHASEN_GENDATA@
pre_data      = @CHASEN_PREDATA@

SUBDIRS = doc

dic_DATA      = $(pre_data) $(gen_data)
EXTRA_DIST    = $(pre_data) $(lexical_dic) $(manual_files) 
CLEANFILES    = $(gen_data)
#
matrix.cha table.cha:
	$(MKDICDIR)/makemat

chadic.da: 
	$(MKDICDIR)/makeda chadic *.dic

install-data-local:
	if test -f @CHASEN_CHASENRC_PATH@  ; then \
		echo "Please modify @CHASEN_CHASENRC_PATH@"; \
	else \
		cp chasenrc @CHASEN_CHASENRC_PATH@ ;\
	fi


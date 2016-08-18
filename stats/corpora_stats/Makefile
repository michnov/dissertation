DATA_DIR=../../data

pdt.stats :
	echo "PDT 3.0 - train:" > $@
	treex -p --jobs 100 -Lcs -Sref \
		Read::Treex from='@$(DATA_DIR)/cs/analysed/pdt/train/0009/list' \
		Util::Eval doc='print "DOC\n";' \
		Util::Eval ttree='print "SENT\n";' \
		Util::Eval language=cs selector=ref anode='print "ANODE_REF\n";' \
		Util::Eval language=cs selector=src anode='print "ANODE_SRC\n";' \
		Util::Eval language=cs selector=ref tnode='print "TNODE_REF\n";' \
		Util::Eval language=cs selector=src tnode='print "TNODE_SRC\n";' | \
	sort | uniq -c | sort -nr >> $@
	echo "PDT 3.0 - dev:" >> $@
	treex -p --jobs 50 -Lcs -Sref \
		Read::Treex from='@$(DATA_DIR)/cs/analysed/pdt/dev/0009/list' \
		Util::Eval doc='print "DOC\n";' \
		Util::Eval ttree='print "SENT\n";' \
		Util::Eval language=cs selector=ref anode='print "ANODE_REF\n";' \
		Util::Eval language=cs selector=src anode='print "ANODE_SRC\n";' \
		Util::Eval language=cs selector=ref tnode='print "TNODE_REF\n";' \
		Util::Eval language=cs selector=src tnode='print "TNODE_SRC\n";' | \
	sort | uniq -c | sort -nr >> $@
	echo "PDT 3.0 - eval:" >> $@
	treex -p --jobs 50 -Lcs -Sref \
		Read::Treex from='@$(DATA_DIR)/cs/analysed/pdt/eval/0009/list' \
		Util::Eval doc='print "DOC\n";' \
		Util::Eval ttree='print "SENT\n";' \
		Util::Eval language=cs selector=ref anode='print "ANODE_REF\n";' \
		Util::Eval language=cs selector=src anode='print "ANODE_SRC\n";' \
		Util::Eval language=cs selector=ref tnode='print "TNODE_REF\n";' \
		Util::Eval language=cs selector=src tnode='print "TNODE_SRC\n";' | \
	sort | uniq -c | sort -nr >> $@

pcedt.stats :
	echo "PCEDT 2.0 Coref - train:" > $@
	treex -p --jobs 100 -Lcs -Sref \
		Read::Treex from='@$(DATA_DIR)/cs/analysed/pcedt_bi/train_00-18/0023/list' \
		Util::Eval doc='print "DOC\n";' \
		Util::Eval ttree='print "SENT\n";' \
		Util::Eval language=cs selector=ref anode='print "ANODE_CS_REF\n";' \
		Util::Eval language=cs selector=src anode='print "ANODE_CS_SRC\n";' \
		Util::Eval language=cs selector=ref tnode='print "TNODE_CS_REF\n";' \
		Util::Eval language=cs selector=src tnode='print "TNODE_CS_SRC\n";' \
		Util::Eval language=en selector=ref anode='print "ANODE_EN_REF\n";' \
		Util::Eval language=en selector=src anode='print "ANODE_EN_SRC\n";' \
		Util::Eval language=en selector=ref tnode='print "TNODE_EN_REF\n";' \
		Util::Eval language=en selector=src tnode='print "TNODE_EN_SRC\n";' | \
	sort | uniq -c | sort -nr >> $@
	echo "PCEDT 2.0 Coref - dev:" >> $@
	treex -p --jobs 50 -Lcs -Sref \
		Read::Treex from='@$(DATA_DIR)/cs/analysed/pcedt_bi/dev/0023/list' \
		Util::Eval doc='print "DOC\n";' \
		Util::Eval ttree='print "SENT\n";' \
		Util::Eval language=cs selector=ref anode='print "ANODE_CS_REF\n";' \
		Util::Eval language=cs selector=src anode='print "ANODE_CS_SRC\n";' \
		Util::Eval language=cs selector=ref tnode='print "TNODE_CS_REF\n";' \
		Util::Eval language=cs selector=src tnode='print "TNODE_CS_SRC\n";' \
		Util::Eval language=en selector=ref anode='print "ANODE_EN_REF\n";' \
		Util::Eval language=en selector=src anode='print "ANODE_EN_SRC\n";' \
		Util::Eval language=en selector=ref tnode='print "TNODE_EN_REF\n";' \
		Util::Eval language=en selector=src tnode='print "TNODE_EN_SRC\n";' | \
	sort | uniq -c | sort -nr >> $@
	echo "PCEDT 2.0 Coref - eval:" >> $@
	treex -p --jobs 50 -Lcs -Sref \
		Read::Treex from='@$(DATA_DIR)/cs/analysed/pcedt_bi/eval/0023/list' \
		Util::Eval doc='print "DOC\n";' \
		Util::Eval ttree='print "SENT\n";' \
		Util::Eval language=cs selector=ref anode='print "ANODE_CS_REF\n";' \
		Util::Eval language=cs selector=src anode='print "ANODE_CS_SRC\n";' \
		Util::Eval language=cs selector=ref tnode='print "TNODE_CS_REF\n";' \
		Util::Eval language=cs selector=src tnode='print "TNODE_CS_SRC\n";' \
		Util::Eval language=en selector=ref anode='print "ANODE_EN_REF\n";' \
		Util::Eval language=en selector=src anode='print "ANODE_EN_SRC\n";' \
		Util::Eval language=en selector=ref tnode='print "TNODE_EN_REF\n";' \
		Util::Eval language=en selector=src tnode='print "TNODE_EN_SRC\n";' | \
	sort | uniq -c | sort -nr >> $@


ifpreupdir = $(sysconfdir)/network/if-pre-up.d
ifpreup_SCRIPTS = qinq

man5_MANS = man5/qinq.5

%.5: %.5.md
	ronn --roff $< --pipe >$@


ifpreupdir = $(sysconfdir)/network/if-pre-up.d
ifpreup_SCRIPTS = qinq

ifpostdowndir = $(sysconfdir)/network/if-post-down.d
ifpostdown_SCRIPTS = qinq

man5_MANS = qinq.5

%.5: %.5.md
	ronn --roff $< --pipe >$@

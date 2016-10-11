
ifpreupdir = $(sysconfdir)/network/if-pre-up.d
ifpreup_SCRIPTS = if-pre-up.d/qinq

ifpostdowndir = $(sysconfdir)/network/if-post-down.d
ifpostdown_SCRIPTS = if-post-down.d/qinq

man5_MANS = qinq.5

%.5: %.5.md
	ronn --roff $< --pipe >$@

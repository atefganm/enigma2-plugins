include $(top_srcdir)/Rules-cpp.mak

plugindir = $(libdir)/enigma2/python/Plugins/SystemPlugins/NetworkBrowser

plugin_LTLIBRARIES = netscan.la

netscan_la_SOURCES = \
	errors.h \
	list.c \
	list.h \
	nbtscan.c \
	nbtscan.h \
	range.c \
	range.h \
	showmount.c \
	showmount.h \
	smb.h \
	smbinfo.c \
	smbinfo.h \
	statusq.c \
	statusq.h \
	time_compat.h \
	main.c

netscan_la_LDFLAGS = \
	$(PLUGIN_LIBTOOL_FLAGS)

ACLOCAL_AMFLAGS = -I m4

SUBDIRS = \
	advhdmi \
	antiscrollbar \
	aspectratioswitch \
	audiorestart \
	audiosync \
	automaticcleanup \
	automaticvolumeadjustment \
	autoresolution \
	autotimer \
	birthdayreminder \
	bonjour \
	cdinfo \
	channelselectionshorttitle \
	curlytx \
	dreamexplorer \
	dreamirc \
	dreammediathek \
	dvdbackup \
	easyinfo \
	easymedia \
	ecasa \
	eibox \
	emailclient \
	emission \
	eparted \
	epgrefresh \
	eurotictv \
	eventlist \
	eventposition \
	filebrowser \
	flashexpander \
	fritzcall \
	fstabeditor \
	ftpbrowser \
	growlee \
	imdb \
	infobartunerstate \
	mediadownloader \
	mosaic \
	moviecut \
	movieretitle \
	movietagger \
	mphelp \
	ofdb \
	permanentclock \
	pipservicerelation \
	podcast \
	reconstructapsc \
	reftopiconname \
	shoutcast \
	simplerss \
	startuptostandby \
	tageditor \
	toolkit \
	vlcplayer \
	vps \
	weatherplugin \
	weathercomponent \
	weathercomponenthandler \
	werbezapper \
	zapstatistic \
	esame \
	sudoku \
	vierg \
	bmediacenter

if DREAMBOX
SUBDIRS +=  fancontrol2 letterbox logomanager movielistpreview genuinedreambox
endif

if VUSOLO2
SUBDIRS +=  fancontrol2
endif
if VUDUO2
SUBDIRS +=  fancontrol2
endif
if VUUNO
SUBDIRS +=  fancontrol2
endif
if VUULTIMO
SUBDIRS +=  fancontrol2
endif

if XC7346
SUBDIRS +=  fancontrol2
endif

if TPM
SUBDIRS += \
	mytube \
	yttrailer \
	pluginhider \
	pluginsort 
endif

if PLI
SUBDIRS += networkbrowserpli epgsearchpli
else
SUBDIRS += networkbrowser epgsearch
endif

SUBDIRS += tetris ardmediathek netzkino Series2Folder srfmediathek epgexport

metadir = $(datadir)/meta
meta_DATA = index-enigma2-plugins.xml
CLEANFILES = index-enigma2-plugins.xml

index-enigma2-plugins.xml: $(top_srcdir)/genmetaindex.py $(top_srcdir)/*/meta/plugin_*.xml
	$(AM_V_GEN)$(PYTHON) $^ > $@

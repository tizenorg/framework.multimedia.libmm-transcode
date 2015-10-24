bin_PROGRAMS = mm_transcode_testsuite

mm_transcode_testsuite_SOURCES = mm_transcode_testsuite.c

mm_transcode_testsuite_CFLAGS = -I$(srcdir)/../include \
                                $(MMCOMMON_CFLAGS) \
                                $(GLIB_CFLAGS) \
                                $(GST_CFLAGS) \
                                $(GSTAPP_CFLAGS)  \
                                $(GST_PLUGIN_BASE_CFLAGS) \
                                $(GST_INTERFACE_CFLAGS) \
                                $(GSTPBUTILS_CFLAGS) \
                                $(MMLOG_CFLAGS) -DMMF_LOG_OWNER=0x300000 -DMMF_DEBUG_PREFIX=\"MMF-TRANSCODE\" -fPIE -pie

mm_transcode_testsuite_DEPENDENCIES = $(srcdir)/../libmm_transcode.la

mm_transcode_testsuite_LDADD = $(srcdir)/../libmm_transcode.la \
                               $(MMCOMMON_LIBS) \
                               $(GLIB_LIBS) \
                               $(GST_LIBS) \
                               $(GST_PLUGIN_BASE_LIBS) \
                               $(GST_INTERFACE_LIBS) \
                               $(GSTPBUTILS_LIBS) \
                               $(GSTAPP_LIBS) \
                               $(MMLOG_LIBS)

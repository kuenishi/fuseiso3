AC_INIT(fuseiso, 20200720)
AM_INIT_AUTOMAKE
AC_CONFIG_SRCDIR(configure.ac)
AM_CONFIG_HEADER(config.h)
AC_CONFIG_MACRO_DIRS([m4])

AC_LANG_C
AC_PROG_CC
AM_PROG_LIBTOOL

PKG_CHECK_MODULES(zlib, zlib)
PKG_CHECK_MODULES(glib, [glib-2.0])
PKG_CHECK_MODULES(fuse3, fuse3)

#AC_CHECK_HEADERS(fuse.h, [], 
#    [ AC_MSG_ERROR([libfuse3 header is required]) ])
#ifndef _FILE_OFFSET_BITS
#define _FILE_OFFSET_BITS 64
#endif


#AC_CHECK_LIB(fuse3, fuse_main, [],
#    [ AC_MSG_ERROR([libfuse3 is required]) ])

AC_OUTPUT(Makefile src/Makefile zAppRun/Makefile)

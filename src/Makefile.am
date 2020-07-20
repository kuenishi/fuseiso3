bin_PROGRAMS = fuseiso
fuseiso_SOURCES = fuseiso.c isofs.c

# set the include path found by configure
# INCLUDES= $(all_includes)
# AM_CPPFLAGS= $(all_includes)

# the library search path.
fuseiso_LDFLAGS = $(all_libraries)
noinst_HEADERS = isofs.h

#  -Wall -D_FILE_OFFSET_BITS=64 isn't required in fuse 3
AM_CFLAGS = `pkg-config --cflags --libs fuse3 glib-2.0` -lz
AM_LDFLAGS = `pkg-config --libs fuse3 glib-2.0` -lz

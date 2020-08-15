# Relative path from here to uninstalled library
INCLUDE_DIR = $(top_builddir)/include
LIB_EGL_DIR = $(top_builddir)/src
LIB_VULCANO_EGL = ${LIB_EGL_DIR}/libEGL.la

# Variables which are common to all example programs
# (Combine variables passed from configure script with
# the local path to uninstalled library)
EXAMPLE_SRCS = test.h test.c
EXAMPLE_CF = @CONFIG_CFLAGS@ -I${INCLUDE_DIR} -I${prefix}/include
EXAMPLE_LA = @CONFIG_LDADD@ ${LIB_VULCANO_EGL}
EXAMPLE_LF = @CONFIG_LDFLAGS@ -L${prefix}/lib

EXTRA_DIST = *.jpg *.png

noinst_PROGRAMS =

if BUILD_EGL
noinst_PROGRAMS += test_egl
endif

test_egl_SOURCES =\
	${EXAMPLE_SRCS} test_egl.c

test_egl_CFLAGS = ${EXAMPLE_CF}
test_egl_LDADD = ${EXAMPLE_LA}
test_egl_LDFLAGS = ${EXAMPLE_LF}


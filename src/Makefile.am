
lib_LTLIBRARIES = libEGL.la

libEGL_la_CFLAGS = \
	-pedantic -I$(top_builddir)/include

libEGL_la_SOURCES =\
	EGL/eglapi.c\
	EGL/eglarray.c\
	EGL/eglconfig.c\
	EGL/eglcontext.c\
	EGL/eglcurrent.c\
	EGL/egldevice.c\
	EGL/egldisplay.c\
	EGL/egldriver.c\
	EGL/eglglobals.c\
	EGL/eglimage.c\
	EGL/egllog.c\
	EGL/eglsurface.c\
	EGL/eglsync.c\
	EGL/egldriverVulkan.c

EGL_includedir = $(includedir)/EGL

EGL_include_HEADERS =\
	$(top_builddir)/include/EGL/egl.h\
	$(top_builddir)/include/EGL/eglext.h\
	$(top_builddir)/include/EGL/eglplatform.h\
	$(top_builddir)/include/EGL/khrplatform.h


#AM_CFLAGS = --pedantic -Wall
#-DDEBUG

nudoku_LDADD = -lncurses
bin_PROGRAMS = nudoku
nudoku_SOURCES = main.c sudoku.c sudoku.h

if BUILD_CAIRO
nudoku_SOURCES += outp.c outp.h
AM_CFLAGS := @CAIRO_CFLAGS@
nudoku_LDADD += @CAIRO_LIBS@
endif

AM_CPPFLAGS = -DLOCALEDIR=\""$(localedir)"\"
LIBS = @LIBINTL@

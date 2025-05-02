# SPDX-License-Identifier: GPL-2.0-or-later

noinst_LTLIBRARIES += %D%/libflash.la
%C%_libflash_la_SOURCES = \
	%D%/common.c %D%/common.h \
	%D%/advanced_elf_image.c %d%/advanced_elf_image.h \
	%D%/FLASHPlugin.c

AM_CPPFLAGS += -I$(top_srcdir)/src/helper

%C%_libflash_la_LIBADD = \
	%D%/nor/libocdflashnor.la \
	%D%/nand/libocdflashnand.la

STARTUP_TCL_SRCS += %D%/startup.tcl


include %D%/nor/Makefile.am
include %D%/nand/Makefile.am

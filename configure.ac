dnl Process this file with autoconf to produce a configure script.
AC_INIT(src/main.c)

VERSION=1.0.0
PACKAGE=mibjig

AM_INIT_AUTOMAKE($PACKAGE, $VERSION)

AM_MAINTAINER_MODE

AM_CONFIG_HEADER(src/config.h)

dnl Checks for programs.
AC_PROG_CC
AC_ISC_POSIX
AC_PROG_INSTALL
AC_PROG_LN_S

dnl Checks for header files.
AC_HEADER_STDC
AC_CHECK_HEADER(unistd.h, , AC_MSG_ERROR([Error : construct requires unistd.h]))
AC_CHECK_HEADER(sys/stat.h, , AC_MSG_ERROR([Error : construct requires sys/stat.h]))
AC_CHECK_HEADER(sys/types.h, , AC_MSG_ERROR([Error : construct requires sys/type.h]))
AC_CHECK_HEADER(sys/ipc.h, , AC_MSG_ERROR([Error : construct requires sys/ipc.h]))
AC_CHECK_HEADER(sys/socket.h, , AC_MSG_ERROR([Error : construct requires sys/socket.h]))
AC_CHECK_HEADER(sys/wait.h, , AC_MSG_ERROR([Error : construct requires sys/wait.h]))
AC_CHECK_HEADER(fcntl.h, , AC_MSG_ERROR([Error : construct requires fcntl.h]))
AC_CHECK_HEADER(stdlib.h, , AC_MSG_ERROR([Error : construct requires stdlib.h]))
AC_CHECK_HEADER(syslog.h, , AC_MSG_ERROR([Error : construct requires syslog.h]))
AC_CHECK_HEADER(netinet/in.h, , AC_MSG_ERROR([Error : construct requires netinet/in.h]))
AC_CHECK_HEADER(netdb.h, , AC_MSG_ERROR([Error : construct requires netdb.h]))
AC_CHECK_HEADER(errno.h, , AC_MSG_ERROR([Error : construct requires errno.h]))
AC_CHECK_HEADER(string.h, , AC_MSG_ERROR([Error : construct requires string.h]))

AC_HAVE_LIBRARY(pcre)
AC_HAVE_LIBRARY(netsnmp)
AC_HAVE_LIBRARY(netsnmplibs)
AC_HAVE_LIBRARY(netsnmphelpers)
AC_HAVE_LIBRARY(netsnmpagent)

AC_OUTPUT(	Makefile 		\
		src/Makefile		\
		)

#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([MyGestures], [2.0], [lucasdeters@users.sourceforge.net])
AM_INIT_AUTOMAKE([subdir-objects])
AC_CONFIG_SRCDIR([src/mygestures.c])
AC_CONFIG_HEADERS([src/config.h])

# Checks for programs.
AC_PROG_CC

# Checks for libraries.
PKG_CHECK_MODULES(X11, x11)
PKG_CHECK_MODULES(Xrender, xrender)
PKG_CHECK_MODULES(Xtst, xtst)
PKG_CHECK_MODULES(Xi, xi)
PKG_CHECK_MODULES(libXML, libxml-2.0 >= 2.4)

AC_SEARCH_LIBS([shm_open], [rt], [])

# Checks for header files.
AC_PATH_X
AC_CHECK_HEADERS([fcntl.h stdlib.h string.h strings.h unistd.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_MODE_T

# Checks for library functions.
AC_FUNC_FORK
AC_FUNC_MALLOC
AC_CHECK_FUNCS([bzero memset mkdir regcomp strcasecmp strdup strncasecmp])          

AC_CONFIG_FILES([Makefile
                 src/Makefile])
                 
                 

            
AC_OUTPUT



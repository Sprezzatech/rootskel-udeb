DEB_HOST_ARCH_OS ?= $(shell dpkg-architecture -qDEB_HOST_ARCH_OS 2>/dev/null)

dir =

subdirs = \
	etc \
	lib \
	sbin \
	var

subdirs_empty = \
	dev \
	media \
	initrd \
	mnt \
	proc \
	sys

ifeq ($(DEB_HOST_ARCH_OS),linux)
  files_exec = \
	init

  subdirs_empty += \
	run
endif

include ../Makefile.inc

#MAKEFILES = $(shell find . -maxdepth 2 -type f -name Makefile)
#SUBDIRS   = $(filter-out ./,$(dir $(MAKEFILES)))

SUBDIRS = $(shell ls -d */)
all:
	for dir in $(SUBDIRS) ; do \
		make -C  $$dir ; \
	done
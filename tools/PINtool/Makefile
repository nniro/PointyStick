##############################################################
#
#                   DO NOT EDIT THIS FILE!
#
##############################################################

ifeq ($(OS),Windows_NT)
else
UNAME := $(shell uname)
ifeq ($(UNAME), Darwin)
HOST_ARCH ?= intel64
endif
endif

ifdef m64
HOST_ARCH ?= intel64
else
HOST_ARCH ?= ia32
endif

ifdef PIN_ROOT
CONFIG_ROOT := $(PIN_ROOT)/source/tools/Config
else
all:
	@echo Please define PIN_ROOT.
endif

include $(CONFIG_ROOT)/makefile.config
include makefile.rules
include $(TOOLS_ROOT)/Config/makefile.default.rules

##############################################################
#
#                   DO NOT EDIT THIS FILE!
#
##############################################################


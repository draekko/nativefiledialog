# GNU Make workspace makefile autogenerated by Premake

.NOTPARALLEL:

ifndef config
  config=release_x64
endif

ifndef verbose
  SILENT = @
endif

ifeq ($(config),release_x64)
  nfd_config = release_x64
  test_pickfolder_config = release_x64
  test_opendialog_config = release_x64
  test_opendialogmultiple_config = release_x64
  test_savedialog_config = release_x64
endif
ifeq ($(config),release_x86)
  nfd_config = release_x86
  test_pickfolder_config = release_x86
  test_opendialog_config = release_x86
  test_opendialogmultiple_config = release_x86
  test_savedialog_config = release_x86
endif
ifeq ($(config),debug_x64)
  nfd_config = debug_x64
  test_pickfolder_config = debug_x64
  test_opendialog_config = debug_x64
  test_opendialogmultiple_config = debug_x64
  test_savedialog_config = debug_x64
endif
ifeq ($(config),debug_x86)
  nfd_config = debug_x86
  test_pickfolder_config = debug_x86
  test_opendialog_config = debug_x86
  test_opendialogmultiple_config = debug_x86
  test_savedialog_config = debug_x86
endif

PROJECTS := nfd test_pickfolder test_opendialog test_opendialogmultiple test_savedialog

.PHONY: all clean help $(PROJECTS) 

all: $(PROJECTS)

nfd:
ifneq (,$(nfd_config))
	@echo "==== Building nfd ($(nfd_config)) ===="
	@${MAKE} --no-print-directory -C . -f nfd.make config=$(nfd_config)
endif

test_pickfolder: nfd
ifneq (,$(test_pickfolder_config))
	@echo "==== Building test_pickfolder ($(test_pickfolder_config)) ===="
	@${MAKE} --no-print-directory -C . -f test_pickfolder.make config=$(test_pickfolder_config)
endif

test_opendialog: nfd
ifneq (,$(test_opendialog_config))
	@echo "==== Building test_opendialog ($(test_opendialog_config)) ===="
	@${MAKE} --no-print-directory -C . -f test_opendialog.make config=$(test_opendialog_config)
endif

test_opendialogmultiple: nfd
ifneq (,$(test_opendialogmultiple_config))
	@echo "==== Building test_opendialogmultiple ($(test_opendialogmultiple_config)) ===="
	@${MAKE} --no-print-directory -C . -f test_opendialogmultiple.make config=$(test_opendialogmultiple_config)
endif

test_savedialog: nfd
ifneq (,$(test_savedialog_config))
	@echo "==== Building test_savedialog ($(test_savedialog_config)) ===="
	@${MAKE} --no-print-directory -C . -f test_savedialog.make config=$(test_savedialog_config)
endif

clean:
	@${MAKE} --no-print-directory -C . -f nfd.make clean
	@${MAKE} --no-print-directory -C . -f test_pickfolder.make clean
	@${MAKE} --no-print-directory -C . -f test_opendialog.make clean
	@${MAKE} --no-print-directory -C . -f test_opendialogmultiple.make clean
	@${MAKE} --no-print-directory -C . -f test_savedialog.make clean

help:
	@echo "Usage: make [config=name] [target]"
	@echo ""
	@echo "CONFIGURATIONS:"
	@echo "  release_x64"
	@echo "  release_x86"
	@echo "  debug_x64"
	@echo "  debug_x86"
	@echo ""
	@echo "TARGETS:"
	@echo "   all (default)"
	@echo "   clean"
	@echo "   nfd"
	@echo "   test_pickfolder"
	@echo "   test_opendialog"
	@echo "   test_opendialogmultiple"
	@echo "   test_savedialog"
	@echo ""
	@echo "For more information, see http://industriousone.com/premake/quick-start"
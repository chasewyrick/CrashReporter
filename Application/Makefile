APPLICATION_NAME = CrashReporter
CrashReporter_FILES = \
    BlameController.m \
    CrashLogDateChooser.m \
    CrashLogViewController.m \
    CrashLogsFolderReader.m \
    CrashLogsTableController.m \
    CrashReporterDelegate.m \
    CustomBlameController.m \
    ModalActionSheet.m \
    RegexKitLite.m \
    SuspectsViewController.m \
    common.c \
    find_dpkg.m \
    main.m \
    move_as_root.m \
    pastie.m \
    reporter.m
CrashReporter_CFLAGS = -I ../symbolicate
CrashReporter_LDFLAGS = -licucore
CrashReporter_FRAMEWORKS = MessageUI SystemConfiguration UIKit
CrashReporter_PRIVATE_FRAMEWORKS = Symbolication

include $(THEOS_MAKE_PATH)/common.mk
include $(THEOS_MAKE_PATH)/application.mk

after-clean::
	- rm -rf $(THEOS_PROJECT_DIR)/Application/symbolicate

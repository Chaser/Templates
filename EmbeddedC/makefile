# ==========================================
#   Template Project
#   Copyright (c) 2014 Chase Johnson
# ========================================== 

#
TARGET_BASE = HelloWorld

#COMPILIER = gcc
COMPILER = g++
ifeq ($(OS),Windows_NT)
	TARGET_EXTENSION=.exe
else
	TARGET_EXTENSION=.out
endif
TARGET = $(TARGET_BASE)$(TARGET_EXTENSION)
OUTPUT=-o $(TARGET)

#INCLUDE FILES


#SYMBOLS



#SOURCE FILES
SRC_FILES=src/unity.c



CLEANUP = rm -f ../build/* ; rm -f $(TARGET) ; mkdir -p ../build

#Check for windows otherwise assume OSX (Darwin) or posix
#ifeq ($(OS),Windows_NT)
#else
#	CLEANUP = rm -f build/* ; rm -f $(TARGET) ; mkdir -p build

#endif

all: clean default

default:
	$(info *** Default Action - Building Project ***)
	$(COMPILER) $(INC_DIRS) $(SYMBOLS) $(SRC_FILES) $(OUT_FILE)
	./$(TARGET)
	

clean:
	$(CLEANUP)
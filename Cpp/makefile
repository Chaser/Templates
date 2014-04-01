# ==========================================
#   Template Project
#   Copyright (c) 2014 Chase Johnson
# ========================================== 

#
TARGET_BASE = HelloWorld

#COMPILIER = gcc
COMPILER = g++
OUTPUT_DIRECTORY = -o bin/

ifeq ($(OS),Windows_NT)
	TARGET_EXTENSION=.exe
else
	TARGET_EXTENSION=.out
endif
TARGET = $(TARGET_BASE)$(TARGET_EXTENSION)


#INCLUDE FILES


#SYMBOLS



#SOURCE FILES
SOURCE_FILES=src/HelloWorld.cpp


CLEANUP = rm -f ../build/* ; rm -f $(TARGET) ; mkdir -p ../build

#Check for windows otherwise assume OSX (Darwin) or posix
#ifeq ($(OS),Windows_NT)
#else
#	CLEANUP = rm -f build/* ; rm -f $(TARGET) ; mkdir -p build

#endif

all: clean default

default:
	$(info *** Default Action - Building Project ***)
	$(COMPILER) $(INC_DIRS) $(SYMBOLS) $(SOURCE_FILES) $(OUTPUT_DIRECTORY)$(TARGET)
	./bin/$(TARGET)
	

clean:
	$(CLEANUP)
TOP_DIR := $(shell pwd)
APP = $(TOP_DIR)/cameratoh264
DEP_LIBS = -L$(TOP_DIR)/lib/mips/lib
HEADER = -I$(TOP_DIR)/lib/mips/include
#DEP_LIBS = -L$(TOP_DIR)/lib/x86/lib
#HEADER = -I$(TOP_DIR)/lib/x86/include

CC = gcc
CFLAGS = -g $(HEADER)
LIBS = -lpthread -lx264 -lm -ldl
OBJS = main.o video_capture.o h264encoder.o

all:  $(OBJS)
	$(CC) -g -o $(APP) $(OBJS) $(LIBS) $(DEP_LIBS) 

clean:
	rm -f *.o a.out $(APP) core *~

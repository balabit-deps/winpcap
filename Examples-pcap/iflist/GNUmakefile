# Makefile for cygwin gcc
# Nate Lawson <nate@rootlabs.com>

CFLAGS = -g -O -mno-cygwin -I ../../wpcap/libpcap -I ../../wpcap/libpcap/Win32/include

OBJS = iflist.o
LIBS = -L ../../wpcap/PRJ/ -L ../../packetNtx/Dll/Project -lwpcap

all: ${OBJS}
	${CC} ${CFLAGS} -o iflist.exe ${OBJS} ${LIBS}

clean:
	rm -f ${OBJS} iflist.exe

.c.o:
	${CC} ${CFLAGS} -c -o $*.o $<

.PHONY: clean

CFLAGS	:= -Wall -g -O2
LD	:= gcc
LDFLAGS	:= -libverbs -lrdmacm

APPS	:= mckey

all: ${APPS}

mckey: mckey.o
	${LD} -g -o $@ $^ ${LDFLAGS}

clean:
	rm -f *.o ${APPS} 

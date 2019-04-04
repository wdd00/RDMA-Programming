.PHONY: clean

CFLAGS	:= -Wall -g -O2
LD	:= gcc
LDFLAGS	:= -libverbs -lrdmacm -lpthread

APPS	:= mc

all: ${APPS}

mckey: mc.o
	${LD} -g -o $@ $^ ${LDFLAGS}

clean:
	rm -f *.o ${APPS} 

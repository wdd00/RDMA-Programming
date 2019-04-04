.PHONY: clean

LD	:= gcc
LDFLAGS	:= -libverbs -lrdmacm -lpthread

APPS	:= apm

all: ${APPS}

apm: apm.o
	${LD} -g -o $@ $^ ${LDFLAGS}

clean:
	rm -f *.o ${APPS}

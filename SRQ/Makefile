.PHONY: clean

LD	:= gcc
LDFLAGS	:= -libverbs -lrdmacm

APPS	:= srq

all: ${APPS}

srq: srq.o
	${LD} -g -o $@ $^ ${LDFLAGS}

clean:
	rm -f *.o ${APPS} 

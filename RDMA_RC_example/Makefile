.PHONY: clean

CFLAGS	:= -Wall -g -O2
LD 	:= gcc
LDFLAGS	:= -libverbs

APPS	:= RDMA_RC_example

all: ${APPS}

RDMA_RC_example: RDMA_RC_example.o
	${LD} -g -o $@ $^ ${LDFLAGS}

clean:
	rm -f *.o ${APPS}

CFLAGS = -c -Wall
CC = gcc
LIBS =  -lm
JRB = ../../Libfdr/jrb.c
JVAL = ../../Libfdr/jval.c 
all: main

main : main.o function.o jrb.o jval.o 
	${CC} main.o jrb.o jval.o

main.o: main.c
	${CC} ${CFLAGS} main.c

function.o: function.c
	${CC} ${CFLAGS} function.c

jrb.o: 
	${CC} ${CFLAGS} ${JRB}

jval.o:
	${CC} ${CFLAGS} ${JVAL}

clean:
	rm -f *.o *~ 

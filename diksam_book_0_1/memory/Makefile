TARGET = mem.o
CC=gcc
CFLAGS = -c -g3 -gdwarf-4 -DDEBUG -Wall
OBJS = memory.o storage.o

$(TARGET):$(OBJS)
	ld -r -o $@ $(OBJS)
testp : $(OBJS) main.o
	$(CC) -o $@ $(OBJS) main.o
.c.o:
	$(CC) $(CFLAGS) -I../include $*.c
main.o: main.c ../include/MEM.h
memory.o: memory.c memory.h ../include/MEM.h
storage.o: storage.c memory.h ../include/MEM.h

.PHONY: clean
clean:
	-rm -fr *.o

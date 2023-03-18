CFLAGS = -O3 -pedantic-errors

build:
	gcc $(CFLAGS) -c main.c 
	gcc $(CFLAGS) -S -o main.asm main.c
	gcc $(CFLAGS) -o program main.o
clean:
	rm *.o
	rm program
	rm *.asm
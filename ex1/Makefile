CC=gcc
CFLAGS=-O3 -g
LDFLAGS=-lm

TARGET=main

all: $(TARGET)

libppm.so : ppm.c
	$(CC) $(CFLAGS) -fpic -shared $^ -o $@

main: main.c libppm.so
	$(CC) $(CFLAGS) $(LDFLAGS) main.c -L. -lppm -Wl,-rpath=$(PWD) -o $@

clean:
	rm -f $(TARGET) *.so

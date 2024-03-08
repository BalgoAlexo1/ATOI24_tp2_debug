CC=gcc
CFLAGS= -Wall -Wextra -pthread

TARGET=lock
all: $(TARGET)

lock: lock.c 
	$(CC) $(CFLAGS) $^ -o $@

clean:
	rm -f $(TARGET) 

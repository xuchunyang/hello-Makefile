TARGET = program
LIBS = -lm
CC = gcc
CFLAGS = -g -Wall

.PHONY: default all clean

default: $(TARGET)
all: default

OBJECTS = program.o
HEADERS = program.h headers.h

%.o: %.c $(HEADERS)
	$(CC) $(CFLAGS) -c $< -o $@

program: $(OBJECTS)
	gcc $(OBJECTS) -o $@

clean:
	-rm -f $(OBJECTS)
	-rm -f program

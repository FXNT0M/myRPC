CC = gcc
CFLAGS = -Wall -g -fPIC -I/home/fxnt0m/mysyslog/libmysyslog
LDFLAGS = -shared
TARGET = libmysyslog-text.so

all: $(TARGET)

$(TARGET): libmysyslog-text.o
	$(CC) $(LDFLAGS) -o $@ $<

libmysyslog-text.o: libmysyslog-text.c
	$(CC) $(CFLAGS) -c $<
clean:
	rm -f *.o ^.so


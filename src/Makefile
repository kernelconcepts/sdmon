# (c)2018 ogi-it, Ognian Tschakalov

VERSION = 0.01
# CC is just set by the toolchain
#CC      = /usr/bin/gcc
CFLAGS  = -Wall -g -D_REENTRANT -DVERSION=\"$(VERSION)\"
LDFLAGS =

OBJ = sdmon.o
BIN = sdmon

$(BIN): $(OBJ)
	$(CC) $(CFLAGS) -o $(BIN) $(OBJ) $(LDFLAGS)

%.o: %.c
	$(CC) $(CFLAGS) -c $<

.PHONY: clean
clean:
	rm -rf $(BIN) $(OBJ)

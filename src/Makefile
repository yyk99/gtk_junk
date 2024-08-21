#
#
#

all: f1
	@echo Done
	
clean:
	rm -f f1
	
f1:	f1.c
	gcc f1.c -o f1 `pkg-config --cflags --libs gtk+-2.0`

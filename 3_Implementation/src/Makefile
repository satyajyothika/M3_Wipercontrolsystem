CC = arm-none-eabi-gcc
MACH = cortex-m4
CFLAGS = -c -mcpu=$(MACH) -mthumb -std=gnu11 -Wall -O0
all:wiper.o wiper1.o output.elf

wiper.o:wiper.c
	$(CC) $(CFLAGS) -o $@ $^
	
wiper1o:wiper1.c
	$(CC) $(CFLAGS) -o $@ $^

output.elf: wiper.o  wiper1.o
	$(CC)  -o $@ $^		
	
clean:
	rm -rf *.o *.elf

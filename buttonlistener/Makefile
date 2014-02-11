CXX = gcc
CFLAGS = -fPIC

buttonlistener.pd_linux: buttonlistener.o
	ld $(CFLAGS) -export-dynamic -shared -o buttonlistener.pd_linux buttonlistener.o -lc -lm -lwiringPi

buttonlistener.o: buttonlistener.c
	$(CXX) -c buttonlistener.c -o buttonlistener.o

clean:
	rm *.pd_linux
	rm *.o

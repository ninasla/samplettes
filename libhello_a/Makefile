CXX=g++
CFLAGS=-Wall -Wextra -pedantic -std=c++11

all: main

main: main.cpp libhello.a
	$(CXX) $(CFLAGS) main.cpp -L. -lhello -o main

libhello.a: hello.cpp
	$(CXX) $(CFLAGS) -c hello.cpp
	ar rcs libhello.a hello.o

clean:
	rm -f main libhello.a hello.o

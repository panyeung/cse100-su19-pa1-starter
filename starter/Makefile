# A simple makefile for CSE 100 P1

#use g++ for everything
CC= g++  	

# include debugging symbols in object files,
# and enable all warnings
CXXFLAGS= -g -Wall -std=c++11

#include debugging symbols in executable
LDFLAGS= -g	

default: test_bst test_kdt test_kdt2

test_bst: test_BST.o 
	g++ -o test_bst test_BST.o

test_kdt: test_KDT.o
	g++ -o test_kdt test_KDT.o

test_kdt2: test_KDT_2.o
	g++ -o test_kdt2 test_KDT_2.o

test_BST.o: BST.hpp BSTNode.hpp BSTIterator.hpp 
test_KDT.o: KDT.hpp BST.hpp BSTNode.hpp BSTIterator.hpp 
test_KDT_2.o: KDT.hpp BST.hpp BSTNode.hpp BSTIterator.hpp 


clean:
	$(RM) test_bst test_kdt test_kdt2 *.o

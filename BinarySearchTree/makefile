CC = g++
LFLAGS = -std=c++11
CFLAGS = -c -Wall

# Edit the following two lines when compiling
# EXECUTABLE_NAME is the name of the program to run
# SOURCES should include all the .cpp files to compile
EXECUTABLE_NAME = BinarySearchTree
SOURCES = main.cpp PrecondViolatedExcep.cpp NotFoundException.cpp BinaryNode.cpp BinaryNodeTree.cpp BinarySearchTree.cpp

OBJECTS = $(SOURCES:.cpp=.o)

all: $(EXECUTABLE_NAME)

$(EXECUTABLE_NAME): $(OBJECTS) 
	$(CC) -o $(EXECUTABLE_NAME) $(OBJECTS)

.cpp.o:
	$(CC) $(CFLAGS) $(LFLAGS) $< -o $@

clean:
	$(RM) *.o *~ $(EXECUTABLE_NAME)

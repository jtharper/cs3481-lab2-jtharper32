CXX = g++
CXXFLAGS = -c -Wall -g -std=c++11 -I ../include

INC = ../include
BIN = ../bin

OBJS = sortProg.o Sort.o BubbleSort.o MergeSort.o QuickSort.o List.o

TARGET = sortProg

$(TARGET): $(OBJS)
	$(CXX) $(OBJS) -o $(TARGET)

%.o: %.C $(INC)/Sort.h $(INC)/BubbleSort.h $(INC)/MergeSort.h $(INC)/QuickSort.h $(INC)/List.h
	$(CXX) $(CXXFLAGS) $< -o $@

install: $(TARGET)
	mkdir -p $(BIN)
	mv $(TARGET) $(BIN)/

clean:
	rm -f $(OBJS)

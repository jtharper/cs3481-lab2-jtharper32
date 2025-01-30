CXX = g++
CXXFLAGS = -c -Wall -g -std=c++11

OBJS = makeAnimals.o Animal.o Dog.o

TARGET = makeAnimals

$(TARGET): $(OBJS)
	$(CXX) $(OBJS) -o $(TARGET)

%.o: %.C
	$(CXX) $(CXXFLAGS) $< -o $@
clean:
	rm -f $(OBJS) $(TARGET)

CXX = g++
CXXFLAGS = -c -Wall -g -std=c++11

OBJS = makeNumber.o Number.o

TARGET = makeNumber

$(TARGET): $(OBJS)
	$(CXX) $(OBJS) -o $(TARGET)

%.o: %.C
	$(CXX) $(CXXFLAGS) $< -o $@
clean:
	rm -f $(OBJS) $(TARGET)

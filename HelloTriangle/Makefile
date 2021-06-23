CFLAGS = -std=c++17 -O2
LDFLAGS = -lglfw -lvulkan -ldl -lpthread -lX11 -lXrandr

HelloTriangle: main.cpp
	g++ $(CFLAGS) -o HelloTriangle.out main.cpp $(LDFLAGS)

.PHONY: test clean

test: HelloTriangle
	./HelloTriangle.out

clean:
	rm -f HelloTriangle.out 
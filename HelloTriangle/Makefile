CFLAGS = -std=c++17 -O2
RFLAGS = -std=c++17 -O3
LDFLAGS = -lglfw -lvulkan -ldl -lpthread -lX11 -lXrandr

HelloTriangle: main.cpp
	cd shaders/	&& ./compile.sh
	g++ $(RFLAGS) -o HelloTriangle.out main.cpp $(LDFLAGS)

.PHONY: test clean

test: HelloTriangle
	./HelloTriangle.out

clean:
	rm -f HelloTriangle.out 
CXX = gcc

LIB = -L/usr/local/lib -Wl,-rpath=/usr/local/lib \
	-L${VULKAN_SDK_PATH}/lib \
	-lSDL2_test \
	-lSDL2 \
	-lvulkan \

INCLUDE = -I/usr/local/include \
		-I${VULKAN_SDK_PATH}/include \

CXXFLAGS = -Wall -c $(INCLUDE)
LDFLAGS = $(LIB)
EXE = minimal-sdl2-vulkan

all: $(EXE)

$(EXE): main.o
	$(CXX) $< $(LDFLAGS) -o $@

main.o: minimal-sdl2-vulkan.c
	$(CXX) $(CXXFLAGS) $< -o $@

clean:
	rm *.o && rm $(EXE)

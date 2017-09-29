# learning-vulkan-through-sdl2
I'm trying to learn Vulkan graphics API.

- download, build and install latest SDL2 2.0.6 from libsdl.org
- download, extract, and configure vulkan sdk from lunarg.com/vulkan-sdk/ 
  bash configuration is something like
```
	export VULKAN_SDK=/home/user/VulkanSDK/1.0.61.1/
	export VULKAN_SDK_PATH=$VULKAN_SDK/x86_64
	export PATH=$PATH:$VULKAN_SDK/x86_64/bin
	export LD_LIBRARY_PATH=$VULKAN_SDK/x86_64/lib
	export VK_LAYER_PATH=$VULKAN_SDK/x86_64/etc/explicit_layer.d
```

- update your graphics driver
- cd minimal-sdl2 && make && ./minimal-sdl2-vulkan
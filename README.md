### New VCPKG Project

```shell
$ update-vcpkg
$ mkdir imgui-Tutorial && cd imgui-Tutorial
$ vcpkg add port imgui[docking-experimental,glfw-binding,vulkan-binding]
```

### Copy & Edit Files

- [`.gitignore`](https://www.toptal.com/developers/gitignore): add `build` directory
- [`CMakeLists.txt`](https://github.com/mkohlhaas/vcpkg-Tutorial/blob/main/helloworld/CMakeLists.txt): minor changes
- [`CMakePresets.json`](https://github.com/mkohlhaas/vcpkg-Tutorial/blob/main/helloworld/CMakePresets.json): no change
- [`main.cpp`](https://github.com/ocornut/imgui/blob/master/examples/example_glfw_vulkan/main.cpp): no change
- [`.clang-format`](https://github.com/mkohlhaas/Template-Metaprogramming-with-CPP/blob/main/.clang-format): no change

### Build

```shell
$ cmake --preset=default
$ cmake --build build/
$ ./build/HelloImgui
```

### Links

- [vcpkg Tutorial](https://github.com/mkohlhaas/vcpkg-Tutorial)
- [Dear ImGui](https://github.com/ocornut/imgui)
- [How to use vcpkg features (special syntax)](https://learn.microsoft.com/en-us/vcpkg/concepts/default-features#default-features-interactions)
- [gitignore.io](https://www.toptal.com/developers/gitignore)

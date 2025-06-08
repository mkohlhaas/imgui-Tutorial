### New VCPKG Project

```shell
$ update-vcpkg
$ mkdir helloworld && cd helloworld
$ mkdir imgui-Tutorial
$ cd imgui-Tutorial
$ vcpkg add port imgui[docking-experimental,glfw-binding,vulkan-binding]
```

### Copy & Edit Files

- `.gitignore` from https://www.toptal.com (add `build` directory)
- `CMakeLists.txt` from https://github.com/mkohlhaas/vcpkg-Tutorial/blob/main/helloworld/CMakeLists.txt (minor changes)
- `CMakePresets.json` from https://github.com/mkohlhaas/vcpkg-Tutorial/blob/main/helloworld/CMakePresets.json (no change)
- `main.cpp` from https://github.com/ocornut/imgui/blob/master/examples/example_glfw_vulkan/main.cpp (no change)

### Build

```shell
$ cmake --preset=default
$ cmake --build build/
$ ./build/HelloImgui
```

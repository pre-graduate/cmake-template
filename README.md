
<img src='preview.gif' /> 

<img src='icon.png' width='150' height='150' align='right' />

# CMake Template

This is a personal template for CMake based C++ projects. It sets out a layout which forces a good project structure including making dependencies external, samples and unit tests enabled by default. Changes may happen in future but this repository represents a good start for a C++ based project.

## Building Windows

Note build directory can be any name you want.

```cmd
mkdir build 
cd build
cmake ../
cmake --build .
```

## Testing

Release/Debug depending on your build.

```cmd
ctest -C Release
ctest -C Debug
```
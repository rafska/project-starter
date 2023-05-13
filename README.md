# project-starter

To build the project, checkout the repository and run
```bash
conan install . --output-folder=build --build=missing
cd build/
cmake .. -DCMAKE_TOOLCHAIN_FILE=conan_toolchain.cmake -DCMAKE_BUILD_TYPE=Release
cmake --build . --config Release
```
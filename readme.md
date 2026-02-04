

# vcpkg + CMake Template (Linux)

A **minimal, modern template** for building C++ projects using **vcpkg (manifest mode)**, **CMake Presets**, and **Ninja** on Linux.
##  Project Structure

```
.
├── CMakeLists.txt
├── CMakePresets.json
├── CMakeUserPresets.json   # optional, user-local overrides
├── vcpkg.json
├── vcpkg-configuration.json
├── src/
│   └── main.cpp
└── build/
```



## Adding  dependencies

```bash 
vcpkg install <package_name>
vcpkg add port <package_name>
```

---
## Build & Run

### Configure (installs dependencies automatically)

```bash
cmake --preset default
```

### Build

```bash
cmake --build build
```

### Run

```bash
./build/hello
```

---



## Clean Build

```bash
rm -rf build
cmake --preset default
```

---


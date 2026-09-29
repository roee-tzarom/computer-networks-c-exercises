# C Toolchain Starter

A compact C11 project for checking a compiler, linker and CMake setup. The program has one entry point and prints `Hello, World!`.

## Why keep this project?

Before working on larger native programs, it is useful to have a known-good build target. This repository is that baseline: `main.c` contains the complete program and `CMakeLists.txt` describes how to compile it. There are no libraries to install, configuration files to prepare or services to start.

## Build and run

You need a C compiler and CMake 4.1 or newer, as required by the current `CMakeLists.txt`.

```bash
cmake -S . -B build
cmake --build build
```

Run the generated `untitled` executable from the build directory (`untitled.exe` on Windows). The exact location depends on the CMake generator. A successful run prints one line:

```text
Hello, World!
```

## Repository map

| File | Purpose |
| --- | --- |
| `main.c` | Application entry point and terminal output |
| `CMakeLists.txt` | C11 build configuration and executable target |

This is a toolchain starter, not a network protocol implementation. For socket and protocol work, see the [TCP sliding-window transfer](https://github.com/roee-tzarom/computer-networks-python-exercises) and [reliable UDP network simulator](https://github.com/roee-tzarom/reliable-udp-network-simulator).

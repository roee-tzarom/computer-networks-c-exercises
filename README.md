# C Toolchain Starter

A minimal C/CMake exercise used to verify a working compiler and build setup. The current program in `main.c` prints `Hello, World!`; no socket or networking code is present yet.

## Build and run

```bash
cmake -S . -B build
cmake --build build
```

Run the generated executable from `build/` (`main` on Unix-like systems or `main.exe` on Windows, subject to the CMake generator). This repository is a starter project rather than a completed networking application.


## Repository walkthrough

`main.c` is the complete application entry point. The CMake configuration declares the executable and delegates compiler-specific build files to CMake. This is useful for checking that a C compiler, linker and CMake installation are working before starting larger socket assignments. There is no dependency manager, runtime configuration or input file.

## A reproducible check

After building, run the executable and expect a single `Hello, World!` line. If the build fails, check the C compiler selected by CMake and the generator-specific location of the executable. The `build/` directory is generated output and can be recreated with the commands above.

## Scope and next steps

Despite the repository name, this snapshot contains a toolchain starter only. It does not open sockets, implement a protocol, or include a test suite. For actual networking code in this GitHub account, see the [Python TCP sliding-window exercise](https://github.com/roee-tzarom/computer-networks-python-exercises) and [network simulator](https://github.com/roee-tzarom/reliable-udp-network-simulator). Keeping that distinction explicit makes the repository easier to evaluate accurately.

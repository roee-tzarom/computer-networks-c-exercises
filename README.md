# C Toolchain Starter

A minimal C/CMake exercise used to verify a working compiler and build setup. The current program in `main.c` prints `Hello, World!`; no socket or networking code is present yet.

## Build and run

```bash
cmake -S . -B build
cmake --build build
```

Run the generated executable from `build/` (`main` on Unix-like systems or `main.exe` on Windows, subject to the CMake generator). This repository is a starter project rather than a completed networking application.

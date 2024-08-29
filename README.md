# Lightweight "Native" Runtime for Ada GNAT
This is a lightweight runtime for Ada GNAT, designed for "native" platforms like Linux but without OS support. It provides minimal features for scenarios where a full native runtime is unnecessary or undesired, such as in kernel development.

## Project Structure

- Light Ada Runtime: `./`
- Example code and Makefile to test this runtime: `./example`

## Usage
Note: known to build for x86-64 using the latest Alire GNAT compiler (Linux)

### Building the Runtime

1. Ensure you have the GNAT compiler installed and properly set up.
2. Navigate to the project root directory.

```bash
gprbuild runtime_build.gpr
```

### Test the runtime

```bash
cd example
make
./main
```

### Useage in your own project, my_main.adb
```
gnatmake my_main.adb --RTS=/path/to/rts-native-light/
```

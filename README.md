# Light x86-64 Runtime for Ada GNAT

This is a lightweight runtime for Ada GNAT, x86-64, no OS. It provides a minimal set of features for scenarios where a full native runtime is not necessary or desired, such x86-64 kernel development.


## Project Structure

- Light x86-64 Ada Runtime: `./`
- Example code and Makefile to test this runtime: `./example`

## Usage

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
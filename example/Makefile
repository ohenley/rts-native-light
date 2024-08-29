# Variables
GNATMAKE = gnatmake
RTS_PATH = ../../rts-native-light
SRC = main.adb
TARGET = main

# Default rule
all: $(TARGET)

# Compile rule
$(TARGET): $(SRC)
	$(GNATMAKE) $(SRC) --RTS=$(RTS_PATH)

# Clean rule
clean:
	rm -f $(TARGET) *.o *.ali

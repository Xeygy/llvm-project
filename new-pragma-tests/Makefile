CC = clang
CFLAGS = -fopenmp -L/usr/lib/llvm-18/lib
OUTPUT = hw

all: $(OUTPUT).out
ll: $(OUTPUT).ll

$(OUTPUT).out: $(OUTPUT).c
	$(CC) $(CFLAGS) $< -o $@

$(OUTPUT).ll: $(OUTPUT).c
	$(CC) $(CFLAGS) -S -emit-llvm $< -o $@

clean:
	rm -f $(OUTPUT).out $(OUTPUT).ll


# MemoryAlloc - Custom Linux Heap Memory Manager

MemoryAlloc is a custom heap memory manager developed in C for Linux environments. This project aims to provide efficient memory allocation, deallocation, and reallocation functions, along with debugging tools to track memory leaks and usage patterns.

## Features

- Efficient memory allocation, deallocation, and reallocation functions.
- Debugging tools to track memory leaks and monitor memory usage.
- Enhanced understanding of low-level memory management and operating system concepts.

## Tech Stack

- **Programming Language**: C
- **Environment**: Linux

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/MemoryAlloc.git
    ```
2. Navigate to the project directory:
    ```sh
    cd MemoryAlloc
    ```
3. Compile the project:
    ```sh
    make
    ```

## Usage

To use the MemoryAlloc library in your project, include the `memory_alloc.h` header file and link against the compiled library.

Example:
```c
#include "memory_alloc.h"

int main() {
    // Allocate memory
    void *ptr = malloc_custom(100);
    if (ptr == NULL) {
        fprintf(stderr, "Memory allocation failed\n");
        return 1;
    }

    // Use the allocated memory

    // Free the allocated memory
    free_custom(ptr);

    return 0;
}

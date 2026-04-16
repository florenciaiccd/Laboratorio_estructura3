# HashMap Lab (C)

## Project Overview
A C programming laboratory for implementing a HashMap (Hash Table) data structure. The project uses linear probing for collision resolution and supports dynamic resizing.

## Structure
- `hashmap.h` — Defines `Pair` and `HashMap` structs and the public API
- `hashmap.c` — Core HashMap implementation (student exercises)
- `main.c` — Word counter demo using the HashMap
- `test.c` / `test.sh` — Test suite to validate the implementation
- `README.md` — Lab instructions (in Spanish)

## Build & Run
```bash
# Compile and run the demo
gcc main.c hashmap.c -o main -lm && ./main

# Run tests
bash test.sh
```

## Workflow
The "Start application" workflow compiles and runs `main.c` with the hashmap implementation.

## Notes
- `hashmap.c` contains stub functions for students to implement (do not modify stubs)
- Functions to implement: `createMap`, `insertMap`, `searchMap`, `eraseMap`, `firstMap`, `nextMap`, `enlarge`
- Uses linear probing for collision resolution
- Lazy deletion: erased pairs have `key = NULL` but the slot remains

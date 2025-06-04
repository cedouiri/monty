
# Monty - Bytecode Interpreter

## Description

**Monty** is a simple interpreter for Monty ByteCode files.  
Monty ByteCode is a scripting language that operates on a stack or a queue.  
The interpreter reads Monty bytecode instructions line by line and executes them.  
This project was developed as part of the Holberton School system programming curriculum.

## Features

- Stack and queue implementation using doubly linked lists
- Opcodes supported: `push`, `pall`, `pint`, `pop`, `swap`, `add`, `nop`, etc.
- Error handling for invalid instructions or missing arguments
- Line-by-line file parsing
- Memory management and clean exit on failure
- Support for both stack (LIFO) and queue (FIFO) modes

## How to Use

### Compilation

```
gcc -Wall -Werror -Wextra -pedantic *.c -o monty
```

### Run the Interpreter

```
./monty bytecode_file.m
```

### Example

Contents of `bytecode_file.m`:

```
push 1
push 2
push 3
pall
```

Execution:

```
$ ./monty bytecode_file.m
3
2
1
```

## Files

| File            | Description                                      |
|-----------------|--------------------------------------------------|
| `monty.c`       | Main file and entry point                        |
| `opcode.c`      | Execution of bytecode instructions               |
| `stack_ops.c`   | Stack manipulation functions                     |
| `utils.c`       | Helper functions                                 |
| `free.c`        | Memory freeing and cleanup                       |
| `bytecode.m`    | Example Monty bytecode script                    |

## Requirements

- OS: Ubuntu 20.04 LTS
- GCC compiler

## Skills Learned

- C programming
- Data structures (stack, queue)
- File parsing
- Error handling
- Memory management

## Authors

- [Chamsseddine Douiri](https://github.com/cedouiri)

## License

This project is licensed under the MIT License.

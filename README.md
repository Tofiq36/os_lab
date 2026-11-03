# Operating Systems Lab

This repository contains a collection of beginner-to-intermediate Operating Systems lab exercises implemented in shell scripts and C programs. The programs cover core OS concepts such as file handling, process management, memory usage, CPU-bound and I/O-bound tasks, and basic shell scripting.

## Overview

The lab exercises in this project demonstrate:

- Shell scripting basics and decision-making
- File and directory checks
- User login and active session monitoring
- Text processing with `sed` and `awk`
- String length and substring operations
- Dynamic memory allocation
- Process creation with `fork()` and `wait()`
- CPU-intensive vs I/O-intensive workloads
- PID and process behavior monitoring

## Repository Structure

- `exp3a.sh` — checks whether a given path is a file, directory, or invalid input
- `exp3b.sh` — renames files by converting filenames to uppercase
- `exp4a.sh` — shows currently logged-in users and calculates their working duration
- `exp4b.sh` — prints a range of lines from a file
- `exp4c.sh` — removes lines containing a given word from one or more files
- `exp5.sh` — gets string length and extracts a substring from user input
- `exp5.c` — C version of the string length and substring program
- `exp6.c` — allocates a user-specified amount of memory and keeps it alive
- `exp7a` / `exp7a.c` — CPU-bound process loop
- `exp7b` / `exp7b.c` — I/O-bound process loop writing to a file repeatedly
- `exp9.c` — demonstrates `fork()` and parent waiting for child termination
- `exp10` / `exp10.c` — prints process ID and memory address, then sleeps forever

## How to Run

### Shell scripts

```bash
chmod +x exp3a.sh exp3b.sh exp4a.sh exp4b.sh exp4c.sh exp5.sh
./exp3a.sh /tmp
./exp3b.sh file1.txt file2.txt
./exp4a.sh
./exp4b.sh sample.txt 5 20
./exp4c.sh hello sample.txt notes.txt
./exp5.sh
```

### C programs

Compile and run the C programs with `gcc`:

```bash
gcc exp5.c -o exp5
./exp5

gcc exp6.c -o exp6
./exp6 64

gcc exp7a.c -o exp7a
./exp7a

gcc exp7b.c -o exp7b
./exp7b

gcc exp9.c -o exp9
./exp9

gcc exp10.c -o exp10
./exp10
```

## Notes

These exercises are intended for academic learning and follow common operating systems lab assignments. They are useful for understanding process states, shell scripting, and resource behavior at a practical level.

## License

This project is provided for educational use within the OS lab curriculum.

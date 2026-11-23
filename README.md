# Operating Systems Utilities and Simulators — COMP 3430

This individual coursework suite covers executable inspection, process/thread management, scheduling simulation, synchronization, and FAT32 filesystem analysis in C on Linux.

> **Coursework publication boundary:** this repository is a verified case study. Raw assignment source and supplied course artifacts are intentionally withheld to avoid publishing reusable assignment solutions.

## Projects

### ELF parser and worker herders

- Parses 64-bit ELF headers, program headers, and section information
- Runs configurable process and pthread worker groups
- Responds to signals for resizing and clean shutdown

### MLFQ scheduler simulator

- Simulates a multilevel feedback queue with pthread CPU workers
- Coordinates shared queues and timing data with synchronization
- Reports turnaround and response time by task type

### FAT32 reader

- Reads boot-sector and FSInfo metadata
- Recursively lists files and directories
- Extracts files from a supplied FAT32 image

## Fresh verification

During the November 2026 hosting pass:

- all three assignments rebuilt with strict warning flags;
- the ELF parser reported the supplied 64-bit executable structure;
- the MLFQ simulator completed a four-CPU workload and printed timing results;
- the FAT32 reader reported volume information; and
- the FAT32 recursive listing produced 1,024 lines.

See [`evidence/verification.txt`](evidence/verification.txt) for the concise verification record.

## Stack

- C11
- Linux/POSIX
- processes, signals, and pthreads
- synchronization and scheduling
- ELF and FAT32 data structures

## Demo availability

No browser demo is provided because the projects are command-line systems programs. The README and verification record provide the public demonstration.

## Portfolio

[View the suite in my portfolio](https://damilola-durodola.vercel.app/#operating-systems-utilities)

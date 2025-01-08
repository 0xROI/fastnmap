# Fast Port Scanning Wrapper for Nmap (Written in C)

This project is a **C-based wrapper** for `nmap` that performs fast port scanning. The tool runs an initial scan to find open ports and then performs an aggressive scan on those open ports. The program is **statically compiled**, meaning all required libraries are included in the binary itself, making it portable across different Linux-based systems.

## Features
- **TCP** and **UDP** port scan support using `nmap`.
- Performs an **initial fast scan** to detect open ports quickly.
- Runs an **aggressive scan** on detected open ports for detailed information.
- **Static compilation** ensures the binary runs independently of system libraries.
- Saves the output in a file with a timestamp for easy tracking.

## Requirements
- **GCC** (GNU Compiler Collection) installed for compiling the source code.
- **nmap** installed on the system to perform the actual port scanning.
- Linux-based environment to run the compiled tool.

## How to Compile

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/nmap-scan-tool.git
   cd nmap-scan-tool
   gcc -static -o nmap_scan_wrapper nmap_scan_wrapper.c

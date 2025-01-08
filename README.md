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
   git clone https://github.com/0xROI/fastnmap
   gcc -static -o fastnmap fastnmap.c
##User Manual
`./nmap_scan_wrapper <target-ip> [tcp|udp]`
For a TCP scan:
`./nmap_scan_wrapper 192.168.1.1 tcp`
For a UDP scan:
`./nmap_scan_wrapper 192.168.1.1 udp`
Output:
`nmap_<scan-type>_scan_<target-ip>_<timestamp>.txt`

##Download the Binary
You can download the statically compiled binary from the latest release here: [https://github.com/0xROI/fastnmap/raw/refs/heads/main/fastnmap
](download)
##Acknowledgements
This project utilizes nmap for network scanning. Refer to the nmap documentation for more [https://nmap.org/](details).

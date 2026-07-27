# Python Port Scanner

A Python command-line application that scans the TCP ports of a specified host and reports which ports are open.

This project was originally developed as part of the Python Programming for Security Analysis and Penetration Testing course in Spring 2022. In 2026, it was refactored and expanded as a portfolio project to demonstrate Python programming, socket programming, networking fundamentals, clean code practices, and exception handling.

---

## Overview

This application uses Python's built-in `socket` module to attempt a TCP connection to each port on a target host. If a connection is successfully established, the port is reported as open.

The scanner iterates through the standard TCP port range (1–65535) and provides a simple way to explore how network services are exposed on a host.

**This program is intended for educational purposes and should only be used on systems that you own or have explicit permission to test.**

---

## Features

- Scans TCP ports 1–65535
- Reports open ports
- Uses Python socket programming
- Handles user interruption (Ctrl+C)
- Handles connection and hostname errors
- Simple command-line interface

---

## Technologies

- Python 3
- socket module
- Exception handling
- Command-line programming

---

## How to Run

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/python-port-scanner.git
```

Run the program:

```bash
python portScanner.py
```

Enter the IP address or hostname when prompted.

Example:

```
What IP do you want me to scan?
192.168.1.1
```

---

## Example Output

```
Hello, I am a port scanner. Use me wisely.
------------------------------------------

What IP do you want me to scan?
192.168.1.1

Port 22 is open
Port 80 is open
Port 443 is open

Scan complete.
```

---

## Skills Demonstrated

- Python programming
- TCP/IP networking fundamentals
- Socket programming
- Exception handling
- Command-line application development
- Network service discovery

---

## Future Improvements

Potential enhancements include:

- Custom port ranges
- Multithreaded scanning
- Configurable timeout values
- Service name detection
- Banner grabbing
- Saving results to a file
- Progress indicator
- Command-line arguments using `argparse`

---

## Educational Use

This project was created to learn networking concepts and Python socket programming. It is intended to be used only on systems that you own or are explicitly authorized to test.

---
## Version

**Version 2.0** (July 2026)

### Improvements from the original release

- Refactored and cleaned up the code
- Improved documentation
- Added a professional README
- Updated the project for portfolio presentation

---

## License

This project is licensed under the MIT License.

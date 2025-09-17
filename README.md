# PortScanner (Java) – My Custom Version

This is **my own implementation of a TCP port scanner** in Java.  
I built it to explore **network programming, multi-threading, and performance optimization**.  
It scans a range of TCP ports on a specified host and reports which ones are open.

---

## Why I Made This
I wanted a simple yet efficient way to check open ports for **learning purposes** and to understand, as a Software Engineering student interested in cybersecurity, how **sockets and threads work in Java**.  
This is **not for scanning networks without permission** — only test it on your own machines.

---

## Features
- Scan any TCP port range (default: 1–1024)  
- Configurable connection timeout (default: 300ms)  
- Multi-threaded scanning for faster results (default: 200 threads)  
- Prints open ports in ascending order  

---

## How to Use

1. **Compile the program**:

```bash
javac PortScanner.java
2. Run the scanner:

java PortScanner <host> [startPort] [endPort] [timeoutMs] [threads]


Parameters explained:

host → the IP or hostname to scan

startPort → first port in the range (optional, default: 1)

endPort → last port in the range (optional, default: 1024)

timeoutMs → connection timeout in milliseconds (optional, default: 300)

threads → number of concurrent threads (optional, default: 200)

Example run:

java PortScanner 127.0.0.1 1 1024 300 200

Example Output
Open TCP ports:
  - 22
  - 80
  - 443
Scan completed in 1245 ms

My Notes

Only scan machines you own or have explicit permission to scan.

I made this to learn Java concurrency and socket programming as a Software Engineering student interested in cybersecurity.

Works best with Java 8 or higher.

License

This is my personal project. Feel free to study and modify for learning purposes, but always use responsibly.

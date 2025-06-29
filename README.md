# Watchdog

Watchdog is a lightweight Python-based Windows process monitor that detects suspicious running processes in real-time. It flags unsigned executables and processes using unusually high CPU or memory, helping identify potential malware or unwanted software quickly.

---

## Features

- Enumerates all running Windows processes.
- Checks if executables are digitally signed.
- Flags unsigned processes as suspicious.
- Detects processes with high CPU or memory usage.
- Prints a summary of suspicious processes detected.
- Designed for quick local system auditing.

---

## Requirements

- Windows OS
- Python 3.x
- `psutil` Python library

Install dependencies:

```bash
pip install psutil
Usage
Run Watchdog via command line:

bash
Kopírovať
Upraviť
python watchdog.py
The script outputs suspicious processes with details:

Process ID (PID)

CPU usage percentage

Memory usage

Executable path

Signature status (Signed/Unsigned)

How Watchdog Works
Watchdog scans all active processes, checking their executable files for a valid digital signature. Processes that are unsigned or exceed CPU/memory usage thresholds are flagged as suspicious. This helps quickly identify unknown or potentially malicious processes on your system.

Important Legal & Ethical Notice
Reporting Only: Watchdog only reports suspicious processes; it does not remove, modify, or interfere with any software or processes.

Ethical Use: You must use Watchdog responsibly and ethically. Use it

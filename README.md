
# 🔍 Network Port Scanner GUI

A powerful and user-friendly GUI-based Network Port Scanner built using Python and Tkinter. This tool allows users to scan open ports on a target IP address or hostname and identify active services in real-time.

## 🚀 Features
Scan ports for any IP address or domain
Real-time progress tracking with progress bar
Displays open ports with detected services (HTTP, FTP, SSH, etc.)
Start/Stop scan functionality
Save scan results to a file

## Requirements

- Python 3.7 or newer
- Tkinter (included in the standard Python distribution; on Debian/Ubuntu install `python3-tk`)

No third-party packages are required.

## Installation

```bash
git clone https://github.com/sakshigadilkar01/NetworkPortscanner.git
cd NetworkPortScanner
```

## Usage

```bash
python portscanner.py
```

1. Enter the **Target** – an IP address (e.g. `192.168.1.1`) or hostname (e.g. `scanme.nmap.org`).
2. Set the **Start Port** and **End Port** (defaults: `1` – `1024`).
3. Click **Start Scan**. Open ports appear in real time in the results pane.
4. Click **Stop** to cancel a scan early.
5. After a scan completes, click **Save Results** to write the open-port list to a text file.

## Detected Services

The following ports are automatically labelled:

| Port | Service   |
|------|-----------|
| 21   | FTP       |
| 22   | SSH       |
| 23   | Telnet    |
| 25   | SMTP      |
| 53   | DNS       |
| 80   | HTTP      |
| 110  | POP3      |
| 143  | IMAP      |
| 443  | HTTPS     |
| 3306 | MySQL     |
| 3389 | RDP       |
| 5900 | VNC       |
| 8080 | HTTP-Alt  |

Ports not in the list are reported as `Unknown`.

## Project Structure

```
NetworkPortScanner/
├── portscanner.py   
└── README.md
```

# ⚠️ Disclaimer
This tool is intended for educational purposes only.
Do not scan networks or systems without proper authorization.

## License

This project is released under the [MIT License](https://opensource.org/licenses/MIT).

# 👩‍💻 Author
Sakshi Gadilkar

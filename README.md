![Alt text](logo.png?raw=true "Title")

Perform automated network reconnaissance scans to gather network intelligence.

IntelSpy is a network intelligence spy tool which performs automated enumeration of network services. It performs live hosts detection scans, port scans, services enumeration scans, web content scans, brute-force, detailed off-line exploits searches and more. The tool will also launch further enumeration scans for each detected service using a number of different tools.

---

### Features

* Scans IP addresses and IP ranges (CIDR notation).
* Creates a directory structure for results gathering.
* Logs commands that were run.
* Extracts important information in txt and markdown format.
* Stores data to an SQLite database.

---

### Requirements

* Python 3
* colorama
* nmap

```
pip3 install -r requirements.txt
```

---

### Usage

```
usage: scan.py [-h] -t TARGET -st SCAN_TYPE -p PROJECT_NAME -w WORKING_DIR

optional arguments:
  -h, --help            show this help message and exit
  -t TARGET, --target TARGET
                        target IP or IP range
  -p PROJECT_NAME, --project-name PROJECT_NAME
                        project name
  -w WORKING_DIR, --working-dir WORKING_DIR
                        working directory
```

---

### Usage Examples

```
sudo python3 intelspy.py -t 192.168.10.0/24 -p MyProjectName -w /home/user/pt/projects/
```

---

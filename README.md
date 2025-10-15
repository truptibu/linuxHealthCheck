# 🩺 Linux System Health Check Report

## Project Objective
The goal of this project was to create a comprehensive system health report using only standard Linux command-line tools.
This exercise demonstrates proficiency in basic system administration and command-line utility usage for gathering vital machine statistics.

## 📁 Final Report Structure
The final report is aggregated within a directory and then compressed. The `system_report/` directory contains individual files detailing different aspects of the system's health.

| Filename | Content | Command Used |
| :--- | :--- | :--- |
| `date_time.txt` | Current date and time | `date` |
| `system_info.txt` | Kernel version and architecture | `uname -a` |
| `memory_usage.txt` | Human-readable memory (RAM) statistics | `free -h` |
| `disk_usage.txt` | Human-readable disk space usage for all mounted filesystems | `df -h` |
| `top_processes.txt` | Top 10 running processes sorted by CPU utilization | `ps -eo ... | head -11` |
| `network_info.txt` | Network interface configuration and IP addresses | `ip a` |

The final output is the compressed archive: **`system_report.tar.gz`**.

## 🛠 Project Commands and Implementation Steps

The following steps were executed sequentially to generate the final report:

### Step 1: Setup and Environment Creation
```bash
# 1. Create the main report directory
mkdir ~/system_report

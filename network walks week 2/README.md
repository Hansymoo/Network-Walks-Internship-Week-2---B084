# W2-PM-FINAL: Footprinting & Network Scanning Report

Week 2 final project for the Cybersecurity & Ethical Hacking program at [Networkwalks](https://networkwalks.com).

This repository contains my penetration testing report covering two modules:

- **W2-PM2:** Footprinting & Reconnaissance with GHDB (Google Hacking Database)
- **W2-PM5:** Network Scanning with Zenmap

**Author:** Hans Miguel A. Abrera | Batch B084-Networkwalks
**LinkedIn:** [hans-miguel-abrera](https://www.linkedin.com/in/hans-miguel-abrera-2a371143b/)
**Date:** 14 November 2026

---

## What is in this repo

| File | Description |
| --- | --- |
| `W2-PM-FINAL_Penetration_Testing_Report.pdf` | The final report (PDF) |
| `W2-PM-FINAL_Penetration_Testing_Report.docx` | The final report (editable Word version) |
| `README.md` | This file |

---

## Summary

### W2-PM2: Footprinting with GHDB
I used Google dorks from exploit-db.com's GHDB, plus other dorks, to find publicly exposed content using only Google.

- **Task 1:** Found 10 live, exposed security cameras that opened without a username or password.
- **Task 2:** Found 10 open directory listings with downloadable mathematics PDFs.

### W2-PM5: Network Scanning with Zenmap
I ran a ping scan (`nmap -sn`) on my own local network, 192.168.1.0/24.

- **66 live hosts** found, with their MAC addresses and vendors.
- Several hosts matched a camera vendor (Hangzhou Hikvision).
- Exported the network topology with the legend enabled.
- Scored **100%** on the Zenmap Network Scanning practice lab quiz.

### Main findings
| Finding | Risk |
| --- | --- |
| Exposed live cameras with no authentication | Critical |
| Open directory listings | Medium |
| Sensitive pages indexed by Google | Medium |
| Many live hosts on the local network | Medium |
| Camera vendor devices on the same subnet | Medium |
| MAC addresses reveal device vendors | Low |

The report also lists recommendations, such as keeping cameras off the internet, changing default settings, turning off directory listing, and separating IoT devices onto their own VLAN.

---

## Tools used

- Google Search and GHDB (exploit-db.com)
- Insecam
- Zenmap (Nmap GUI)
- Windows CMD (`ipconfig`)

---

## Scope and ethics

- Scanning was done only on **my own network**.
- The footprinting work was done as part of the assigned Networkwalks lab. I only viewed publicly accessible pages. I did not log in, change settings, use credentials, or download or share any files.
- No exploitation or vulnerability scanning was performed in these modules.
- IP addresses of my own network are hidden in the screenshots.

---

## Disclaimer

This material is for education and research purposes only. Do not use anything from here to break the law. The instructor, the authors and Networkwalks are not responsible for what you do with this knowledge. Every action you take is your own responsibility. Misuse can lead to criminal charges, heavy fines, loss of your job and a permanent record. In most countries unauthorised access is a crime even when nothing is damaged.

Only test devices or networks that you own, or where you have written permission from the owner.

---

## Program

**Program:** Cybersecurity program at Networkwalks | **Week:** 02

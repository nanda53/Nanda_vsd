# 🖥️ RISC-V SoC – VSD Tapeout Program  


This repository documents the full setup process for the **VSD RISC-V  SoC Tapeout Program**,  
including my system specifications, installation steps for required open-source EDA tools,  
and a quick test example to verify your environment.

---

## 💻 My System Specifications
| Component | Details |
|----------|---------|
| **OS** | CachyOS (Arch Linux-based, performance-tuned) |
| **Kernel** | Linux-zen (optimized for low-latency desktop performance) |
| **CPU** | Intel® Core™ i7-12700H (12th Gen) – 14 cores / 20 threads |
| **RAM** | 16 GB |
| **Storage** | 512 GB NVMe SSD (50 GB allocated for this project) |
| **GPU** | NVIDIA GeForce RTX 3060 |


✅ This configuration runs Yosys, Icarus Verilog, and GTKWave smoothly in a VirtualBox VM.

---

## ✅ System Requirements (Recommended by VSD)
- **OS:** Linux (Ubuntu 20.04+ / Arch-based distros recommended)  
- **RAM:** 6 GB minimum (8 GB+ recommended)  
- **Storage:** 50 GB free disk space  
- **CPU:** 4 vCPUs or higher  

---

## 🔧 Setup (CachyOS / Arch-based Distros)

### 1️⃣ Update Packages
```bash
sudo pacman -Syu

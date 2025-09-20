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



## 🔧 Setup (CachyOS / Arch-based Distros)

## 🧰 TOOL CHECK

After installing all tools, run these commands to verify that everything is working correctly.

### 🔨 Yosys (Synthesis Tool)


     
    # Update your package database
    sudo pacman -Syu
    
    #  Install required build dependencies
    sudo pacman -S --needed base-devel git make clang bison flex \
      readline gawk tcl libffi graphviz xdot pkgconf boost zlib python
    
    # Clone Yosys source code
    git clone https://github.com/YosysHQ/yosys.git
    cd yosys
    
    # Configure for GCC
    make config-gcc
    
    #  Build
    make -j$(nproc)
    
    # Install system-wide
    sudo make install


<img width="1917" height="253" alt="Screenshot From 2025-09-20 18-26-34" src="https://github.com/user-attachments/assets/1522b516-8d85-41c0-9edb-f6770ba9aad6" />


### Iverilog:
      # Install Iverilog
      sudo pacman -S iverilog


<img width="1917" height="616" alt="Screenshot From 2025-09-20 18-52-31" src="https://github.com/user-attachments/assets/13b22887-ca7c-40e3-a527-7c6ba643968c" />


### gtkwave :

<img width="1912" height="76" alt="Screenshot From 2025-09-20 18-54-32" src="https://github.com/user-attachments/assets/d1beb2e5-5871-488b-9dde-2e69fe1a07f1" />









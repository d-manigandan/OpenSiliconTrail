# Week 0 – Task 0

## Objective
- Create GitHub repo for documentation  
- Check system requirements  
- Install all required tools for the RISC-V SoC Tapeout flow.

## System Specs
- RAM: 6 GB  
- Storage: 50 GB+  
- CPU: 4 vCPUs  
- OS: Ubuntu 20.04 

## Tools Installed
- **Yosys**
- **Icarus Verilog (iverilog)**
- **GTKWave**
- **Ngspice**
- **Magic**
- **OpenLANE** (with Docker)

## Installation Steps & Logs

### 1. Yosys
```bash
sudo apt-get update
git clone https://github.com/YosysHQ/yosys.git
cd yosys
sudo apt install make build-essential clang bison flex \
    libreadline-dev gawk tcl-dev libffi-dev git \
    graphviz xdot pkg-config python3 libboost-system-dev \
    libboost-python-dev libboost-filesystem-dev zlib1g-dev
make config-gcc
make
sudo make install

```
![Yosys Installation Screenshot](images/yosys.png)

### 2. Icarus Verilog
```bash
sudo apt-get install iverilog
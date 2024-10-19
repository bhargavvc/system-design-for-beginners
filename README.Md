
Here is the system desing for beginers 
## Table of Contents

- [Computer Architecture Components](#computer-architecture-components)

- [Application Architecture](#application-architecture)
- [Design Requirements](#design-requirements)
- [Networking Basics](#networking-basics)
- [TCP vs UDP](#tcp-vs-udp)
- [DNS](#dns)
- [Application Protocols](#application-protocols)
- [API Paradigms](#api-paradigms)
- [API Designs](#api-designs)
- [Caching](#caching)
- [CDN (Content Delivery Network)](#cdn-content-delivery-network)
- [Proxies and Load Balancers](#proxies-and-load-balancers)
- [Hashing](#hashing)
- [SQL](#sql)
- [No-SQL](#no-sql)
- [Replication and Sharding](#replication-and-sharding)
- [Object Storage](#object-storage)
- [Message Queue](#message-queue)

This section provides an overview of key computer hardware components, including their definitions, uses, and technical specifications.

## Computer Architecture Components

 ![Computer Architecture](https://raw.githubusercontent.com/bhargavvc/system-design-for-beginners/main/images/computer_architecture.png)


### 1. Storage (Disk)
**Definition:**
- Disk storage is the primary, non-volatile storage used for permanently storing data and programs, even when the computer is turned off.

**Usage:**
- Stores operating systems, applications, and files (e.g., documents, images, videos).

**Specifications:**
- **Type:**
  - HDD (Hard Disk Drive): Traditional, slower, mechanical.
  - SSD (Solid State Drive): Faster, no moving parts, uses flash memory.
- **Capacity:** Measured in gigabytes (GB) or terabytes (TB) (e.g., 500GB, 1TB).
- **Speed:**
  - HDD: 5-10 milliseconds.
  - SSD: 0.1-1 milliseconds (much faster).

### 2. Memory (RAM)
**Definition:**
RAM (Random Access Memory) is temporary, volatile memory for storing data and instructions for quick access while the computer is running.

**Usage:**
- Used to store data that the CPU needs to access quickly for running active programs and processes.

**Specifications:**
- **Type:** DRAM (Dynamic RAM), SRAM (Static RAM).
- **Capacity:** Measured in gigabytes (GB) (e.g., 4GB, 16GB, 32GB).
- **Speed:** Access times around 10-100 nanoseconds.
- **Volatility:** Data is lost when power is turned off.


### 3. CPU (Central Processing Unit)
**Definition:**
- The CPU is the "brain" of the computer, responsible for executing instructions and performing calculations.

**Usage:**
- Executes commands from programs, processes data, and performs complex calculations.

**Specifications:**
- **Clock Speed:** Measured in gigahertz (GHz) (e.g., 3.0 GHz).
- **Cores:** Single-core, dual-core, quad-core (more cores allow multiple processes to run simultaneously).
- **Architecture:** 32-bit or 64-bit, affecting how much data the CPU can handle at once.


### 4. Cache
**Definition:**
- Cache is a small, high-speed memory located inside the CPU, used for storing frequently accessed data and instructions.

**Usage:**
- Acts as a buffer between RAM and the CPU, speeding up access to frequently used data.

**Specifications:**
- **Size:** Typically measured in megabytes (MB) (e.g., 2MB, 8MB, 16MB).
- **Levels:** L1 (smallest, fastest), L2, L3 (larger but slower).
- **Speed:** Extremely fast, with access times in nanoseconds.

### 5. Bus
**Definition:**
- A communication system that transfers data between components inside or between computers.

**Usage:**
- Transfers data between the CPU, memory (RAM), and other hardware devices.

**Specifications:**
- **Types:** Data bus, address bus, control bus.
- **Speed:** Measured in MT/s (Megatransfers per second).

### 6. GPU (Graphics Processing Unit)
**Definition:**
- A GPU is a specialized processor designed to accelerate the rendering of images, animations, and videos.

**Usage:**
- Primarily used for rendering graphics in gaming, video editing, and 3D rendering. Also used for parallel processing tasks like machine learning and scientific simulations.

**Specifications:**
- **Cores:** Hundreds to thousands of smaller cores for parallel processing.
- **Memory (VRAM):** Dedicated video RAM, measured in gigabytes (e.g., 4GB, 8GB, 16GB).
- **Clock Speed:** Measured in megahertz (MHz) or gigahertz (GHz).
- **Architecture:** Designed for handling large-scale parallel tasks, ideal for processing multiple threads.


### 7. Motherboard
**Definition:**
- The main circuit board that connects all components of a computer.

**Usage:**
- Houses the CPU, memory (RAM), storage, and other components. Facilitates communication between these parts.

**Key Specifications:**
- **Form Factor:** ATX, Micro ATX, Mini ITX.
- **Chipset:** Determines compatibility with CPUs and other components.
- **Ports & Slots:** PCIe slots for GPUs, RAM slots, SATA connectors for storage.


### 8. Power Supply Unit (PSU)
**Definition:**
- Converts AC power from the wall outlet into DC power that the computer components use.

**Usage:**
- Supplies power to the computer's components.

**Key Specifications:**
- **Wattage:** Total power output (e.g., 500W, 750W).
- **Efficiency Rating:** Indicates power conversion efficiency (e.g., 80 Plus Gold, Platinum).
- **Modular vs Non-Modular:** Determines cable management flexibility.


### 9. I/O Devices (Input/Output Devices)
**Definition:**
- Hardware used to input data into or output data from the computer.

**Usage:**
- Facilitates interaction between the computer and external devices.

**Key Types:**
- **Input Devices:** Keyboard, mouse, microphone.
- **Output Devices:** Monitor, printer, speakers.
- **Storage Devices:** Hard drives, SSDs, USBs.


### 10. Network Interface Card (NIC)
**Definition:**
- A hardware component that connects a computer to a network.

**Usage:**
- Allows communication over a network (e.g., Ethernet or Wi-Fi).

**Key Specifications:**
- **Speed:** 100 Mbps, 1 Gbps, 10 Gbps.
- **Type:** Wired (Ethernet) or wireless (Wi-Fi).

### 11. BIOS/UEFI
**Definition:**
- BIOS (Basic Input/Output System) or UEFI (Unified Extensible Firmware Interface) is firmware that initializes hardware during booting.

**Usage:**
- Performs hardware checks during startup and provides a platform for the OS to boot.

**Key Specifications:**
- **BIOS:** Legacy system.
- **UEFI:** Modern alternative with features like support for larger drives and faster boot times.


### 12. Registers
**Definition:**
- Small, high-speed storage locations in the CPU that store data temporarily.

**Key Types:**
- **Accumulator:** Holds intermediate results of calculations.
- **Instruction Register (IR):** Holds the current instruction being executed.
- **Program Counter (PC):** Holds the memory address of the next instruction to be executed.

---

# Hello, everyone!

I’m Polar Bear‑Engineer from «RV Polar Bear», and today I’m excited to present our flagship development kits: **PBKit 501‑A** and **PBKit 501‑A‑Base**.

![pc_br.jpg](pc_br.jpg)

These platforms redefine the boundaries of embedded computing — engineered for mission‑critical AI, ultra‑high‑bandwidth IoT, and real‑time industrial control. Expect unmatched performance, future‑proof connectivity, and rock‑solid reliability.

## What Are PBKit 501‑A and PBKit 501‑A‑Base?

**PBKit 501‑A** is a top‑tier mainboard powered by a cutting‑edge heterogeneous SoC (CPU + GPU + NPU + DSP). It’s built for:
- Edge AI/ML inference at 10+ TOPS;
- 8K video analytics and multi‑camera fusion;
- High‑frequency industrial control (sub‑ms jitter);
- Ruggedized deployments in extreme environments.

**PBKit 501‑A‑Base** is a complete turnkey platform: PBKit 501‑A + a feature‑dense base board. It adds:
- Redundant power and hot‑swap capability;
- Extended I/O for sensor farms and actuators;
- Integrated cooling and EMI shielding;
- Pre‑certified wireless modules (5G, Wi‑Fi 6E, GNSS).

## Key Features

### PBKit 501‑A

- **Processor**:  
  - Heterogeneous SoC: 8×Cortex‑A78 (2.5 GHz) + 2×Cortex‑R8 (real‑time) + Mali‑G710 MC9 GPU + 12 TOPS NPU + dual DSP;
  - Hardware virtualization and TEE (TrustZone).
- **Memory**:  
  - 16 GB LPDDR5 (7500 MT/s);  
  - 128 GB UFS 3.1;  
  - Optional 256 GB NVMe (via M.2).
- **Interfaces**:  
  - **Networking**: 2×10 Gbps Ethernet (SFP+), 1×25 Gbps (QSFP28), 5G/4G modem (M.2), Wi‑Fi 6E/Bluetooth 5.3;  
  - **Storage**: 2×M.2 Key M (NVMe), 1×microSD, 2×SATA III;  
  - **Display**: 2×HDMI 2.1 (8K@60 Hz), 2×DisplayPort 1.4, 4×MIPI‑DSI (4K);  
  - **Cameras**: 4×MIPI‑CSI‑2 (8 lanes each, 4.5 Gbps/lane), ISP (4×4K@60 fps);  
  - **Industrial I/O**: 8×CAN‑FD, 12×UART, 6×SPI, 6×I²C, 4×I²S, 8×12‑bit ADC (1 MSPS), 4×16‑bit DAC;  
  - **General I/O**: 64‑pin GPIO (1.8–3.3 V, 24 mA), 8×isolated digital inputs (24 V), 8×relay outputs (5 A@30 V);  
  - **Timing**: PPS input, TCXO (0.5 ppm), dual RTC.
- **AI Acceleration**: 12 TOPS NPU (INT8), support for TensorRT, ONNX, TFLite.
- **Operating Systems**:  
  - Linux (Yocto 4.2, Ubuntu 24.04, SELinux‑hardened);  
  - Android 14;  
  - QNX 8, VxWorks 7 (optional);  
  - Container support (Docker, Kubernetes).
- **Power**: 18–36 V DC, PoE++ (802.3bt), redundant input, battery backup.
- **Form Factor**: 140 × 100 mm (Eurocard‑compatible).
- **Environmental**: -40 °C to +85 °C, IP40, shock/vibe resistant.

### PBKit 501‑A‑Base


Includes **PBKit 501‑A** + **base board** with:
- Dual power supplies (hot‑swappable);
- Fanless phase‑change cooling;
- 4×additional SATA III ports;
- 2×additional M.2 slots (4G/5G, GNSS);
- Optical isolation on all digital I/O;
- Signal conditioning (anti‑aliasing, ESD protection);
- LED status matrix and debug probes;
- Mechanical mounting for 19″ racks.
- Pre‑installed Ubuntu 24.04 with full BSP and dev tools.

## Why Choose These Kits?


- **Unmatched Performance**: 12 TOPS AI, 2.5 GHz CPU, and ultra‑fast memory for real‑time workloads.
- **Extreme Connectivity**: 10/25 G Ethernet, 5G, 8K displays, and 4 camera inputs.
- **Rugged Design**: Wide temp, redundant power, and industrial I/O protection.
- **Security**: TEE, secure boot, TPM 2.0, and encrypted storage.
- **Scalability**: PCIe 4.0, M.2, and SATA for expansion.
- **Time‑to‑Value**: Pre‑tested hardware, certified modules, and production‑ready OS.


## What’s in the Box (PBKit 501‑A‑Base)


- PBKit 501‑A mainboard;
- Base board;
- 2×10 Gbps SFP+ modules;
- 1×5G modem (pre‑installed);
- 1×Wi‑Fi 6E antenna kit;
- 2×18–36 V power supplies (60 W each);
- 1×USB 3.2 Gen 2 cable;
- 1×Console cable (RJ45‑to‑USB);
- 1×RTC battery (CR2032);
- 1×quick‑start guide and compliance docs.


## Who Is It For?

- Edge AI researchers (autonomous systems, predictive maintenance);
- Defense/aerospace (C4ISR, drones, rugged HMI);
- Smart city deployments (traffic analytics, public safety);
- Medical imaging (real‑time 3D reconstruction);
- High‑frequency trading and financial tech;
- OEMs building mission‑critical embedded systems.

## Getting Started

1. **Unpack and inspect**: Verify all components and seals.
2. **Power up**: Connect redundant PSUs (ensure proper polarity).
3. **Interface setup**:  
   - Console: RJ45‑to‑USB for initial config;  
   - Network: SFP+ for 10 G, RJ45 for management;  
   - Display: HDMI/DP for UI;  
   - Storage: M.2/SATA for data drives.
4. **Download resources**:  
   - Visit [https://pb-embedded.ru/support](https://pb-embedded.ru/support) for:  
     - OS images and BSP (signed builds);  
     - Schematics, gerbers, and 3D models;  
     - API docs and sample apps;  
     - Compliance certificates (CE, FCC, IEC).
5. **Dev environment**:  
   - Cross‑compile for AArch64/RTSA;  
   - Flash eMMC via USB‑Boot mode;  
   - SSH access (default creds in `credentials.md`).
6. **Run examples**:  
   - AI: `tflite_benchmark` (resnet50);  
   - Vision: `gstreamer_8k` pipeline;  
   - I/O: `gpio_matrix_test`.

## Additional Services


We offer:
- custom PCB manufacturing;
- component sourcing;
- system integration services.


Technical support is available via email, phone, and Telegram.

## Where to Buy


Visit our website: [https://pb-embedded.ru/](https://pb-embedded.ru/)
Or email us at: polarbear.embedded@yandex.ru


> We’ll help you choose the right kit and provide support.

---

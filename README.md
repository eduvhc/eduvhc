### Hi, I'm Eduardo 👋

Software engineer building .NET microservices platforms.

---

#### Stack

![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-512BD4?style=flat&logo=csharp&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat&logo=typescript&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL_Server-CC2927?style=flat&logo=microsoftsqlserver&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)

---

#### Setup

<details>
<summary><b>Laptop</b> — MacBook Pro M5 (24 GB)</summary>

```yaml
# laptop.yml
device:
  model: MacBook Pro (2025)
  chip: Apple M5
  cores: 10 (4 performance + 6 efficiency)
  memory: 24 GB unified
  storage: 1 TB SSD
  os: macOS 26 (Tahoe)

dev_setup:
  shell: zsh
  editor: JetBrains Rider / VS Code
  containers: OrbStack
```

</details>

<details>
<summary><b>Desktop</b> — Ryzen 9 9950X3D · RX 9070 XT · 128 GB DDR5</summary>

```yaml
# desktop.yml
motherboard:
  model: MSI MAG X870E TOMAHAWK WIFI
  os: Windows 11 Pro

cpu:
  model: AMD Ryzen 9 9950X3D
  mpn: 100-100001286WOF
  architecture: Zen 5
  cores: 16
  threads: 32
  boost_clock_mhz: 5700

gpu:
  model: Sapphire NITRO+ Radeon RX 9070 XT Gaming OC
  mpn: 11348-01-20G
  architecture: RDNA 4
  vram: 16 GB GDDR6

case:
  model: Corsair Frame 4000D (Mid-Tower ATX, high airflow)
  mpn: CC-9011260-WW

psu:
  model: Corsair RM1000e 2025 (ATX 3.1, Cybenetics Gold, fully modular)
  mpn: CP-9020297-NA

ram:
  total: 128 GB
  model: Corsair Vengeance RGB DDR5-6000 CL30
  mpn: CMH64GX5M2B6000Z30
  config: 4x32 GB Dual Channel (2 kits)

storage:
  - model: Crucial T705 2 TB NVMe (PCIe 5.0, 14.5 GB/s read)
    mpn: CT2000T705SSD3
  - model: WD_BLACK SN7100 2 TB NVMe (PCIe 4.0)
    mpn: WDS200T4X0E

network:
  wifi: Wi-Fi 7 (Qualcomm FastConnect 7800)

monitors:
  - model: Dell U2724D 27" QHD 120Hz IPS Black (DisplayPort)
    mpn: 210-BKVH
  - model: Dell U2724D 27" QHD 120Hz IPS Black (HDMI)
    mpn: 210-BKVH

peripherals:
  keyboard:
    model: RK ROYAL KLUDGE M87 (75% gasket, hot-swap, wireless)
    asin: B0D3LNKQ3W
  mouse:
    model: ProtoArc EM11 NL Vertical Ergonomic (Bluetooth + 2.4GHz, 3-device)
  headset:
    model: HyperX Cloud Alpha 2 Wireless (2.4GHz + Bluetooth, RGB base, 53mm drivers, 250h)
    mpn: AJ5C7AA
```

</details>

<details>
<summary><b>Server</b> — Beelink Mini S12 · Intel N100 · Ubuntu 24.04</summary>

```yaml
# server.yml
host:
  hostname: pwuserver
  model: Beelink Mini S12 (AZW MINI S)
  os: Ubuntu 24.04 LTS (Noble Numbat)
  kernel: Linux 6.8

cpu:
  model: Intel N100
  architecture: Alder Lake-N
  cores: 4
  base_clock_ghz: 2.8
  boost_clock_ghz: 3.4
  tdp_w: 6

gpu: Intel UHD Graphics (Alder Lake-N, integrated)

memory:
  total: 16 GB
  type: DDR4-3200 SODIMM

storage:
  - role: system (SATA, internal)
    model: 512 GB SATA SSD (Beelink OEM)
    firmware: SN16525
  - role: bulk storage (USB 2.5" HDD)
    drive:
      model: Seagate Mobile HDD 2 TB 5400rpm
      mpn: ST2000LM007 (1R8174-070)
    enclosure:
      model: AISENS ASE-2525PB
      lot: V2410
  - role: external SSD (USB 2.5")
    drive:
      model: Samsung SSD 860 EVO 500 GB
      mpn: MZ-76E500B
    enclosure:
      model: Verbatim 53100

network:
  lan: 1 GbE (enp1s0)
  vpn: Tailscale

services:
  - Docker + containerd
  - Pi-hole (DNS / ad-block)
  - LocalStack (AWS emulator)
  - OpenObserve (logs / observability)
  - ps3netsrv (PS3 remote disc server)
```

</details>

<details>
<summary><b>Mobile & accessories</b> — iPhone 17 · WH-1000XM6 · AirPods 4 ANC</summary>

```yaml
# mobile.yml
phone:
  model: iPhone 17 (Black, base)
  chip: Apple A19 (3nm, 6-core CPU, 5-core GPU)
  memory: 8 GB RAM
  storage: 256 GB

headphones:
  model: Sony WH-1000XM6
  processor: HD Noise Canceling QN3 (12 mics, AI-adaptive ANC)
  codecs: LDAC, Hi-Res Audio Wireless
  bluetooth: 5.3 (multipoint)
  battery: 30h

earbuds:
  model: AirPods 4 with ANC
  chip: Apple H2
  features: ANC, Adaptive Audio, Transparency, Spatial Audio
  rating: IP54
  battery: 4h (20h with case)

charger:
  model: Anker Charger 100W USB-C GaN (3-port, smart display, touch control)
  mpn: A121B
  asin: B0FG77P8RR

bag:
  model: MOSISO Laptop Shoulder Bag 15.6" (Briefcase, 2 raised + 1 flap + 1 horizontal pocket)
  asin: B09J19C59Y
```

</details>

<details>
<summary><b>Network</b> — Starlink</summary>

```yaml
# network.yml
isp: Starlink (CGNAT, no public IPv4)
local_dns: Pi-hole (pwuserver)
vpn: Tailscale  # used to bypass CGNAT for remote access
```

</details>

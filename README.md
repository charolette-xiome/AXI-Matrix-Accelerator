# AXI-Matrix-Accelerator

![GitHub stars](https://img.shields.io/github/stars/charolette-xiome/AXI-Matrix-Accelerator?style=for-the-badge&logo=github) ![GitHub forks](https://img.shields.io/github/forks/charolette-xiome/AXI-Matrix-Accelerator?style=for-the-badge&logo=github) ![GitHub issues](https://img.shields.io/github/issues/charolette-xiome/AXI-Matrix-Accelerator?style=for-the-badge&logo=github) ![Last commit](https://img.shields.io/github/last-commit/charolette-xiome/AXI-Matrix-Accelerator?style=for-the-badge&logo=github)

## 📑 Table of Contents

- [Description](#description)
- [Screenshots](#screenshots)
- [Quick Start](#quick-start)
- [Project Structure](#project-structure)
- [Contributors](#contributors)
- [Contributing](#contributing)

## 📝 Description

AXI-Matrix-Accelerator — a software project built with modern tooling.

## 📸 Screenshots

![AXI Architecture](https://raw.githubusercontent.com/charolette-xiome/AXI-Matrix-Accelerator/main/docs/AXI Architecture.jpg)

![AXI Compute Core Architecture](https://raw.githubusercontent.com/charolette-xiome/AXI-Matrix-Accelerator/main/docs/AXI Compute Core Architecture.jpg)

![AXI Compute Wrapper FSM](https://raw.githubusercontent.com/charolette-xiome/AXI-Matrix-Accelerator/main/docs/AXI Compute Wrapper FSM.jpg)

![AXI Lite Interface](https://raw.githubusercontent.com/charolette-xiome/AXI-Matrix-Accelerator/main/docs/AXI Lite Interface.jpg)

![AXI Lite Wrapper](https://raw.githubusercontent.com/charolette-xiome/AXI-Matrix-Accelerator/main/docs/AXI Lite Wrapper.jpg)

![AXI MAC Diagram](https://raw.githubusercontent.com/charolette-xiome/AXI-Matrix-Accelerator/main/docs/AXI MAC Diagram.png)

## ⚡ Quick Start

```bash

# 1. Clone the repository
git clone https://github.com/charolette-xiome/AXI-Matrix-Accelerator.git

# See the Development Setup section below
```

## 📁 Project Structure

```
.
├── docs
│   ├── AXI Architecture.jpg
│   ├── AXI Compute Core Architecture.jpg
│   ├── AXI Compute Wrapper FSM.jpg
│   ├── AXI Lite Interface.jpg
│   ├── AXI Lite Wrapper.jpg
│   ├── AXI MAC Diagram.png
│   └── AXI UVM TB Architecture.jpg
├── rtl_codes
│   ├── AXI Matrix Accelerator.sv
│   ├── Top.sv
│   ├── axi_codes
│   │   └── AXI-Lite Control Wrapper.sv
│   ├── controller_codes
│   │   ├── Compute Wrapper.sv
│   │   └── Controller FSM.sv
│   └── mac_codes
│       ├── MAC Array 4x4.sv
│       ├── MAC Array MxN.sv
│       ├── MAC.sv
│       ├── Matrix Multiplication Control Path.sv
│       ├── Matrix Multiplication Data Path.sv
│       ├── Matrix Multiplication MxN kN.sv
│       ├── Matrix Multiplication Top.sv
│       └── Matrix Multiply 2x2 kN.sv
├── scripts
│   ├── Filelist.f
│   ├── Run XSIM UVM.sh
│   ├── Run XSIM.sh
│   └── UVM Testbench Filelist.f
├── sequence_items
│   ├── AXI Lite Item.sv
│   └── AXI Stream Packet.sv
└── testbenches
    ├── AXI Lite Control Wrapper Testbench.sv
    ├── Basic Testbench.sv
    ├── COMP Wrapper Testbench14 Backpress.sv
    ├── Comp Wrapper Testbench Stress.sv
    ├── Comp Wrapper Testbench13 FSM.sv
    ├── Comp Wrapper Testbench15 doneIntr.sv
    ├── Matrix Multiplication 2x2 kN Testbench.sv
    ├── Matrix Multiplication Core Testbench.sv
    ├── Matrix Multiplication MxN kN Testbench.sv
    ├── Testbench AXI Matrix Accumulator.sv
    ├── Testbench Package.sv
    ├── agents
    │   ├── AXI Lite Agent.sv
    │   ├── AXI Lite Driver.sv
    │   ├── AXI Lite Monitor.sv
    │   ├── AXI Lite Sequencer.sv
    │   ├── AXI Stream Agent.sv
    │   ├── AXI Stream Driver.sv
    │   ├── AXI Stream Monitor.sv
    │   ├── AXI Stream Sequencer.sv
    │   └── Virtual Sequencer.sv
    ├── common
    │   └── AXI Types.sv
    ├── env
    │   ├── AXI Environment.sv
    │   └── AXI Matrix Accumulator System Environment.sv
    ├── interfaces
    │   ├── AXI Lite Interface.sv
    │   └── AXI Stream Interface.sv
    ├── ref_model
    │   └── AXI Reference Model.sv
    ├── scoreboard
    │   ├── AXI Reg Model.sv
    │   ├── AXI S Scoreboard.sv
    │   └── AXI Scoreboard.sv
    ├── sequence_items
    │   ├── AXI Lite Item.sv
    │   └── AXI Stream Packet.sv
    ├── sequences
    │   ├── AXI Basic Sequence.sv
    │   ├── AXI Lite Read Sequence.sv
    │   ├── AXI Matrix Multiplication System VSequence.sv
    │   ├── AXI Random Sequence.sv
    │   ├── AXI Simple Sequence.sv
    │   ├── CFG Read Sequence.sv
    │   ├── Control CFG Sequence.sv
    │   └── Start Control Sequence.sv
    ├── tests
    │   ├── AXI Matrix Multiplication System Test.sv
    │   ├── AXI Random Test.sv
    │   ├── AXIs Data Sanity Test.sv
    │   └── Base test.sv
    └── top
        └── Testbench Top.sv
```

## 👥 Contributors

Thanks to everyone who has contributed to this project:

<p align="left">
<a href="https://github.com/charolette-xiome" title="charolette-xiome"><img src="https://avatars.githubusercontent.com/u/167672969?v=4&s=64" width="64" height="64" alt="charolette-xiome" style="border-radius:50%" /></a>
</p>

[See the full list of contributors →](https://github.com/charolette-xiome/AXI-Matrix-Accelerator/graphs/contributors)

## 👥 Contributing

Contributions are welcome! Here's the standard flow:

1. **Fork** the repository
2. **Clone** your fork: `git clone https://github.com/charolette-xiome/AXI-Matrix-Accelerator.git`
3. **Branch**: `git checkout -b feature/your-feature`
4. **Commit**: `git commit -m 'feat: add some feature'`
5. **Push**: `git push origin feature/your-feature`
6. **Open** a pull request

Please follow the existing code style and include tests for new behavior where applicable.

---

<div align="center">

[![Made with ReadmeBuddy](https://img.shields.io/badge/Made%20with-ReadmeBuddy-8B5CFF?style=for-the-badge&logo=markdown&logoColor=white)](https://readmebuddy.com)

<sub>Generate beautiful READMEs in seconds → <a href="https://readmebuddy.com">readmebuddy.com</a></sub>

</div>

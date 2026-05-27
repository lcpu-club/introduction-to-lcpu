---
theme: slidev-theme-lcpu
title: Introduction to LCPU
transition: fade-out
zoom: 0.8
---

# <span style="font-weight: initial">Introduction to </span><br>Linux Club of Peking University

<br> <span style="line-height: 35px">Presented by **[Sifer](https://github.com/Chen571428)**</span>
<br> Mar. 29th 2026

<!--
aaa
-->

---
zoom: 1.2
---

# Overview

<v-clicks>

- Founded in **2003**, Free/Libre and Open Source Software (**FOSS**).
- Very Active Student Club related to **Computer Science**
- 400+ Members from a Variety of Departments
- 50+ Core Members Working in Various Projects and Teams
- Install Party, Seminars/Lectures
- HPCGame, GeekGame, ...
- CLab, PKUTeX, PKUGit, SigStore ...
- SigHW, SigMLSys / AI Infra, Rust, Kernel ...
- Getting Started (Missing Semester Course from MIT) & The **Notebook**
- LLM From Scratch
- Visits to Sister Clubs, Uni.s, and Top Businesses in CS

</v-clicks>

---
zoom: 1.2
---

<Image src="/brand-club.jpg" caption="Brand Club from 2023-2026 in Peking University"/>

<p style="text-align: center; color: grey; font-size: smaller; margin-top: -5px">only 5 clubs can be entitled this honor every year</p>

---
zoom: 1.2
---

# LCPU Infrastructures

Infrastructure that Enpowers PKU

<v-clicks>

- CLab: All-in-one Cloud Provider
- PKUTeX: Online LaTeX Collaboration
- PKUGit: Secure Git Hosting w/ CI/CD Pipelines
- SigStore: **PetaBytes** Level S3 / WebDev Storage Provider

</v-clicks>

---
zoom: 1.2
---

<Video src="/clab.mp4" caption="CLab demo: Creating a VM"/>

---
zoom: 1.1
---

<Video src="/wukong.mp4" caption="Black Myth: Wukong demo w/ remote GPU on CLab"/>

<p style="text-align: center; color: grey; font-size: smaller">( video is compressed, gameplay at 1080P/60FPS )</p>


---
zoom: 1.2
---

# Services: CLab

<v-clicks>

- All-in-one Cloud Platform
- Free 4C4G qouta for every student
- Serving over 2,500 Users
- Support over 30 courses
- Remote Development
- Education and Research

</v-clicks>

---
zoom: 1.2
---

# Services: CLab v2 [WIP]

<v-clicks>

- Remote GPU
  - Machine Learning
  - LLM
  - HPC acceleration
  - Gaming
- High-Performance RDMA Network
- DAOS Distributed High-Performant Storage / Ceph
- DOCA-Powered Bare-Metal Virtualization

</v-clicks>

---
zoom: 1.2
---

<Video src="/latex.mp4" caption="PKUTeX demo: Building LaTeX documents"/>

---
zoom: 1.2
---

# Services: PKUTeX

<v-clicks>

- Overleaf w/ Premium Features
  - Reference Auto-completion
  - Sandboxed Compilation
  - Review and Comments
  - ...
- Unlimited Compilations and Collaboration

</v-clicks>

---
zoom: 1.2
---

<Image src="/pkugit.png" caption="PKUGit demo"/>

---
zoom: 1.2
---

# Services: PKUGit

<v-clicks>

- Secure Platform for Code Management
- CI/CD Pipelines Powered by CLab

</v-clicks>

---
zoom: 1.2
---

# LCPU Competitions

<v-clicks>

- HPCGame
  - Co-Hosted with Weiming HPC Team
  - Entry-Level High Performence Competition Competition
- GeekGame
  - Co-Hosted with PKUCC Team & Tsinghua Univ.
  - Entry-Level CTF Competition

</v-clicks>

---
zoom: 1.2
---

# Competitions: HPCGame

<v-clicks>

- Entry-level Competition Featuring Parallelizing Programs
- Encourage More Students to Enter the Field of HPC
- In Deep Collaboration with Weiming HPC Team
- Universal AutoJudge Platform Built by LCPU
- 0th to 2th: Thousands of Students from across China and the Globe
</v-clicks>

---
zoom: 1.2
---

<Image src="/hpcgame.png" caption="AOI Platform for HPCGame" />

---
zoom: 1.1
layout: two-cols-header
---

# <span style="font-weight: bold">AI Infra Study Group · Logistics</span>

::left::

<v-clicks>

- **Seminar Format**: 1-2 sessions weekly; a group of students present on a specific topic
- **High Standards**: 20-40 min per session; code, handouts, and exercises required (no vibe-only)
- **Multi-channel Publishing**: Videos on Bilibili & YouTube; documents on WeChat, Web, hpcwiki & Zhihu
- **Guest Lectures**: Guest talks by Weiming HPC team seniors and sponsor engineers

</v-clicks>

::right::

<v-clicks>

- **Requirements**: Normal participants present $\ge 1$ time; PKUSC core members $\ge 2$ times
- **Compute & Support**: GPU development nodes sponsored; exercises integrated into HPCGame auto-judge
- **Incentives & Rewards**: 300-600 RMB compensations per lecture based on peer evaluations

</v-clicks>

---
zoom: 1.1
---

# <span style="font-weight: bold">AI Infra Topics: GPU Programming</span>

<v-clicks>

- **GPU Architecture & CUDA Programming** (Sessions 01-04)
  - Hardware architecture, programming models, CUDA ecosystem, CUB and parallel algorithms
- **Hardware-Aware Optimizations** (Sessions 05-07)
  - Warp divergence, bank conflicts, memory hierarchy, TMA, Tensor Cores, and computing bounds
- **Kernel Writing & Tuning** (Sessions 08-10)
  - Speed of Light, Profiling, Fusing, Tiling, Soft pipeline, and Warp specialization
- **Domain-Specific Languages (DSL)** (Sessions 11-14)
  - Triton programming, TileLang primitives, CuTeDSL, and trading off in DSL
- **Advanced Kernel Design** (Sessions 15-18)
  - Ampere/Hopper/Blackwell features; SoL GEMM, Attention (MHA/MLA), and MoE optimizations

</v-clicks>

---
zoom: 1.0
layout: two-cols-header
---

# <span style="font-weight: bold">AI Infra Topics: Systems & Compilation</span>

::left::

<v-clicks>

- **ML Compiler & Compilation**
  - **Auto-tuning**: Triton, TileLang, TVM, AutoTVM, Ansor
  - **Graph Optimizations**: TASO, PET
  - **Code Generation**: DSL to cubin compile pipeline
- **Cluster Communication**
  - **High-speed Network**: TCP/IP to RDMA (IB, RoCE, iWarp)
  - **Communication Libraries**: NCCL/UCCL internals, torch.distributed primitives
  - **Co-design**: Writing custom communication Kernels

</v-clicks>

::right::

<v-clicks>

- **LLM Training & Inference & RL**
  - **Distributed Training**: DP, ZeRO-1/2/3, FSDP, TP, PP, SP, CP, EP
  - **High-performance Serving**: Paged Attention, PD Separation, Continuous Batching, Speculative Decoding
  - **RL Frameworks**: verl, ROLL, multi-framework coordination
- **Generative AI Algorithm Foundation**
  - Transformers/Diffusion, Scaling Laws/MoE, Long Context, Reasoning models

</v-clicks>

---
zoom: 1.2
---

# LCPU Events

<v-clicks>

- Install Party
- NVIDIA GTC Watch Party
- JetBrains Techniques Salon
- Visits to AMD
- Nights of Distros
- ...

</v-clicks>

---
zoom: 1.2
---

# LCPU Programmes
- LCPU Getting Started
- SigHW (FPGA, DMA, etc.)
- SigMLSys / AI Infra
- SigAgent
- The **Notebook**
- LLM From Scratch (CS336 From Stanford, 200+ participant)


---
zoom: 1.1
layout: two-cols-header
---

# <span style="font-weight: bold">Courses: Getting Started</span>

::left::

<v-clicks style="margin: auto">

- Comprehensive Tutorials on CS
- From Beginners to the Experienced
- Intro, Experiments, Tasks
- [Online Textbooks](https://missing.lcpu.dev) with In-class Courses

</v-clicks>

::right::

<img :src="'/lgs-bilibili.png'" />

<span style="font-size: smaller; text-align: center">LGS: Stats on Chinese Video Sharing Platform Bilibili</span>

---
zoom: 1.2
---

# LCPU Living!
- LCPU Wechat Group (100+ DAU, Rust, Arch, ~~Deepseek V4😡~~)
- LCPU 吃喝玩乐!
- LCPU Cooking!

---
zoom: 1.2
---

# LCPU Core
- Operations Department
- Technical Department
- Learning Department
- Ops Team

---
zoom: 1.2
---

# Thanks
Thanks Wizard Quant for Sponsoring us!

<img :src="'/wizard-quant.png'" alt="Wizard Quant" />


---
layout: center
---

<span class="text-3rem bold mx-auto my-auto" v-mark.underline>Thanks for Listening!</span>

---
layout: end
---

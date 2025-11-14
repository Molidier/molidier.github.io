---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* **Nazarbayev University**, BS in Computer Science — CGPA 3.68/4.0 (Top 3% of cohort), 2022–June 2026, Astana, Kazakhstan  
  * Dean’s List for Academic Excellence — Fall 2024  
  * Selected coursework: Micro-architecture Design and Verification; Computer Systems and Organization; Internet of Things; Micro-controllers; Operating Systems; Computer Networks; Data Structures and Algorithms  

Work experience
======
* **UGRIP Research Intern, MBZUAI (Mohamed bin Zayed University of Artificial Intelligence)**  
  *June 2025 – October 2025, Abu Dhabi, United Arab Emirates*  
  * Investigated failure modes in LLM-based assembly transpilation across x86, ARMv8, and RISC-V by analyzing 200+ programs and identifying systematic weaknesses in instruction semantics and register allocation.  
  * Established a taxonomy of 25 recurring failure patterns and designed a synthetic program generation pipeline (≈400k C programs), improving cross-ISA transpiler accuracy on held-out benchmarks.  

* **Senior Thesis Project – Educational Chatbot for Second Language Learning, Nazarbayev University**  
  *August 2025 – Present, Astana, Kazakhstan*  
  * Building an edge-deployed STT–LLM–TTS language learning system optimized for an 8GB Orange Pi NPU, focusing on low-latency inference.  
  * Fine-tuning a 1B-parameter LLM on A2-level content with controllable pedagogical parameters (e.g., correction directness, encouragement frequency) to study tutoring strategies in resource-constrained settings.  

* **RTL Design and Verification Engineer, Texer.AI (Hardware Verification & EDA Startup)**  
  *September 2024 – Present, Astana, Kazakhstan*  
  * Implemented a 16-bit “Bitty” processor with a custom 21-instruction ISA in synthesizable Verilog and developed its verification infrastructure.  
  * Designed a RISC-V32E → custom 16-bit ISA asm-to-asm translator, mapping ~40 instructions to 21 optimized opcodes while maintaining ≈95% code density and functional correctness.  
  * Validated the custom processor on a DE1-SoC FPGA by implementing UART and a Load-Store Unit, achieving 140 MHz in 526 ALMs with PC-controlled instruction streaming.  
  * Implemented an I²C master on Tang Nano 9K to drive an SSD1306 OLED with a memory-mapped frame buffer for real-time visualization of processor state.  

* **Teaching Assistant & Lab Developer – Microarchitecture Design and Verification, MAVERIC Lab, Nazarbayev University**  
  *January 2025 – May 2025, Astana, Kazakhstan*  
  * Supported Kazakhstan’s first hardware design course, mentoring 18 students who successfully completed working processor designs.  
  * Designed two hands-on FPGA labs (UART and Load-Store Unit) on the Altera DE1-SoC and ran weekly Q&A / debugging sessions for 20+ students.  
  * Created a cocotb-based verification framework for Tiny Tapeout-style designs, reducing student onboarding time by about 70%.  

Selected Projects
======
* **Single-Cycle RISC-V RV32I Processor** — *SystemVerilog, C++, Verilator*  
  * Designed a complete RV32I processor supporting all 37 base instructions with a single-cycle datapath.  
  * Built a C++/Verilator co-simulation framework with waveform tracing for cycle-accurate debugging.  
  * Validated the design against the official RISC-V compliance test suite, achieving full ISA conformance.  

* **“Bitty” Processor (Tiny Tapeout)** — *Verilog, C++, Verilator*  
  * Architected a 16-bit custom processor with a 21-instruction ISA and 3 instruction formats.  
  * Developed a C++/Verilator co-simulation testbench that uncovered and resolved critical hardware bugs.  
  * Built a custom C++ assembler and disassembler to accelerate firmware development and debugging for the core.  

* **SSD1306 OLED Driver on Tang Nano 9K** — *Verilog, I²C*  
  * Implemented a Verilog I²C master FSM for 100 kHz display initialization, configuration, and data transfer.  
  * Designed a pixel-addressable frame buffer with a memory-mapped interface for low-latency rendering.  
  * Integrated custom debug logic to speed up hardware bring-up and visualization of processor internals.  

Skills
======
* **Hardware Design & Verification:** SystemVerilog, Verilog, cocotb, Verilator, Icarus Verilog, GTKWave  
* **Programming Languages:** C, C++, Python  
* **Tools & Platforms:** Linux, Git/GitHub, Quartus, Gowin EDA, Make/Makefile, Hugging Face, vLLM  
* **Hardware Platforms & Protocols:** DE1-SoC FPGA, Tang Nano 9K, UART, I²C, Wishbone  

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* **Co-Lead, Google Developer Group at Nazarbayev University**, January 2024 – Present  
  * Coordinated a 20-person organizing team for a 60-member developer community, managing event logistics and communication with university administration.  
  * Organized the “Google Solution Challenge Camp” with ~60 participants and external guest speakers, and established standardized communication workflows between the club and the university.  

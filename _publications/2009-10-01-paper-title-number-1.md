---
title: "Spaghetti-O: O2 Optimization Level CISC→RISC Transpilation"
collection: publications
category: manuscripts
permalink: /publication/2026-01-01-spaghetti-o-o2-cisc-risc-transpilation
excerpt: "We analyze failure modes of LLM-based transpilers at -O2, focusing on cross-ISA correctness across x86, ARMv8, and RISC-V."
date: 2026-01-01
venue: "Under submission"
slidesurl: ""          # e.g., "/files/spaghetti-o-slides.pdf"
paperurl: ""           # e.g., "/files/spaghetti-o-paper.pdf"
bibtexurl: ""          # e.g., "/files/spaghetti-o.bib"
citation: "Azhimukhanbet, M. et al. (2026). \"Spaghetti-O: O2 Optimization Level CISC→RISC Transpilation.\" Under submission."
---

This work studies the robustness and correctness of LLM-based assembly transpilers operating at the **-O2 optimization level** for CISC→RISC translation. Using a curated and synthetically-augmented benchmark that spans **x86, ARMv8, and RISC-V**, we:

- Build a **taxonomy of recurrent failure modes**, including mis-handled calling conventions, broken control-flow, and incorrect flag/condition semantics.  
- Introduce a **program generation pipeline** that produces diverse C programs whose compiled assembly stresses specific instruction patterns and optimization interactions.  
- Show that targeted augmentation using these synthetic programs can **improve cross-ISA translation accuracy** on held-out benchmarks, especially for tricky patterns such as loop unrolling, strength reduction, and instruction fusion at -O2.
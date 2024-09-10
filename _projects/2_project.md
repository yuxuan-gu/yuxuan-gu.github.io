---
layout: page
title: RISCV CPU
description: 
img: assets/img/RISCV-CPU/CPU-3.png
importance: 1
category: 2022
# related_publications: true
---

# Project information:
- **Category**: Instruction-set Architecture and Compiler (IAC) coursework [[Github link](https://github.com/guyuxuan9/RISCV-CPU/tree/main)]
- **Year**: 2022
- **Location**: Imperial College London, London, UK

Our team of four successfully developed a single-cycle CPU from scratch using System Verilog and Verilator, featuring diverse instructions like addi, lw, and jal. This achievement led us to delve into pipelining, where we meticulously segmented tasks into Registers and Control Unit, Data Hazards, Control Hazards, and Testing. The culmination of our coursework involved the implementation of cache memory, encompassing both directly mapped and 2-way associative mapped approaches.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/RISCV-CPU/CPU-3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Block diagram of the RISCV single-cycle CPU
</div>


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/RISCV-CPU/CPU-1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/RISCV-CPU/CPU-2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    On the left, visualisation of the executed output of the CPU; Right, waveforms in gtkWave for debugging.
</div>


---
title: "Benchmarking GPU Matrix Operations Optimizations"
date: 2025-05-23
lastmod: 2025-05-23
tags: ["Transformers", "CUDA", "GPU Optimization", "AI", "Deep Learning", "Python", "C++", "PyTorch", "NVIDIA Nsight Systems", "Profiling Tools"]
description: "Comprehensive benchmarking study of matrix transpose and multiplication optimizations across NVIDIA GPU architectures, analyzing performance characteristics and implementation strategies."
summary: "Completed project for CS6501: GPU Architectures at the University of Virginia. This research presents a comprehensive benchmarking study of matrix operation optimizations across NVIDIA GPU architectures, focusing on matrix transpose and multiplication. Through systematic evaluation of custom CUDA kernels and library implementations across RTX 2080 Ti and A100 GPUs, demonstrated that vectorized implementations achieve up to 6x speedup over naive approaches, reaching 1800 GB/s throughput on A100."
showToc: false
weight: 2
cover:
    image: "project2.png"
    alt: "GPU Matrix Operations Performance Benchmarking"
    relative: false
---

---

##### Links

+ [Final Report](GPU_Architectures_Final_Project.pdf)
+ [Code](https://github.com/mmjerge/cudatorch)
+ [Final Presentation Slides](GPUArch_final_slides.pdf)

---

##### Overview
Conducted comprehensive benchmarking of CUDA matrix operations to explore opportunities for reducing latency and improving GPU resource utilization in AI workloads across NVIDIA Turing and Ampere architectures (RTX 2080 Ti and A100 GPUs). I focused in matrix transpose analysis, implementing multiple custom CUDA kernels using advanced techniques including shared memory tiling with bank conflict avoidance, vectorized float4 memory access, and warp shuffle primitives. Systematically compared custom implementations against industry-standard libraries (cuBLAS, CUTLASS, CuTe) across matrix dimensions (32×32 to 8192×8192), identifying architecture-specific optimization strategies for transformer model acceleration.

---

#### Related material

+ [🏛️ CS6501: GPU Architectures Course](https://adwaitjog.github.io/teach/uva_6501_s25.html)
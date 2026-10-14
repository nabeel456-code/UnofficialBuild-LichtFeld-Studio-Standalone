# LichtFeld Studio Standalone

A prebuilt Windows standalone environment for **LichtFeld Studio**—a high-performance, native application designed to train, inspect, edit, automate, and export 3D Gaussian Splatting (3DGS) scenes.

---

## 🚀 Overview

This repository hosts a compiled desktop distribution of LichtFeld Studio, bundling the application executable, native rendering and machine learning backend libraries (CUDA/OnnxRuntime/Tensor kernels), python integration runtimes, and local workspace directories.

### Key Capabilities
- **Native 3DGS Training & Inspection:** Fast local training loops leveraging modern C++ and NVIDIA CUDA hardware acceleration.
- **Interactive Editing Suite:** Brush, mask, crop, and manipulate gaussian subsets directly inside the live viewport.
- **Plugin Architecture & Python Runtime:** Extend processing pipelines via custom Python scripts, embedded runtimes, and local plugins.
- **Model Interoperability:** Import/export common radiance field assets (PLY, SPZ, SOG, USD, glTF).

---

## 🛠️ System Requirements

To successfully run or build upon this standalone distribution, your system must meet the following baseline requirements:

| Component | Minimum Requirement |
| :--- | :--- |
| **OS** | Windows 10 / 11 (64-bit) |
| **GPU** | NVIDIA GPU with **CUDA Compute Capability 7.5+** (GTX 16-series, RTX 20-series or newer) |
| **Drivers** | Recent NVIDIA Display Drivers with CUDA support |
| **Memory** | 16 GB+ RAM recommended (dependent on dataset size) |

*Note: AMD and Intel GPUs are not supported for training or core CUDA-accelerated rendering workflows.*

---

## 📂 Directory Structure

```text
C:\INSTALLED_SOFTWAREs\LichtFeld-Studio-Standalone\
│
├── LichtFeld-Studio.exe    # Main application executable
├── DLLs/                   # Required dynamic link libraries (FFmpeg, OpenEXR, etc.)
├── extensions/             # Application extensions and plugin modules
├── src/                    # Internal python modules & frontend panel contracts
├── resources/              # Shaders, UI assets, and runtime configurations
└── usd/                    # Universal Scene Description bindings & DLLs

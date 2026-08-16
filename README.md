# 🚀 Edge AI on Raspberry Pi 5

> **Building, optimizing, deploying, and benchmarking AI directly at the edge.**

This repository is a hands-on **Edge AI engineering platform built around Raspberry Pi 5**, focused on running modern AI/ML workloads on resource-constrained embedded hardware.

The project explores the complete Edge AI pipeline:

**Model Development → Conversion → Optimization → Quantization → Hardware Acceleration → Deployment → Profiling → Real-Time Inference**

The goal is to understand not only how to build AI models, but also how to make them **fast, efficient, memory-conscious, and deployable on real embedded systems**.

---

## 🎯 Project Goals

* Build AI applications directly on Raspberry Pi 5
* Deploy deep learning models at the edge
* Explore CPU, GPU and NPU acceleration
* Optimize AI models for embedded hardware
* Experiment with quantization and reduced-precision inference
* Benchmark latency, throughput, memory and power efficiency
* Explore real-time computer vision
* Experiment with NLP and lightweight LLMs
* Integrate cameras, sensors and other edge devices
* Explore AI deployment across Linux and Android/AOSP
* Develop reusable Edge AI deployment workflows

---

## 🧠 Areas of Exploration

### Computer Vision

Real-time vision applications using the Raspberry Pi camera and external cameras.

Examples:

* Object detection
* Object classification
* Image segmentation
* Face detection
* Pose estimation
* OCR
* Video analytics
* Multi-object tracking

---

### 🤖 Deep Learning

Experimentation with modern neural-network architectures and deployment frameworks.

* CNNs
* MLPs / ANN
* Transformers
* Vision Transformers
* Lightweight vision models
* Multimodal models
* TinyML / Edge ML models

---

### 🗣️ NLP & LLMs

Exploring the possibility of running smaller language models directly on edge hardware.

Areas include:

* Small Language Models
* LLM inference
* Tokenization
* Embeddings
* Quantized models
* RAG experiments
* Local AI assistants
* Speech-to-text / text-to-speech

---

## ⚡ Model Optimization

A major focus of this repository is **AI performance optimization for edge hardware**.

Techniques explored include:

* FP32 inference
* FP16 inference
* INT8 quantization
* Post-training quantization
* Quantization-aware training
* Model pruning
* Knowledge distillation
* Operator optimization
* Graph optimization
* Memory optimization
* Batch-size optimization

---

## 🔄 AI Deployment Pipeline

```text
              ┌──────────────────────┐
              │   AI Model Training  │
              │ PyTorch / TensorFlow │
              └──────────┬───────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │   Model Conversion   │
              │       ONNX           │
              └──────────┬───────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │ Model Optimization   │
              │ Quantization / Graph │
              │      Optimization    │
              └──────────┬───────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │ Hardware Acceleration│
              │ CPU / GPU / NPU      │
              └──────────┬───────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │ Raspberry Pi 5       │
              │ Edge Deployment      │
              └──────────┬───────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │ Real-Time Inference  │
              │ + Profiling          │
              └──────────────────────┘
```

---

# 🖥️ Hardware

## Raspberry Pi 5

Primary development platform:

* Raspberry Pi 5
* ARM64
* Cortex-A76 CPU
* VideoCore VII GPU
* Raspberry Pi Camera
* USB peripherals
* GPIO / SPI / I2C / UART
* Ethernet / Wi-Fi / Bluetooth

---

## 🧩 AI Accelerators

The repository will also explore external AI acceleration hardware such as:

* Raspberry Pi AI HAT+
* NPU accelerators
* Edge AI inference accelerators
* USB AI accelerators
* Other ARM-based AI platforms

The objective is to compare **CPU-only vs GPU vs NPU accelerated inference**.

---

# 🐧 Operating Systems

Experiments will primarily focus on:

### Raspberry Pi OS

Native Linux-based Edge AI development and deployment.

### Android / AOSP

Exploring AI workloads running on:

```text
Raspberry Pi 5
      │
      ├── Linux
      │
      └── Android / AOSP
```

This provides an opportunity to investigate AI deployment in both **embedded Linux and Android Automotive / embedded Android environments**.

---

# 🛠️ Software Stack

## Programming Languages

* Python
* C++
* Bash

## AI / ML

* PyTorch
* TensorFlow
* Keras
* ONNX
* ONNX Runtime
* TensorFlow Lite

## Computer Vision

* OpenCV
* GStreamer
* Picamera2

## Development

* Git
* CMake
* GCC
* Clang
* Docker
* Linux

---

# 📦 Repository Structure

```text
edge-ai-rpi5/
│
├── README.md
│
├── models/
│   ├── classification/
│   ├── detection/
│   ├── segmentation/
│   ├── vision/
│   └── llm/
│
├── python/
│   ├── inference/
│   ├── vision/
│   ├── nlp/
│   ├── preprocessing/
│   └── benchmarking/
│
├── cpp/
│   ├── inference/
│   ├── vision/
│   ├── runtime/
│   └── benchmarks/
│
├── conversion/
│   ├── pytorch/
│   ├── tensorflow/
│   └── onnx/
│
├── quantization/
│   ├── fp16/
│   ├── int8/
│   └── calibration/
│
├── acceleration/
│   ├── cpu/
│   ├── gpu/
│   └── npu/
│
├── camera/
│   ├── capture/
│   ├── streaming/
│   └── vision/
│
├── llm/
│   ├── inference/
│   ├── quantization/
│   └── benchmarks/
│
├── benchmarks/
│   ├── latency/
│   ├── throughput/
│   ├── memory/
│   └── power/
│
├── scripts/
│
├── docs/
│
└── examples/
```

---

# 📊 Performance Benchmarking

Performance is a core part of this project.

Each model will be evaluated using metrics such as:

| Metric     | Description                     |
| ---------- | ------------------------------- |
| Latency    | Time required for one inference |
| FPS        | Frames processed per second     |
| Throughput | Inferences per second           |
| CPU Usage  | Processor utilization           |
| GPU Usage  | GPU utilization                 |
| NPU Usage  | Accelerator utilization         |
| RAM        | Memory consumption              |
| Power      | Approximate power consumption   |
| Model Size | Storage requirements            |
| Accuracy   | Model prediction quality        |

Example:

```text
Model: YOLO

Backend       Latency       FPS       RAM
------------------------------------------------
CPU           XX ms         XX        XX MB
GPU           XX ms         XX        XX MB
NPU           XX ms         XX        XX MB
```

---

# 🔬 Example Projects

The repository will gradually include practical Edge AI applications such as:

### 👁️ Real-Time Object Detection

```text
Camera
   ↓
Frame Capture
   ↓
Preprocessing
   ↓
AI Model
   ↓
Hardware Accelerator
   ↓
Post Processing
   ↓
Detected Objects
```

### 🧍 Human Detection & Tracking

Real-time detection and tracking using Raspberry Pi camera input.

### 📷 Smart Vision Monitor

Camera-based monitoring using optimized AI models.

### 🗣️ Local AI Assistant

Experimenting with small language models running locally on the Raspberry Pi.

### 📡 Sensor + AI

Combining sensor data with machine-learning models for edge intelligence.

---

# 🧪 Experiments

Each experiment will document:

```text
Hardware
   ↓
Operating System
   ↓
Model
   ↓
Framework
   ↓
Model Format
   ↓
Optimization
   ↓
Inference Backend
   ↓
Benchmark
   ↓
Results
```

Experiments will be reproducible wherever possible.

---

# 📈 Performance Optimization Workflow

```text
Original Model
      │
      ▼
Baseline Benchmark
      │
      ▼
Model Conversion
      │
      ▼
FP16 / INT8 Optimization
      │
      ▼
Hardware Acceleration
      │
      ▼
Runtime Optimization
      │
      ▼
Benchmark Again
      │
      ▼
Compare Results
```

The objective is not simply to achieve the highest accuracy, but to find the best balance between:

**Accuracy ↔ Latency ↔ Memory ↔ Power ↔ Throughput**

---

# 🔧 Setup

Clone the repository:

```bash
git clone https://github.com/<username>/edge-ai-rpi5.git
cd edge-ai-rpi5
```

Create a Python environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Run an example:

```bash
python3 examples/inference.py
```

> Individual experiments may have their own dependencies and setup instructions.

---

# 🧠 Engineering Philosophy

This repository is not limited to running pre-trained models.

The focus is on understanding the **entire Edge AI stack**:

```text
AI / ML
   │
   ▼
Model Architecture
   │
   ▼
Model Optimization
   │
   ▼
Inference Runtime
   │
   ▼
Compiler / Graph
   │
   ▼
CPU / GPU / NPU
   │
   ▼
Operating System
   │
   ▼
Embedded Hardware
```

The long-term objective is to understand how AI workloads move from **research environments into real embedded products**.

---

# 🚀 Future Roadmap

* [ ] Raspberry Pi 5 AI environment setup
* [ ] Camera-based inference pipeline
* [ ] PyTorch inference
* [ ] ONNX conversion
* [ ] ONNX Runtime deployment
* [ ] TensorFlow Lite experiments
* [ ] FP16 benchmarking
* [ ] INT8 quantization
* [ ] Raspberry Pi AI HAT+ integration
* [ ] CPU vs GPU vs NPU benchmarking
* [ ] Real-time object detection
* [ ] Real-time segmentation
* [ ] Edge NLP experiments
* [ ] Lightweight LLM inference
* [ ] LLM quantization
* [ ] RAG on Raspberry Pi
* [ ] C++ inference runtime
* [ ] Linux deployment
* [ ] Android / AOSP deployment
* [ ] Automated benchmarking
* [ ] Power/performance analysis
* [ ] Multi-platform Edge AI benchmarking

---

# 📚 Documentation

Detailed documentation will be maintained in:

```text
docs/
├── setup/
├── models/
├── optimization/
├── quantization/
├── acceleration/
├── benchmarking/
├── linux/
├── android/
└── llm/
```

---

# 🌍 Vision

The long-term goal is to evolve this repository from a Raspberry Pi experimentation project into a **practical Edge AI engineering platform** covering:

**AI + Embedded Linux + C++ + Computer Vision + LLMs + Model Optimization + Hardware Acceleration**

with an emphasis on **real-time, efficient and production-oriented AI deployment at the edge**.

---

## ⭐ Why Raspberry Pi 5?

Raspberry Pi 5 provides an excellent platform for understanding the constraints and engineering challenges involved in deploying AI outside the cloud.

Instead of relying entirely on powerful data-center GPUs, this project explores:

> **How much intelligence can we move from the cloud to the edge?**

---

## 📜 License

This project will be released under the license specified in the repository.

---

## 👨‍💻 Author

**Sivaraman Ramamoorthy**

Exploring:

`Edge AI` • `Embedded Linux` • `C++` • `Computer Vision` • `Deep Learning` • `LLM Inference` • `Model Optimization` • `Hardware Acceleration`

---

⭐ **If you find this project useful, consider starring the repository and following the experiments as the platform evolves.**

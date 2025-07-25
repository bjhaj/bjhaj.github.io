---
layout: project
title: DistillKit - Knowledge Distillation Framework
---
<p style="text-align: center; font-weight: bold;">
Library/Toolkit • Edge AI • Knowledge Distillation • Quantization  • QAT
</p>
---

![DistillKit Banner](/images/distillkit-banner.jpg)

[🔗 GitHub Repository](https://github.com/bjhaj/DistillKit) |

## 🎯 Project Overview

DistillKit is a comprehensive PyTorch implementation of knowledge distillation combined with model quantization for efficient deep learning. This project demonstrates how to train compact student models using knowledge from larger teacher models, then apply quantization techniques for deployment optimization.

**Key Achievement**: Complete pipeline for model compression achieving 85%+ accuracy retention with 90%+ size reduction.

### 🌟 Key Features

- 🧠 **Knowledge Distillation** with temperature scaling and soft/hard loss combination
- 📱 **Mobile-Friendly Models** using MobileNetV2 architecture optimized for CIFAR-10
- ⚡ **Quantization Support** with both static and quantization-aware training
- 📊 **Comprehensive Evaluation** including accuracy, latency, throughput, and model size
- 🔧 **Modular Design** with separate components for easy experimentation
- 📈 **Performance Tracking** with detailed metrics and visualization tools

## 🏗️ Technical Architecture

### Pipeline Overview

1. **Teacher Training**: Train a large ResNet152 teacher model on CIFAR-10
2. **Knowledge Distillation**: Transfer knowledge from teacher to a smaller MobileNetV2 student
3. **Model Quantization**: Apply static and quantization-aware training (QAT) for deployment
4. **Performance Evaluation**: Compare accuracy, speed, and model size across all variants

### Model Performance Comparison

| Model | Accuracy | Size | Inference Time | Throughput |
|-------|----------|------|----------------|------------|
| Teacher (ResNet152) | 96.8% | 230MB | 45ms | 22 FPS |
| Student (MobileNetV2) | 94.2% | 14MB | 12ms | 83 FPS |
| Quantized Student | 93.8% | 3.8MB | 8ms | 125 FPS |

## 🔬 Technical Implementation

### Knowledge Distillation Process

- **Temperature Scaling**: Adjustable temperature parameter for soft target generation
- **Loss Combination**: Weighted combination of hard and soft losses
- **Feature Alignment**: Intermediate layer knowledge transfer
- **Training Strategy**: Progressive distillation with learning rate scheduling

### Quantization Techniques

- **Static Quantization**: Post-training INT8 quantization
- **Quantization-Aware Training (QAT)**: Training with quantization simulation
- **Dynamic Quantization**: Runtime quantization for inference
- **Custom Quantization**: Layer-specific quantization strategies

## 📊 Results & Analysis

### Compression Results

- **Size Reduction**: 90%+ model size reduction (230MB → 3.8MB)
- **Speed Improvement**: 5.6x faster inference
- **Accuracy Retention**: 97% of original teacher accuracy maintained
- **Memory Efficiency**: 85% reduction in memory footprint

### Deployment Benefits

- **Edge Device Compatible**: Optimized for mobile and embedded systems
- **Real-time Performance**: Achieves real-time inference on resource-constrained devices
- **Energy Efficient**: Reduced computational requirements for battery-powered devices
- **Scalable Architecture**: Easy integration into larger ML pipelines

## 🚀 Applications & Use Cases

### Computer Vision Applications
- **Image Classification**: Efficient image recognition systems
- **Object Detection**: Lightweight detection for mobile apps
- **Edge AI**: Deployment on IoT and embedded devices
- **Real-time Processing**: Video analysis with minimal latency

### Educational Use
- **ML Research**: Framework for distillation experiments
- **Academic Projects**: Teaching tool for model compression
- **Benchmarking**: Standardized evaluation of compression techniques
- **Prototyping**: Rapid development of efficient models

---

*DistillKit provides a comprehensive framework for researchers and practitioners to explore and implement state-of-the-art model compression techniques, making advanced AI accessible on resource-constrained devices.*

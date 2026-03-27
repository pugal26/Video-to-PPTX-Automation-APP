# 🎬 Video to PPTX Automation Pipeline (AI-Powered)

## 🚀 Overview

This project is an **AI-driven automation pipeline** that converts video content into structured PowerPoint presentations. It intelligently extracts frames, removes redundant visuals, analyzes content using deep learning and image processing techniques, and generates concise slide decks.

The system is designed for:
- 📊 Presentation generation from recorded sessions
- 🎓 Lecture / webinar summarization
- 🧠 Visual content analysis
- ⚡ High-performance batch processing

---

## 🧩 Key Features

- 🎥 **Frame Extraction (Time-based Sampling)**  
  Extracts frames at configurable intervals (e.g., 1 frame per second) for full video coverage.

- 🧹 **Duplicate & Near-Duplicate Removal**  
  Removes redundant frames using perceptual hashing and similarity checks.

- 🧠 **AI-Based Image Comparison**  
  Combines deep learning embeddings, structural similarity, and semantic text comparison.

- ⚡ **Hardware Acceleration Support**  
  - GPU (CUDA via PyTorch)  
  - Intel NPU / GPU (via OpenVINO)  
  - CPU fallback

- 🖼️ **Automatic PPT Generation**  
  Creates structured PowerPoint files from filtered frames.

- 📂 **Batch Processing + GUI**  
  Process multiple videos with:
  - Progress tracking
  - ETA estimation
  - Logs and monitoring

- 🧹 **Auto Cleanup (Optional)**  
  Removes intermediate frames after PPT generation to save storage.

---

## 🏗️ System Architecture
# 🎬 Video to PPTX Automation Pipeline (AI-Powered)

## 🚀 Overview

This project is an **AI-driven automation pipeline** that converts video content into structured PowerPoint presentations. It intelligently extracts frames, removes redundant visuals, analyzes content using deep learning and image processing techniques, and generates concise slide decks.

The system is designed for:
- 📊 Presentation generation from recorded sessions
- 🎓 Lecture / webinar summarization
- 🧠 Visual content analysis
- ⚡ High-performance batch processing

---

## 🧩 Key Features

- 🎥 **Frame Extraction (Time-based Sampling)**  
  Extracts frames at configurable intervals (e.g., 1 frame per second) for full video coverage.

- 🧹 **Duplicate & Near-Duplicate Removal**  
  Removes redundant frames using perceptual hashing and similarity checks.

- 🧠 **AI-Based Image Comparison**  
  Combines deep learning embeddings, structural similarity, and semantic text comparison.

- ⚡ **Hardware Acceleration Support**  
  - GPU (CUDA via PyTorch)  
  - Intel NPU / GPU (via OpenVINO)  
  - CPU fallback

- 🖼️ **Automatic PPT Generation**  
  Creates structured PowerPoint files from filtered frames.

- 📂 **Batch Processing + GUI**  
  Process multiple videos with:
  - Progress tracking
  - ETA estimation
  - Logs and monitoring

- 🧹 **Auto Cleanup (Optional)**  
  Removes intermediate frames after PPT generation to save storage.

---

## 🏗️ System Architecture
Video Input → Frame Extraction (FFmpeg) → Duplicate Filtering → Deep Image Analysis (AI) → Decision Engine (Similarity Logic) → PPT Generation → Output (Slides)

---

## ⚙️ Tech Stack

### 🐍 Core Language
- Python 3.10+

---

### 📦 Libraries Used

#### 🔹 Computer Vision & Image Processing
- `opencv-python` – Image processing and frame handling  
- `Pillow` – Image loading and transformation  
- `scikit-image` – Structural similarity (SSIM)

#### 🔹 Deep Learning
- `torch` (PyTorch) – GPU-based inference  
- `torchvision` – Pretrained ResNet50 model  

#### 🔹 AI Acceleration (Optional)
- `openvino` – NPU / Intel GPU inference backend  

#### 🔹 OCR & Text Analysis
- `pytesseract` – Text extraction from images  
- `difflib` – Text similarity comparison  

#### 🔹 Image Similarity
- `imagehash` – Perceptual hashing  

#### 🔹 System & Automation
- `subprocess` – FFmpeg execution  
- `os`, `shutil`, `json` – File and system handling  
- `threading` – Parallel execution (GUI & batch)

#### 🔹 GUI
- `tkinter` – Desktop interface  

---

## 🤖 AI Techniques Used

- 🧠 **Deep Feature Embeddings (ResNet50)**  
  Extracts semantic features from images for comparison.

- 📐 **Cosine Similarity**  
  Measures similarity between image embeddings.

- 🧩 **Structural Similarity Index (SSIM)**  
  Detects visual differences at pixel level.

- 🔍 **Perceptual Hashing (pHash)**  
  Identifies visually similar images efficiently.

- 📝 **OCR-based Text Comparison**  
  Compares textual content inside frames.

- ⚖️ **Hybrid Decision Logic**  
  Combines all signals for accurate duplicate detection.

---

## ⚡ Hardware Utilization

| Component | Usage |
|----------|------|
| GPU (NVIDIA RTX) | Deep learning inference |
| NPU (Intel AI Boost) | OpenVINO inference |
| GPU Decoder (NVDEC) | Video decoding |
| CPU | OCR, SSIM, I/O |

---

## 📦 Installation

```bash
pip install torch torchvision opencv-python pillow scikit-image pytesseract imagehash openvino
```

## 🔧 External Requirements
- FFmpeg (must be added to PATH)
- Tesseract OCR installed

## 📊 Output
- 📁 One .pptx file per video
- 🧹 Optional cleanup of intermediate frames
- 📂 Centralized output directory

## 🎯 Advantages
- ✅ High accuracy in detecting meaningful slide changes
- ⚡ Optimized performance using GPU/NPU
- 🔄 Scalable batch processing
- 🧠 Combines visual + semantic analysis
- 🖥️ User-friendly GUI

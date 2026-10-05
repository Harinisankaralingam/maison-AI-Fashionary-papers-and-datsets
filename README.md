MAISON AI
AI-Powered Fashion E-Commerce with Real-Time Virtual Try-On

MAISON AI is a full-stack fashion e-commerce platform that combines online shopping, AI-powered size recommendation, virtual try-on technology, and real-time fashion visualization.

The project aims to improve online fashion shopping by allowing users to preview garments before purchasing and reducing size-related returns.

---

# Project Overview

Traditional online fashion shopping faces several challenges:

- Customers cannot see how garments look on them.
- Customers often choose incorrect sizes.
- Product images do not represent personalized fitting.
- Existing virtual try-on systems are slow and computationally expensive.

MAISON AI addresses these problems through:

- Fashion E-Commerce Platform
- AI Size Recommendation System
- AI Virtual Try-On System
- Real-Time Webcam-Based Try-On Research
- Future Diffusion-Based Fashion Intelligence

---

# Research Problem

Current virtual try-on systems such as:

- IDM-VTON
- CatVTON
- OOTDiffusion
- VITON-HD
- HR-VITON

can generate highly realistic try-on images.

However, these systems are:

- Image-based
- Computationally expensive
- GPU intensive
- Not suitable for real-time interaction
- Unable to provide live webcam experiences

As a result, users must wait several seconds for a single generated output.

The challenge is to develop a virtual try-on framework that combines:

- Real-time performance
- Accurate body tracking
- Realistic garment behavior
- Low latency
- Practical deployment

while maintaining acceptable visual quality.

---

# Research Gap

Most existing virtual try-on research focuses on:

- Offline image generation
- Diffusion-based synthesis
- High-performance GPUs
- Single-image try-on

Limited research exists on:

- Real-time webcam virtual try-on
- Interactive garment visualization
- Continuous motion tracking
- Temporal consistency
- Lightweight deployment

There is a gap between:

- Highly realistic virtual try-on
- Real-time virtual try-on

MAISON AI investigates how both can be combined.

---

# Proposed Solution

MAISON AI introduces a hybrid virtual try-on framework.

The proposed system combines:

- MediaPipe Pose Tracking
- MediaPipe Segmentation
- Garment Warping
- Landmark Smoothing
- Real-Time Rendering
- Future AI Refinement

The system enables users to:

- Open a webcam
- Select garments
- Visualize garments instantly
- Move naturally
- Capture try-on snapshots

while maintaining low latency and responsiveness.

---

# Novelty

The proposed framework combines:

1. Real-Time Webcam Virtual Try-On
2. Dynamic Garment Alignment
3. Pose-Based Garment Warping
4. Segmentation-Aware Rendering
5. Temporal Landmark Stabilization
6. Future AI Refinement Integration

Unlike traditional virtual try-on systems, MAISON AI prioritizes:

- Real-Time Interaction
- Continuous User Movement
- Lightweight Deployment
- Browser Compatibility
- Future AI Expansion

---

# System Architecture

MAISON AI consists of three major modules:

---

## Frontend

### Technology Stack

- React.js
- Vite
- Tailwind CSS
- Lucide React

### Features

- Product Browsing
- Authentication
- Cart
- Wishlist
- Orders
- AI Virtual Try-On
- User Profile

---

## Backend

### Technology Stack

- Node.js
- Express.js
- MongoDB

### Features

- Authentication
- Product Management
- Order Management
- Cart Management
- Wishlist Management
- User Management
- Admin Dashboard

---

## AI Service

### Technology Stack

- Python
- FastAPI
- MediaPipe
- OpenCV

### Features

- Pose Detection
- Body Tracking
- Size Recommendation
- Virtual Try-On
- Future AI Integration

---

# Phase 1 – AI Fashion E-Commerce

## User Features

- User Registration
- Login & Authentication
- Product Browsing
- Product Search
- Product Details
- Shopping Cart
- Wishlist
- Order Placement
- User Profile

---

## Admin Features

- Product Management
- Order Management
- Dashboard Analytics

---

## AI Features

### AI Size Recommendation

The system recommends clothing sizes based on:

- Height
- Weight
- Body Measurements
- User Preferences

---

## IDM-VTON Fine-Tuning Research

### Base Model

- IDM-VTON

### Fine-Tuning Method

- LoRA (Low-Rank Adaptation)

### Dataset

- Zalando Fashion Dataset
- VITON-Style Garment-Person Pairs

### Training Platform

- Kaggle GPU Environment

### Image Resolution

- 512 × 384

### LoRA Configuration

| Parameter | Value |
|------------|--------|
| Rank (r) | 16 |
| Alpha (α) | 16 |
| Scale (α/r) | 1.0 |
| Training Steps | 100 |

---

## Fine-Tuning Results

| Metric | Step 0 | Step 100 | Improvement |
|----------|---------|---------|---------|
| Validation Loss | 0.0439 | 0.0429 | ↓ 0.0010 |
| Noise Cosine Similarity | 0.9775 | 0.9780 | ↑ 0.0005 |
| SSIM Overall | 0.8843 | 0.8888 | ↑ 0.0045 |
| SSIM Garment Region | 0.7292 | 0.7411 | ↑ 0.0119 |
| PSNR Garment Region | 22.0084 | 22.1441 | ↑ 0.1357 |
| Visual Accuracy | 72.9196% | 74.1083% | ↑ 1.1887% |

---

## Generated Artifacts

- lora_50.pt
- lora_100.pt
- lora_final.pt
- train_log.csv
- val_log.csv
- curves.png
- base_output.png
- lora_output.png
- difference_heatmap.png
- side_by_side_comparison.png

---

# Phase 2 – Real-Time Virtual Try-On

The objective of Phase 2 is to develop a real-time virtual try-on framework that allows users to visualize garments directly through a webcam.

---

## User Workflow

1. Open Webcam
2. Select Garment
3. Body Detection
4. Pose Tracking
5. Garment Alignment
6. Live Visualization
7. Capture Snapshot

---

## Technologies Used

- MediaPipe Pose
- MediaPipe Selfie Segmentation
- OpenCV
- HTML5 Canvas
- WebRTC
- WebAssembly
- FastAPI

Future Integration:

- CatVTON
- IDM-VTON Teacher Pipeline
- AI Refinement Models

---

## Core Components

### Pose Tracking Engine

Tracks:

- Shoulder Landmarks
- Elbow Landmarks
- Wrist Landmarks
- Hip Landmarks

---

### Body Segmentation Engine

Separates:

- Human Body
- Background
- Arms
- Torso

for proper garment rendering.

---

### Garment Warping Engine

Performs:

- Dynamic Scaling
- Rotation Adjustment
- Shoulder Alignment
- Torso Alignment

---

### Temporal Smoothing Engine

Reduces:

- Landmark Jitter
- Frame Flickering
- Garment Instability

during movement.

---

### Real-Time Rendering Engine

Combines:

- Camera Feed
- Pose Landmarks
- Garment Assets
- Segmentation Masks

to create live try-on visualization.

---

# Current Research Status

## Completed

- Literature Survey
- Research Paper Collection
- Dataset Collection
- Phase 1 Development
- IDM-VTON Fine-Tuning
- LoRA Training
- LoRA Evaluation
- AI Service Development
- Pose Tracking Research

---

## In Progress

- Phase 2 Architecture Design
- Real-Time Webcam Pipeline
- MediaPipe Integration
- Garment Warping System
- Segmentation Pipeline

---

## Future Work

- Live AI Virtual Try-On
- CatVTON Integration
- Teacher-Student Distillation
- Temporal Consistency Learning
- Multi-Garment Support
- Mobile Optimization
- Personalized Fashion Assistant
- AI Styling Recommendations

---

# Datasets

The project studies the following datasets:

- VITON-HD
- DressCode
- IDM-VTON Related Datasets
- Zalando Fashion Dataset

These datasets are used for:

- Benchmarking
- Evaluation
- Fine-Tuning
- Comparative Analysis

---

# Evaluation Metrics

## Performance Metrics

- FPS (Frames Per Second)
- Latency
- Memory Usage
- GPU Utilization

---

## Image Quality Metrics

- SSIM
- LPIPS
- PSNR
- Noise Cosine Similarity

---

## User Experience Metrics

- Responsiveness
- Ease of Use
- User Satisfaction

---

# Folder Structure

```text
maison/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── src/
│   ├── uploads/
│   └── package.json
│
└── ai-service/
    ├── models/
    ├── services/
    ├── utils/
    ├── lora_out/
    └── app.py
```

---

# Technologies Used

## Frontend

- React.js
- Vite
- Tailwind CSS

---

## Backend

- Node.js
- Express.js
- MongoDB

---

## AI

- Python
- FastAPI
- MediaPipe
- OpenCV
- IDM-VTON
- LoRA

---

## Tools

- Git
- GitHub
- VS Code
- Kaggle
- Hugging Face

---

 Authors

**Harini Sankaralingam**

B.Tech Information Technology

Maison AI Research & Development


Disclaimer

This project is developed for academic research and educational purposes.

Phase 1 focuses on AI-powered fashion e-commerce and IDM-VTON fine-tuning research.

Phase 2 focuses on investigating real-time virtual try-on systems using pose tracking, segmentation, garment warping, and future AI-assisted refinement techniques.

## Nodirbek Makhtumov

**AI/ML Engineer — Computer Vision · Edge AI · Model Optimization**
Daejeon, South Korea · E-7 visa (authorized to work in Korea)

I build computer vision systems that run on real hardware in the field — not just in a notebook.
Three years shipping production vision to NVIDIA Jetson, Hailo NPU and Android devices, owning
the whole path: model design and training → quantization and pruning → containerized edge deployment.

I don't stop at a headline accuracy number. I validate with per-class metrics, adversarial
robustness testing, and measured per-hardware benchmarks, because an aggregate score hides
the failures that matter in production.

---

### Selected work

**[face-recognition](https://github.com/Nodir0705/face-recognition)** — Face recognition attendance kiosk
Same pipeline implemented three ways — Python/CPU, a C++ port, and Hailo-8 NPU — benchmarked
head-to-head on identical hardware to choose a deployment target.

| Pipeline | Median latency | Jitter | Throughput |
|---|---:|---:|---:|
| Python + CPU (4 threads) | 48.08 ms | ±27 ms | ~21 fps |
| **Hailo-8 NPU** | **5.59 ms** | **±0.29 ms** | **~180 fps** |

8.6× faster, and 95× tighter jitter — the variance win is what actually makes a kiosk feel responsive.
`SCRFD/RetinaFace · ArcFace · InsightFace · Flask · SQLite · Raspberry Pi 5 · Hailo-8`

**[malware_classifier](https://github.com/Nodir0705/malware_classifier)** — Robustness study of an image-based classifier
Built a 98.95% classifier, then spent longer trying to break it. Imperceptible-noise attacks
dropped it to **0%**; full adversarial retraining recovered **89.46% under attack** for a 2-point
clean-accuracy cost. Includes an architecture comparison (most accurate ≠ most robust) and a
documented negative result where metric learning made few-shot detection *worse*.
`ResNet50 · PyTorch · Grad-CAM · MalConv · FastAPI · Docker`

---

### Work

**AI/ML Engineer @ Netvision Telecom** · 2023.04 – present

- Replaced a YOLOv8 backbone with ResNet50 + 1×1 conv adapters and offloaded to the Jetson DLA — **~30% GPU memory reduction**, deployed to vehicle-mounted edge inference
- Built a rail-wheel gap measurement pipeline (RANSAC boundary fitting + custom temporal point stabilization) sustaining **25+ FPS across 4 concurrent camera streams**
- Built a SAM2 temporal-propagation auto-labeling tool — one first-frame prompt labels a whole video, **10×+ faster** dataset construction

**Freelance** · truck parking ID recognition (OCR accuracy **76% → 92%** via a custom deskewing pipeline), face recognition kiosk delivered on Samsung Galaxy Tab

---

### Stack

**Vision** Object Detection · Segmentation · OCR · Multi-Object Tracking · Face Recognition (ArcFace)
**Frameworks** PyTorch · TensorFlow · Ultralytics (YOLO) · OpenCV · InsightFace · Hugging Face
**Optimization** Quantization · Pruning · TensorRT · ONNX Runtime · DLA offloading
**Edge** NVIDIA Jetson (Orin NX / Orin Nano) · Hailo-8 NPU · Raspberry Pi 4/5 · Android
**Serving** Docker · FastAPI · Flask · PostgreSQL · REST
**Languages** Python · C++ · SQL

---

Korean (conversational) · English (fluent) · Russian (conversational)

[LinkedIn](https://linkedin.com/in/nodirbek-makhtumov-03084a194) · stark.developer2877@gmail.com

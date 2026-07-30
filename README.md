# YOLOv8 INT8 Optimization using ONNX Runtime

## Overview

This project demonstrates how to optimize a YOLOv8 object detection model by converting it from PyTorch to ONNX and applying INT8 quantization using ONNX Runtime.

The project compares the original FP32 model and the quantized INT8 model based on:

- Model Size
- Inference Time
- Frames Per Second (FPS)
- Memory Usage

---

## Features

- YOLOv8 Object Detection
- ONNX Model Export
- INT8 Quantization
- Performance Benchmarking
- FP32 vs INT8 Comparison
- Webcam Object Detection

---

## Project Structure

```
benchmark/
camera_node/
detection_node/
models/
results/
assets/

README.md
requirements.txt
LICENSE
```

---

## Technologies Used

- Python
- OpenCV
- Ultralytics YOLOv8
- ONNX
- ONNX Runtime
- PyTorch
- NumPy

---

## Benchmark Results

| Metric | FP32 | INT8 |
|--------|------:|------:|
| Model Size | 12.85 MB | 3.50 MB |
| Inference Time | 66.09 ms | 440.73 ms |
| FPS | 15.13 | 2.27 |
| RAM Usage | 371.24 MB | 454.63 MB |

---

## Installation

Clone the repository

```bash
git clone https://github.com/Haririshx/yolov8-int8-optimization.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Run FP32 Detection

```bash
python detection_node/detector.py
```

---

## Export ONNX Model

```bash
python models/export_model.py
```

---

## Quantize Model

```bash
python models/quantize_model.py
```

---

## Run Benchmarks

```bash
python benchmark/benchmark_fp32.py
```

```bash
python benchmark/benchmark_int8.py
```

---

## Future Improvements

- OpenVINO Optimization
- Raspberry Pi Deployment
- Edge AI Deployment
- ROS2 Integration

---

## License

MIT License

## Project Workflow

![Project Workflow](assets/project_workflow.png)

---

## FP32 Object Detection

![FP32 Detection](assets/fp32_detection.png)

---

## Benchmark Results

![Benchmark Results](assets/benchmark_results.png)

---

## INT8 Object Detection

![INT8 Detection](assets/int8_detection.png)


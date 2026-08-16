# Edge AI on Raspberry Pi 5 — Real-Time Object Detection with LiteRT and YOLO

An implementation and performance report for real-time object detection on a Raspberry Pi 5 — from OS setup and the LiteRT CLI to a live camera detector recording annotated video, with a full system resource analysis under sustained inference load.

| | |
|---|---|
| **Platform** | Raspberry Pi 5 (8 GB) · Raspberry Pi OS 64-bit (aarch64) |
| **Camera** | Camera Module 3 (Sony IMX708, CSI) |
| **Runtime** | LiteRT CLI · Ultralytics 8.4.x · YOLO11n |
| **Date** | 16 August 2026 |
| **Status** | Camera, classification, detection & recording operational |

## Contents

The full write-up (`edge_ai_rpi5_report.pdf`) covers:

1. Objective & Scope
2. System Setup — OS, Access & LiteRT CLI
3. Baseline Inference — Image Classification
4. Object Detection — Model Selection & Pitfalls
5. Live Camera Detector with Video Recording
6. Environment & Colour-Space Fixes
7. Performance Analysis Under Load
8. Findings, Conclusions & Next Steps
9. Appendix: Command & Artifact Reference

## Files

| File | Description |
|---|---|
| [`edge_ai_rpi5_report.pdf`](edge_ai_rpi5_report.pdf) | Full technical report |
| [`detections.mp4`](detections.mp4) | Annotated live-camera object detection recording |
| [`rpi_usage.csv`](rpi_usage.csv) | Per-core CPU, memory, SoC temperature, and clock speed samples during sustained inference |
| [`rpi_usage.png`](rpi_usage.png) | Plotted system resource usage over the benchmark run |

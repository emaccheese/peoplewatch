# peoplewatch

Multi-stream people detection and tracking in C++ with ONNX Runtime, built to run on the device (edge AI).

Personal learning project, work in progress.

## Goals
- Read several video streams at once (files or RTSP)
- Detect people with a pretrained YOLO model in ONNX format
- Track each person across frames and raise alerts (new person, line crossing, loitering)
- Measure and optimize speed on CPU and GPU

## Status
- [x] Step 0: build setup
- [ ] Step 1: multi-stream video pipeline
- [ ] Step 2: person detection
- [ ] Step 3: tracking and alerts
- [ ] Step 4: GPU speed-up

## Requirements
- Linux, CMake 3.16+, a C++17 compiler
- OpenCV
- ONNX Runtime C++ (path set in `CMakeLists.txt`)

## Build
```
cmake -S . -B build
cmake --build build
```

## Videos and models
Test videos and ONNX models are not included in this repo, because they're too large for git. Pretrained models have their own licenses.

## License
MIT

# Face Recognition with YOLO

This repository contains a comprehensive implementation of face recognition using the YOLO (You Only Look Once) model for face detection and recognition. The code provides a complete solution for real-time face detection and recognition.

## Features
- Real-time face detection and recognition using YOLO
- Integration with camera (webcam) for live detection
- Support for static image processing
- Support for video file processing
- Face matching and identification
- Utility functions for image processing

## Directory Structure
```
face-recognition-yolo/
├── README.md                 # Project documentation
├── requirements.txt          # Python dependencies
├── config.py                 # Configuration settings
├── face_detector.py          # YOLO face detection
├── face_recognizer.py        # Face recognition logic
├── main.py                   # Main entry point
├── camera_handler.py         # Real-time camera processing
├── image_handler.py          # Static image processing
├── video_handler.py          # Video file processing
├── utils.py                  # Utility functions
└── data/
    └── known_faces/          # Directory for known face encodings
```

## Installation

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

### Steps
1. Clone this repository
```bash
git clone https://github.com/20221173-code/face-recognition-yolo.git
cd face-recognition-yolo
```

2. Create a virtual environment (optional but recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install required packages
```bash
pip install -r requirements.txt
```

## Usage

### Real-time Camera Detection
```bash
python main.py --mode camera
```

### Process Static Image
```bash
python main.py --mode image --input path/to/image.jpg
```

### Process Video File
```bash
python main.py --mode video --input path/to/video.mp4
```

## Configuration
Edit `config.py` to customize:
- YOLO model version (YOLOv5, YOLOv8, etc.)
- Confidence thresholds
- Face recognition parameters
- Output settings

## Dependencies
- OpenCV (cv2)
- YOLO (ultralytics)
- face-recognition library
- NumPy
- Pillow

## License
This project is licensed under the MIT License.

## Author
Created by: 20221173-code


## Overview

**AI Powered Vehicle Damage Detector** is a computer vision and deep learning application designed to assist vehicle damage inspection by automatically detecting and classifying visible damage in vehicle images.

Powered by a custom-trained YOLO object detection model, the system identifies damage regions and generates bounding boxes, predicted damage categories, and confidence scores. The application demonstrates how deep learning can support digital insurance workflows by reducing repetitive manual inspection tasks.

**Live Demo:** [aicardamagedetection.netlify.app](https://aicardamagedetection.netlify.app/)

## Key Features

- **AI-Powered Damage Detection:** Detects visible vehicle damage using a trained YOLO model.
- **Multiple Damage Detection:** Identifies multiple damage instances within a single image.
- **Bounding Box Localization:** Highlights the approximate location of detected damage.
- **Damage Classification:** Categorizes detected regions into supported damage classes.
- **Confidence Scores:** Provides confidence values for individual predictions.
- **Web-Based Interface:** Enables users to interact with the application through a browser.
- **API Integration:** Supports connecting model inference with a web frontend through a backend API.

## Supported Damage Categories

The model is designed to detect six vehicle damage categories:

- Dent
- Scratch
- Crack
- Glass Shatter
- Lamp Broken
- Tire Flat

## How It Works

1. Upload a vehicle image through the web interface.
2. The backend validates and preprocesses the image.
3. The trained YOLO model performs damage detection.
4. The system generates predicted classes, bounding boxes, and confidence scores.
5. The frontend presents the available detection results.

## Technology Stack

| Category        | Technologies                                                           |
| --------------- | ---------------------------------------------------------------------- |
| Programming     | Python                                                                 |
| Deep Learning   | PyTorch, Ultralytics YOLO                                              |
| Computer Vision | OpenCV, NumPy                                                          |
| Backend API     | FastAPI                                                                |
| Frontend        | HTML, CSS, JavaScript                                                  |
| Deployment      | Netlify for frontend hosting; backend hosting depends on configuration |
| Dataset         | CarDD — Car Damage Detection                                           |

## Dataset and Model Development

The project uses the [CarDD dataset](https://cardd-ustc.github.io/) for vehicle damage detection.

The development pipeline includes dataset exploration, annotation validation, COCO-to-YOLO format conversion, train-validation-test splitting, model training, fine-tuning, and evaluation.

The trained model is intended to identify visible damage patterns in vehicle photographs and support preliminary inspection workflows.

## Potential Applications

- Preliminary insurance claim inspection
- Digital vehicle damage documentation
- Automotive inspection workflows
- Fleet maintenance screening
- AI-assisted vehicle assessment



## Author

**Haseeb Chaudhary**
AI/ML Engineer | Deep Learning | Computer Vision

- **Live Demo:** [AI Insurance Claim Automation](https://aicardamagedetection.netlify.app/)
- **GitHub:** [haseebchaudhary-dev](https://github.com/haseebchaudhary-dev)

---

*Developed to explore practical applications of deep learning and computer vision in vehicle damage inspection and insurance claim workflows.*

# Vanish Webcam — macOS Adaptation

A macOS adaptation of [Vanish Webcam](https://github.com/Nicovic17/vanish_webcam), a Python computer vision project that creates a disappearing effect using webcam input and hand gestures.

This fork adds macOS camera support, a faster white-flash dissolve effect, and reverse dissolve reappearance.

## Features

- macOS webcam support using OpenCV's AVFoundation backend
- Gesture-triggered disappearance
- Reverse dissolve reappearance using a second V gesture
- Fast visual effects with a custom white flash
- Background calibration
- Configurable webcam resolution

## Technologies

- Python
- OpenCV
- Hand gesture recognition
- Pygame, where used by the project

## Requirements

- macOS
- Python 3
- Git
- A working webcam

## Installation

Clone this repository:

```bash
git clone -b macos-vanish-improvements https://github.com/Tushar-7035/vanish_webcam_macos.git
cd vanish_webcam_macos
```

Create a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## Run

```bash
python vanish_cam.py --mode normal --no-virtual-camera --width 480 --height 360
```

Grant camera permission if macOS requests it. Follow the application's instructions for background calibration and gesture recognition.

## How It Works

The application processes webcam frames and detects a configured hand gesture to trigger the disappearance effect. When invisible, a second V gesture triggers the reverse dissolve animation.

A relatively static background and consistent lighting may improve the effect.

## Main Files

- `vanish_cam.py` — main application
- `requirements.txt` — Python dependencies
- Supporting model and asset files — used by the application

## Attribution

This project is based on the original [Vanish Webcam repository](https://github.com/Nicovic17/vanish_webcam). The macOS compatibility and visual-effect modifications are maintained in this fork.

Please consult the original project for its licensing and attribution requirements.

---

Maintained by [Tushar-7035](https://github.com/Tushar-7035).

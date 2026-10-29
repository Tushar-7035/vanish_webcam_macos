# Vanish Webcam — macOS Adaptation

A Python-based computer vision project that creates a disappearing effect using webcam input and hand gesture recognition.

This fork adapts the original [Vanish Webcam](https://github.com/Nicovic17/vanish_webcam) project for macOS and adds a faster dissolve animation with reverse reappearance.

## Features

- **macOS Camera Support** — Uses OpenCV's AVFoundation backend.
- **Gesture-Based Disappearance** — Trigger the effect with a V hand gesture.
- **Reverse Reappearance** — Become visible again using a second V gesture.
- **Fast Dissolve Effect** — Custom white-flash animation for a quicker transition.
- **Background Calibration** — Captures the background before the effect begins.
- **Configurable Resolution** — Set webcam dimensions through command-line options.

## Built With

- Python
- OpenCV
- Computer vision and hand gesture recognition
- Pygame, where used by the original project

## Requirements

- macOS
- Python 3
- Git
- A working webcam

## Installation

Clone the repository:

```bash
git clone -b macos-vanish-improvements https://github.com/Tushar-7035/vanish_webcam_macos.git
cd vanish_webcam_macos
```

Create and activate a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

## Run the Application

```bash
python vanish_cam.py --mode normal --no-virtual-camera --width 480 --height 360
```

Grant camera access if macOS requests it. Follow the application's on-screen instructions for background calibration and gesture recognition.

## How It Works

The application processes webcam frames and uses hand gesture recognition to trigger the disappearance effect. When the person is invisible, a second V gesture triggers the reverse dissolve animation.

A relatively static background and consistent lighting may improve the results.

## Project Structure

- `vanish_cam.py` — Main application
- `requirements.txt` — Python dependencies
- Supporting model and asset files — Required by the application

## Attribution

This project is based on the original [Vanish Webcam repository](https://github.com/Nicovic17/vanish_webcam).

This fork contains macOS compatibility changes and visual-effect modifications. Please consult the original project for its licensing and attribution requirements.

## Future Improvements

- Improve gesture recognition reliability.
- Add more visual-effect customization options.
- Improve setup documentation and cross-platform compatibility.

---

Maintained by [Tushar-7035](https://github.com/Tushar-7035).

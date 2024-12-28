# Vehicle Speed Detection System

This is a Python-based system to detect and measure vehicle speeds from video feeds using OpenCV. The system flags vehicles exceeding a defined speed limit and saves images of violators for further analysis.

## Features

- Real-time speed calculation in km/h using frame-by-frame motion tracking.
- Flags vehicles exceeding the defined speed limit.
- Captures and saves images of vehicles violating the speed limit.

## Requirements

- Python 3.7+
- OpenCV
- NumPy

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/vehicle-speed-detection.git
cd vehicle-speed-detection
exit

Usage
1. Configure the script
Update the video_path variable in the script to point to your video file.
Set the desired speed_limit and output folder in the script.
Example:

python
Copy code
video_path = r"C:\\path\\to\\your\\video.mp4"
speed_limit = 60  # Set the speed limit to 60 km/h
output_folder = "Penalties"  # Folder to store images of violators

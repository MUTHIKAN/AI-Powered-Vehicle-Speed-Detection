# Vehicle Speed Detection System

This Python-based system detects and measures vehicle speeds from video feeds using OpenCV. The system flags vehicles exceeding a defined speed limit and saves images of violators for further analysis.

## Features
- Real-time speed calculation in km/h using frame-by-frame motion tracking.
- Flags vehicles exceeding the defined speed limit.
- Captures and saves images of vehicles violating the speed limit.

## Requirements
- Python 3.7+
- OpenCV
- NumPy

## Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/vehicle-speed-detection.git
    cd vehicle-speed-detection
    ```

2. **Install dependencies:**

    ```bash
    pip install opencv-python-headless numpy
    ```

## Usage

1. **Update configuration:**
   Modify the following variables in the script:
   - `video_path`: Path to the video file you want to analyze.
   - `speed_limit`: Maximum allowed speed in km/h.
   - `output_folder`: Folder where penalty images will be saved.

   Example:
   ```python
   video_path = r"C:\\path\\to\\your\\video.mp4"
   speed_limit = 60  # Set the speed limit to 60 km/h
   output_folder = "Penalties"  # Folder to store images of violators

How It Works
The script reads video frames and detects motion using contour detection.
It tracks objects frame-to-frame to calculate vehicle speeds in km/h.
If a vehicle exceeds the defined speed limit, it is flagged and highlighted.
Images of violating vehicles are saved in the specified output folder.
Example Output
Images of vehicles exceeding the speed limit will be saved in the folder you define in the script. Example folder name: Penalties.

Contributions
Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

Fork the repository.
Create a new branch.
Make your changes.
Submit a Pull Request.
License
This project is licensed under the MIT License.

Vehicle Speed Detection System
This is a Python-based system to detect and measure vehicle speeds from video feeds using OpenCV. It flags vehicles exceeding a defined speed limit and saves images of violators for further analysis.

Features
Real-time speed calculation in km/h using frame-by-frame motion tracking.
Flags vehicles exceeding the speed limit.
Captures and saves images of violating vehicles.
Requirements
Python 3.7+
OpenCV
NumPy

Installation
Step 1: Clone the repository
To clone the repository, run the following command in your terminal:

bash
Copy code
git clone https://github.com/your-username/vehicle-speed-detection.git
cd vehicle-speed-detection
Step 2: Install dependencies
Install the required dependencies by running the following:

bash
Copy code
pip install opencv-python-headless numpy
Usage
Update the video_path variable in the script to the location of your video file.
Set the speed limit and output folder in the script.
Run the script using:
bash
Copy code
python vehicle_speed_detection.py
Images of vehicles exceeding the speed limit will be saved in the "Penalties" folder.

Configuration
You can modify the following parameters in the script:

video_path: Path to the video file you want to analyze.
speed_limit: Maximum allowed speed (in km/h).
output_folder: Folder where images of violators will be saved.
Example:

python
Copy code
video_path = r"C:\\path\\to\\your\\video.mp4"
speed_limit = 60  # Set the speed limit to 60 km/h
output_folder = "Penalties"  # Folder to store penalty images
How It Works
The script reads video frames and detects motion using contour detection.
It tracks objects frame-to-frame and calculates the speed of vehicles in km/h.
Vehicles exceeding the defined speed limit are flagged and highlighted.
Images of violators are saved in the specified output folder for analysis.
Contributions
Contributions are welcome! If you would like to contribute, please fork the repository, create a new branch, and open a Pull Request.

License
This project is licensed under the MIT License.

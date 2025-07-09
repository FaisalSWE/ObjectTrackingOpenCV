# Object Tracking with OpenCV

This project demonstrates **real-time object tracking** using OpenCV and Python by detecting a specific color (red) in a video stream from a webcam.

---

## Objective

Track a red-colored object in real time using your webcam and draw a bounding box around it.

---

## Tools & Libraries

- Python 3.x
- OpenCV
- NumPy

---

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ObjectTrackingOpenCV.git
   cd ObjectTrackingOpenCV
   ```
2. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # or venv\Scripts\activate on Windows
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt

## How to Run

1. Make sure your webcam is connected.

2. Run the Python script:
   ```bash
   python object_tracking.py
   ```
3. Press ESC key to close the window.

## Output Example:

![Tracking Demo](samples/tracking_demo.png)

## How It Works

- Captures frames from webcam
- Converts frame from BGR to HSV color space
- Filters out red color using a predefined HSV range
- Detects contours in the mask
- Draws bounding boxes around objects that match the color
 
## HSV Range for Red

 lower_red = np.array([161, 155, 84])
 upper_red = np.array([179, 255, 255])

You can adjust the range to track other colors.

## Author
FaisalSWE

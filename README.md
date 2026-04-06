

# OpenCV CSRT Object Tracker

A real-time object tracking application built with C++ and OpenCV. This project utilizes the **CSRT (Discriminative Correlation Filter with Channel and Spatial Reliability)** algorithm to track user-selected objects via a webcam feed.

## 🚀 Features

  * **Interactive Selection:** Manually select any object in the video stream using a bounding box.
  * **CSRT Algorithm:** High-accuracy tracking that handles scale changes and partial occlusions effectively.
  * **Real-time Performance:** Low-latency tracking suitable for live webcam applications.

## 🛠 Prerequisites

To build and run this project, you will need:

  * **OpenCV 4.x** (with `opencv_contrib` modules installed).
  * **C++ Compiler** (GCC, Clang, or MSVC).
  * **Qt Creator** (Optional, for using the `.pro` file).

## 📂 Project Structure

  * `main.cpp`: Contains the core logic for webcam capture, ROI selection, and the tracking loop.
  * `Tracker.pro`: Qt Project configuration file for easy building and linking.

## 🔧 Installation & Building

### 1\. Build via Command Line

If you have OpenCV configured with `pkg-config`, you can compile using:

```bash
g++ main.cpp -o tracker `pkg-config --cflags --libs opencv4`
```

### 2\. Build via Qt Creator

1.  Open [Tracker.pro](https://www.google.com/search?q=https://github.com/pranayvaranasi/tracker/blob/main/Tracker.pro) in Qt Creator.
2.  Ensure your build kit is pointed to your OpenCV installation paths.
3.  Click **Build** and **Run**.

## 🎮 How to Use

1.  **Launch the App:** The application will open your default webcam (`device 0`).
2.  **Select ROI:** A static frame will appear. Click and drag your mouse to draw a box around the object you want to track.
3.  **Confirm:** Press **Enter** or **Space** to begin tracking.
4.  **Track:** The yellow box will follow the object. If tracking is lost, a notification will appear on the top-left of the screen.

-----


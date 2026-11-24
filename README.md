<div align="center">
  <!-- Replace 'your_logo.png' with the actual link or path to your drone logo -->
  <img src="./assets/mnm.png" alt="MNM Logo" width="150">
  
  # ZR10 Tactical Gimbal Control
</div>

### The Problem It Solves
Controlling the SIYI ZR10 camera during long-range flight often leads to a major issue: standard control commands can block the network, causing the live H.265 RTSP video stream to stutter, freeze, or drop. 

This application solves that problem. It provides an independent, tactical UI to control the gimbal's precise angles, zoom, and focus using asynchronous UDP packets. It runs smoothly alongside your primary Ground Control Station (GCS) and guarantees **zero interruption** to your critical video stream and telemetry datalink.

### Key Features
* **Zero-Latency Video:** Asynchronous network architecture ensures your video stream never drops or freezes while moving the gimbal.
* **Absolute Precision Control:** Command exact Yaw (±135°) and Pitch (-90° to 25°) angles instantly.
* **Optical Zoom & Focus:** Seamless 1x to 10x optical zoom slider with a one-tap "Auto Focus to Center" capability.
* **Live Syncing:** Instantly fetches and displays the camera's current attitude and zoom state upon launch or refresh.
* **Standalone Operation:** Fully compiled and secured binaries. No dependencies or coding environment required.

### How to Use
1. **Download:** Go to the Releases section and download the standalone executable for your system:
   * **Windows:** Download the `.exe` file.
   * **Linux (Ubuntu):** Download the `.deb` file and install it.
2. **Connect:** Ensure your computer is connected to the SIYI Air Unit/Ground Station network (IP: `192.168.144.X`).
3. **Run:** Open the application. It will automatically sync with the ZR10 camera on port `37260`.
4. **Control:** Use the sliders or manual number inputs to aim the camera, zoom in on targets, and trigger autofocus without disrupting your live video feed.

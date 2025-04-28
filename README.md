# IntelliDrive-Assist
# 🚗 Advanced Driver Assistance System (ADAS)
<h2>Project Overview</h2>

<p>
  This project is developed as part of our Final Year Engineering curriculum. 
  It focuses on implementing an Advanced Driver Assistance System (ADAS) using modern computer vision techniques. 
  The system is divided into four modules: Vehicle Detection and Collision Warning, Lane Detection, Traffic Sign Recognition, and Driver Drowsiness Detection.
  We have utilized state-of-the-art methods such as YOLOv8, UFLD, Canny Edge Detection, Hough Transform, and Dlib's facial landmark detector to create a robust and efficient ADAS solution.
</p>

<h2>Team Members and Roles</h2>

<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Role</th>
      <th>Contributions</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><strong>M. N Maneesha</strong> (Team Lead)</td>
      <td>Lead Developer, Research Coordinator</td>
      <td>Implemented Vehicle Detection and Collision Warning System (Module 1), Lane Detection (Module 2), wrote the conference paper, handled communication for paper publication (ICICT to IEEE)</td>
    </tr>
    <tr>
      <td><strong>S. Ashish Raj</strong></td>
      <td>Developer</td>
      <td>Implemented Traffic Sign Recognition System (Module 3)</td>
    </tr>
    <tr>
      <td><strong>S. Chandanapriya</strong></td>
      <td>Developer</td>
      <td>Implemented Driver Drowsiness Detection System (Module 4)</td>
    </tr>
    <tr>
      <td><strong>Md. Zaheer</strong></td>
      <td>Documentation and Support</td>
      <td>Assisted in documentation, project reports, and presentation materials</td>
    </tr>
    <tr>
      <td><strong>V. Praveen Prakash</strong></td>
      <td>Research Assistant</td>
      <td>Assisted in dataset preparation, testing, and performance evaluation</td>
    </tr>
  </tbody>
</table>


An AI-powered, sensor-free ADAS solution for enhancing road safety using real-time vehicle detection, traffic sign recognition, lane detection, and driver drowsiness monitoring — implemented entirely in Python with deep learning models.

![ADAS Overview](assets/adasgit.jpg)

---

## 📌 Key Features

- 🔍 **Vehicle Detection & Collision Warning:** YOLOv8 detects vehicles; Apple's Depth Pro estimates inter-vehicle distances.
- 🛑 **Traffic Sign Recognition:** Real-time classification of traffic signs using YOLOv8.
- 🛣️ **Lane Detection:** Ultra-Fast Lane Detection (UFLD) to identify lane boundaries and assist in lane keeping.
- 😴 **Driver Drowsiness Detection:** Detects fatigue using Dlib-based facial landmark tracking and CNN for eye state detection.
- ⚙️ **Real-Time Performance:** Achieves ~25 FPS on Google Colab (Tesla T4 GPU).

---

## 🧠 Tech Stack

| Module                   | Frameworks/Libraries Used         |
|--------------------------|-----------------------------------|
| Object Detection         | YOLOv8, PyTorch, OpenCV           |
| Lane Detection           | UFLD, OpenCV                      |
| Drowsiness Monitoring    | Dlib, TensorFlow, SciPy           |
| Depth Estimation         | Apple Depth Pro (simulated)       |
| Inference Pipeline       | Python, NumPy, Google Colab       |

---

## 📷 Visual Output Examples

| Case | Scenario Description                      | Model Response                                      |
|------|-------------------------------------------|-----------------------------------------------------|
| 1️⃣   | Clear Road with Visible Vehicles          | All vehicles detected with high confidence.         |
| 2️⃣   | Heavy Traffic Conditions                  | Overlapping vehicles tracked with NMS.              |
| 3️⃣   | Nighttime Driving                         | Visibility enhanced; reflective features detected.  |
| 4️⃣   | Rainy Weather with Water Splashes         | Partial occlusion handled with shape consistency.   |

### 🖼️ Output Samples

<h3 align="center">🚗 Vehicle Detection & Collision Warning</h3>
<p align="center">
  <img src="assets/collisiongit.jpeg" width="45%" />
</p>

<h3 align="center">🛣️ Lane Detection</h3>
<p align="center">
  <img src="assets/lanedetect-op.png" width="45%" />
</p>

<h3 align="center">🚧 Traffic Sign Recognition</h3>
<p align="center">
  <img src="assets/trafficgit.jpeg" width="45%" />
</p>

<h3 align="center">😴 Driver Drowsiness Detection</h3>
<p align="center">
  <img src="assets/drivergit.jpeg" width="45%" />
</p>


---

## 📊 Computational Performance

| Module                | Complexity             | Avg Latency (ms) |
|----------------------|------------------------|------------------|
| YOLOv8 Detection      | O(n) per frame         | 15               |
| UFLD Lane Detection   | O(h × w)               | 8                |
| Depth Estimation      | O(k) pixels/frame      | 20               |
| Drowsiness Monitoring | O(m) facial landmarks  | 10               |

---
## 🎤 Project Presentation

You can view our conference presentation slides here:  
[📑 ADAS Project Presentation (Google Drive)](https://drive.google.com/file/d/111kHaJihyEma1fWr3vX19TsWF7VlaGE6/view?usp=drive_link)

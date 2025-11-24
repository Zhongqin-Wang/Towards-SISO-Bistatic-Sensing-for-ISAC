# 🚀 Towards SISO Bistatic Sensing for ISAC
Clock asynchrony in bistatic sensing remains a major challenge, as independently clocked and spatially separated transceivers introduce random phase offsets in the Channel State Information (CSI), which must be compensated for accurate sensing. This work presents WiDFS 3.0, a lightweight bistatic Single-Input Single-Output (SISO) sensing framework that enables accurate delay-Doppler estimation from distorted CSI, requiring only a single antenna at both transmitter and receiver. A self-referencing cross-correlation (SRCC) method is proposed for random phase removal by constructing a reference signal from the original CSI, followed by a delay-domain beamforming for interference suppression and beamformed Doppler Fast Fourier Transform (FFT) for unambiguous motion extraction. Our experiments show that WiDFS 3.0 achieves accurate delay-Doppler parameter estimation, with performance comparable to or even surpassing that of prior multi-antenna methods. Based on the extracted robust features, even when using compact neural networks such as the embedded-friendly MobileViT XXS with only 1.3 million parameters, WiDFS 3.0 achieves strong robustness and generalization capability. It consistently outperforms commonly- used features such as CSI amplitude, raw mirrored Doppler, and multi-receiver aggregated Doppler, as validated on extensive single- and multi-target activity datasets.  
<!-- 📌 Code will be uploaded soon — stay tuned! -->

**Developed at:** University of Technology Sydney (UTS), Australia  
**Author:** Zhongqin Wang (zhongqin.wang@uts.edu.au)  
**Google Scholar:** https://scholar.google.com/citations?hl=en&user=F9UMFwIAAAAJ&view_op=list_works&sortby=pubdate

---

## 📄 Reference  
Zhongqin Wang, J. Andrew Zhang, Kai Wu, Min Xu, and Y. Jay Guo, *“Towards SISO Bistatic Sensing for ISAC,”* arXiv:2508.12614, 2025.  
(Reference applies to all demos of WiDFS 3.0 below.)

---

# 📹 Demo Videos of WiDFS 3.0

## **1. Real-Time Bistatic Passive Sensing via Intel 5300 NIC (Static & Dynamic Target Tracking and Vital Sign Monitoring)**  
🔗 **Video:** https://www.youtube.com/watch?v=ldF2vq5x0P4  

This demo presents **WiDFS 3.0**, a real-time **bistatic passive WiFi sensing framework** built on the Intel 5300 NIC.  
The system performs **moving target tracking**, **static object localization**, and **vital sign monitoring** using Channel State Information (CSI).

### **Sensing Functions**
- Motion Detection: Detects human presence or movement  
- Moving Target Localization: Estimates XY position, velocity, and acceleration  
- Tracking: Maintains target trajectory; detects entry & exit  
- Static Target Localization: Determines XY coordinates of stationary objects  
- Vital Sign Estimation: Extracts respiration and heartbeat waveforms  
  - Example: Respiration ≈ 11/min, Heartbeat ≈ 65/min (rest)

---

## **2. Real-Time Single-Antenna Bistatic Gesture Recognition via Intel 5300 NIC**  
🔗 **Video:** https://www.youtube.com/watch?v=I_dquPkgXbE  

This demo shows WiDFS 3.0 performing real-time **motion detection** and **gesture recognition** using a single-antenna bistatic WiFi setup (1Tx-1Rx).  

### **Sensing Functions**
- Motion Detection: Detects walking and hand movements  
- Gesture Recognition: Recognizes gestures such as clapping and zigzag motions  

---

## **3. Real-Time Single-Antenna Bistatic Sensing via ESP32 (Unlocked AGC Mode)**  
🔗 **Video:** https://www.youtube.com/watch?v=SdnUunW9ueA  

This demo presents the **ESP32 implementation** of WiDFS 3.0 using **unlocked AGC mode**, enabling low-cost and flexible real-time CSI sensing. It demonstrates the feasibility of commodity IoT devices for passive wireless perception.

### **Sensing Functions**
- Motion Detection: Detects human and hand movements  
- Vital Sign Estimation: Extracts respiration and heartbeat signals in real time  

---

# 🌟 Potential Applications

WiDFS 3.0 enables a wide range of practical wireless sensing applications:

- Indoor localization & people tracking  
- Smart home & healthcare monitoring (contactless respiration/heartbeat)  
- Elderly fall detection & activity recognition  
- Security: intrusion detection & presence sensing  
- Gesture interfaces & HCI  
- Occupancy estimation for buildings  
- Robotics & autonomous sensing  
- Low-cost IoT-based environmental perception  

---

# 🎥 Additional Demos

### **4. Real-Time Bistatic Multi-Target WiFi Tracking**  
🔗 **Video:** https://youtu.be/DVib9wOY48k  

### **5. Single-Target Real-Time Passive WiFi Tracking**  
🔗 **Video:** https://youtu.be/UvceJ2OnJmE  

Reference:
1. WiDFS 2.0: Zhongqin Wang, J. Andrew Zhang, Haimin Zhang, Min Xu, and Y. Jay Guo, *“Passive Human Tracking with WiFi Point Clouds,”* IEEE Internet of Things Journal, vol. 12, no. 5, pp. 5528–5543, 2025.
2. WiDFS: Zhongqin Wang, J. Andrew Zhang, Min Xu, and Y. Jay Guo, *“Single-Target Real-Time Passive WiFi Tracking,”* IEEE Transactions on Mobile Computing, vol. 22, no. 6, pp. 3724–3742, 2023.

### **6. Water Level Sensing via Communication Signals in a Bi-Static System**  
🔗 **Video:** https://youtu.be/Mh-VjUEpSuY  

Reference:
Zhongqin Wang, J. Andrew Zhang, Kai Wu, and Y. Jay Guo, "Water Level Sensing via Communication Signals in a Bi-Static System," arXiv preprint arXiv:2505.19539, 2025.

---

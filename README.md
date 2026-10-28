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

## 📚 Related Papers: WiFi Tracking, Bistatic and Environmental Sensing

Listed from newest to oldest following the publication order on Google Scholar, these papers cover passive WiFi tracking, CSI/RSSI-based bistatic sensing, micro-Doppler construction, reservoir computing, and human-to-environmental ISAC. The multi-target tracking demonstration is listed separately below.

### 1. CoTrack: Cross-Room Passive WiFi Tracking

Heping Wang, Zhongqin Wang, Henk Wymeersch, and J. Andrew Zhang, *“Cross-Room Passive WiFi Tracking: Joint Estimation of Target Trajectory and Virtual Transmitter Location,”* **arXiv:2609.34797**, 2026.  
**Focus:** Jointly estimating a human trajectory and virtual transmitter location for passive tracking across rooms without requiring the transmitter position.  
🔗 [Preprint](https://arxiv.org/abs/2609.34797)

### 2. Bistatic Passive Sensing via CSI Power

Zhongqin Wang, J. Andrew Zhang, Kai Wu, Kuangda Chen, Min Xu, and Y. Jay Guo, *“Bistatic Passive Sensing via CSI Power,”* **IEEE Transactions on Communications**, 2026.  
**Focus:** CSI-power-domain delay–angle–Doppler processing for passive tracking and position-refined micro-Doppler sensing.  
🔗 [Preprint](https://arxiv.org/abs/2511.22144) · [Google Scholar](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=F9UMFwIAAAAJ&citation_for_view=F9UMFwIAAAAJ:blknAaTinKkC)

### 3. Ambiguity-Resolved Micro-Doppler Construction for Asynchronous Bistatic Sensing

Yiyi Xu, Zhongqin Wang, Kai Wu, and J. Andrew Zhang, *“Ambiguity-Resolved Micro-Doppler Construction for Asynchronous Bistatic Sensing,”* **arXiv:2607.20108**, 2026.  
**Focus:** Resolving mirror ambiguity and suppressing residual by-products in asynchronous bistatic CSI to construct robust micro-Doppler features for WiFi sensing.  
🔗 [Preprint](https://arxiv.org/abs/2607.20108)

### 4. WiFi Sensing via Reservoir Computing

Heping Wang, Zhongqin Wang, and J. Andrew Zhang, *“WiFi Sensing via Reservoir Computing,”* **arXiv:2607.20103**, 2026.  
**Focus:** ReWiS combines structured micro-Doppler features with a graph-coupled reservoir, adapting to new domains by updating only a lightweight readout.  
🔗 [Preprint](https://arxiv.org/abs/2607.20103)

### 5. WiRSSI: Rethinking RSSI for WiFi Sensing

Zhongqin Wang, J. Andrew Zhang, Kai Wu, and Y. Jay Guo, *“Rethinking RSSI for WiFi sensing,”* **npj Wireless Technology**, vol. 2, article 45, 2026.  
**Focus:** RSSI-only passive human tracking and motion sensing using Doppler, angle-of-arrival, and amplitude-derived delay cues from commodity WiFi measurements.  
🔗 [Paper](https://doi.org/10.1038/s44459-026-00053-y)

### 6. WiFi Passive Human Tracking With Multi-Point Differential CSI

Heping Wang, Zhongqin Wang, and J. Andrew Zhang, *“WiFi Passive Human Tracking With Multi-Point Differential CSI,”* **IEEE Transactions on Mobile Computing**, vol. 25, no. 9, pp. 14972–14987, 2026.  
**Focus:** Multi-point CSI differencing and tensor decomposition for joint Doppler, range, and angle estimation, with an unscented Kalman filter for tracking.  
🔗 [Paper](https://doi.org/10.1109/TMC.2026.3688462) · [Demo](https://www.youtube.com/watch?v=DjAdpB8YxgM)

### 7. ISAC: From Human to Environmental Sensing

Kai Wu, Zhongqin Wang, Shu-Lin Chen, J. Andrew Zhang, and Y. Jay Guo, *“ISAC: From Human to Environmental Sensing,”* **IEEE Journal of Selected Topics in Electromagnetics, Antennas and Propagation**, 2025.  
**Focus:** A review of ISAC signal mechanisms and features spanning human localization, activity recognition, vital signs, rainfall, soil moisture, and water-level sensing.  
🔗 [Preprint](https://arxiv.org/abs/2507.13766)

### 8. WiDFS 2.0: Passive Human Tracking With WiFi Point Clouds

Zhongqin Wang, J. Andrew Zhang, Haimin Zhang, Min Xu, and Y. Jay Guo, *“Passive Human Tracking With WiFi Point Clouds,”* **IEEE Internet of Things Journal**, vol. 12, no. 5, pp. 5528–5543, 2025.  
**Focus:** Extracting Doppler, angle, range, and signal-to-noise features from different body parts as WiFi point clouds, followed by trajectory tracking.  
🔗 [Paper](https://doi.org/10.1109/JIOT.2024.3487193)

### 9. WiDFS: Single-Target Real-Time Passive WiFi Tracking

Zhongqin Wang, J. Andrew Zhang, Min Xu, and Y. Jay Guo, *“Single-Target Real-Time Passive WiFi Tracking,”* **IEEE Transactions on Mobile Computing**, vol. 22, no. 6, pp. 3724–3742, 2023.  
**Focus:** Real-time device-free human tracking using Doppler, angle-of-arrival, and reflection-distance estimates from commodity WiFi CSI.  
🔗 [Paper](https://doi.org/10.1109/TMC.2022.3141115) · [Preprint](https://arxiv.org/abs/2109.06006) · [Demo](https://youtu.be/UvceJ2OnJmE)

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

**By:** Heping Wang and Zhongqin Wang, 2025.  
A real-time bistatic WiFi demonstration of tracking multiple targets.  
🔗 [Google Scholar demo entry](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=F9UMFwIAAAAJ&citation_for_view=F9UMFwIAAAAJ:qUcmZB5y_30C)

### **5. Single-Target Real-Time Passive WiFi Tracking**  
🔗 **Video:** https://youtu.be/UvceJ2OnJmE  

**Reference:** WiDFS, *“Single-Target Real-Time Passive WiFi Tracking,”* IEEE Transactions on Mobile Computing, 2023. See the linked paper and full citation in the related papers section above.

### **6. Water Level Sensing via Communication Signals in a Bi-Static System**  
🔗 **Video:** https://youtu.be/Mh-VjUEpSuY  

Reference:
Zhongqin Wang, J. Andrew Zhang, Kai Wu, and Y. Jay Guo, "Water Level Sensing via Communication Signals in a Bi-Static System," arXiv preprint arXiv:2505.19539, 2025.

---

### **7. WiFi Passive Human Tracking With Multi-Point Differential CSI**  
🔗 **Video:** https://www.youtube.com/watch?v=DjAdpB8YxgM  

**By:** Heping Wang and Zhongqin Wang, 2026.  
A demonstration of passive human tracking using multi-point differential CSI.  
**Reference:** Heping Wang, Zhongqin Wang, and J. Andrew Zhang, *“WiFi Passive Human Tracking With Multi-Point Differential CSI,”* IEEE Transactions on Mobile Computing, 2026.  
🔗 [Paper](https://doi.org/10.1109/TMC.2026.3688462)

---

# AI-Women-Safety-System
An AI-powered real-time women safety system using YOLOv5, pose estimation, SOS gesture/voice detection, and anomaly analysis for proactive threat identification.
# 🔐 AI-Women-Safety-System

An AI-powered real-time safety solution for women using advanced computer vision techniques. This system detects threats proactively using YOLOv5 object detection, pose estimation, SOS gesture/voice analysis, and anomaly detection.

---

## 🚀 Features

- ✅ Real-time object detection using YOLOv5
- 🧍‍♀️ Pose estimation with OpenPose or PoseNet
- ✋ SOS gesture and distress voice recognition
- ⚠️ Anomaly detection to identify abnormal behavior
- 🔔 Instant alert system (SMS/email-ready)
- 🔒 Privacy-focused (edge processing & anonymized data)


## 🏗️ System Architecture

             +----------------------+
             |    Video Input (CCTV)|
             +----------+-----------+
                        |
                        v
         +--------------+----------------+
         |  Edge Device (Preprocessing)  |
         |  - Frame extraction           |
         |  - Privacy filtering          |
         +--------------+----------------+
                        |
                        v
     +------------------+---------------------+
     | AI Processing Unit (Deep Learning)     |
     | - YOLOv5 Object Detection              |
     | - Pose Estimation (OpenPose / PoseNet) |
     | - Voice & Gesture Analysis             |
     | - Anomaly Detection (SVM/Autoencoders) |
     +------------------+---------------------+
                        |
                        v
         +--------------+---------------+
         |  Decision Engine             |
         |  - Risk scoring              |
         |  - Threat classification     |
         |  - Generate alert payload    |
         +--------------+---------------+
                        |
                        v
         +--------------+----------------------+
         | Alert System                         |
         | - Notify police/emergency contacts   |
         | - Trigger lights/alarms              |
         | - Log and archive event              |
         +--------------------------------------+


## 🛠️ Tech Stack

| Component           | Tool/Library         |
|--------------------|----------------------|
| Object Detection   | YOLOv5               |
| Pose Estimation    | OpenPose / PoseNet   |
| Anomaly Detection  | One-Class SVM / Autoencoders |
| Voice Detection    | PyDub, SpeechRecognition |
| Alert System       | SMTP / Twilio-ready  |
| Language           | Python               |

---

## 📂 Project Structure
women_safety_ai/
├── main.py
├── data/
├── models/
│ ├── yolo_model.py
│ └── anomaly_detector.py
├── utils/
│ ├── video_processing.py
│ └── alert_system.py
├── requirements.txt
└── README.md


.

📦 VIII. INSTALLATION & BACKEND SETUP
This section provides step-by-step instructions to install and run the AI-Driven Women Safety Analytics System on a local machine. The project is built in Python and uses computer vision, deep learning, and real-time alert modules.
| Component        | Requirement             |
| ---------------- | ----------------------- |
| Operating System | Windows / Linux / macOS |
| Python Version   | 3.8 or higher           |
| Disk Space       | Min 1 GB free           |
| Optional         | GPU with CUDA for speed |

2. Folder Structure
women_safety_ai/
├── main.py
├── requirements.txt
├── models/
│   ├── yolo_model.py
│   └── anomaly_detector.py
├── utils/
│   ├── video_processing.py
│   └── alert_system.py
├── data/
│   └── sample_dataset_description.txt
├── README.md
└── LICENSE

3. Clone the Repository
 git clone https://github.com/yourusername/AI-Women-Safety-System.git
cd AI-Women-Safety-System/women_safety_ai

4. Install Dependencies
 pip install -r requirements.txt
  
▶️ 5. Run the Project
python main.py



⚙️ BACKEND MODULES EXPLAINED
🧠 A. models/yolo_model.py
Loads YOLOv5 model using TorchHub

Detects people and objects in video frames

Returns bounding boxes with class labels

🧍‍♀️ B. models/anomaly_detector.py
Trained One-Class SVM or autoencoder

Flags suspicious behavior like loitering, pacing

Learns normal behavior from environment
environment

🎥 C. utils/video_processing.py
Reads video frame-by-frame from webcam or file

Preprocesses input (resize, normalize)

🚨 D. utils/alert_system.py
Sends alerts when threats are detected

Can be extended to email, SMS (Twilio), app notifications

🧩 E. main.py
Central script that connects all modules
Real-time loop for object detection, pose recognition, SOS detection, and alert triggering


📍 Note:
To test the system, use sample videos or CCTV feed simulation.

Replace placeholder models with trained versions.

Add voice detection module (SpeechRecognition, PyDub) if required

⏳ IX. PROJECT TIMELINE
| **Phase**                            | **Duration** | **Key Activities**                                                                                                                                                                        |
| ------------------------------------ | ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Phase 1: Research & Design**       | Weeks 1–3    | - Define objectives and scope  <br> - Literature survey  <br> - Select models (YOLOv5, OpenPose, etc.) <br> - Design system architecture                                                  |
| **Phase 2: Core Implementation**     | Weeks 4–7    | - Implement YOLOv5 for object & gender detection  <br> - Add pose estimation  <br> - Integrate gesture & voice-based SOS detection <br> - Build anomaly detection model (SVM/Autoencoder) |
| **Phase 3: Alert System & Mapping**  | Weeks 8–10   | - Develop real-time alert generation logic  <br> - Send notifications to authorities  <br> - Predict crime zones using historical + real-time data                                        |
| **Phase 4: Testing & Documentation** | Weeks 11–14  | - System testing and refinement  <br> - Evaluate model accuracy  <br> - Capture sample outputs  <br> - Finalize report, documentation, and GitHub upload                                  |

.

🎯 X. EXPECTED OUTCOMES
The AI-Driven Women Safety Analytics System is designed to proactively detect and respond to public safety threats using real-time analysis. The following outcomes are expected upon successful implementation:
| **Category**                      | **Expected Outcome**                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| **Real-Time Detection**           | Detect threats such as stalking, aggressive behavior, or crowding near isolated women with >93% accuracy using YOLOv5 and pose estimation. |
| **SOS Recognition**               | Recognize predefined emergency gestures (e.g., raised arms, crossed wrists) with up to 96% accuracy.                                       |
| **Voice-Based Alerting**          | Detect voice-based distress cues (e.g., screams, urgent tones) with \~94% accuracy using trained audio models.                             |
| **Anomaly Detection**             | Identify unusual behavior (e.g., loitering, pacing) using one-class SVMs or autoencoders.                                                  |
| **Automatic Alert System**        | Send real-time alerts to emergency contacts/law enforcement without manual user input.                                                     |
| **Predictive Crime Mapping**      | Generate heatmaps to predict high-risk zones with ≈92% accuracy based on live and historical data.                                         |
| **Privacy-Preserving AI**         | Ensure anonymized surveillance data, encrypted alerts, and bias-mitigated model training.                                                  |
| **Emergency Response Efficiency** | Reduce average emergency response time by enabling faster detection and multi-channel alerts.                                              |


📌 TODOs
 Integrate OpenPose or PoseNet

 Add voice recognition module

 Finalize real-time alert trigger

 Add deployment notebook (Colab / Streamlit)
  


📜 License
This project is licensed under the MIT License.

.

🙌 Acknowledgements
YOLOv5 by Ultralytics

OpenPose by CMU

Community datasets and contributors working for safer public spaces.

:

📬 XI. CONTACT INFORMATION
For any queries, contributions, or collaboration related to this project, feel free to reach out:

👩‍💻 Name: Sampada Vikrant Kabule

🔗 LinkedIn: linkedin.com/in/sampada-kabule-4728642b3

📧 Email: sampadakabule03@gmail.com










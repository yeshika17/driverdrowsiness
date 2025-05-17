# 🚗 Driver Drowsiness Detection
A real-time computer vision project using OpenCV and deep learning to detect driver drowsiness through eye closure and alert the user with an alarm to prevent accidents

 📌 Features
* Real-time webcam monitoring
* Eye detection using Haar cascades or facial landmarks
* Eye aspect ratio (EAR) based drowsiness detection
* Audible alarm when drowsiness is detected
* Simple and intuitive interface

 🖥️ Tech Stack
* Python
* OpenCV
* Dlib / Mediapipe (for facial landmark detection)
* Scipy / NumPy
* Pygame or playsound (for alarm)

 🧠 How It Works
1. Face & Eye Detection: Detects facial landmarks (especially eyes).
2. Eye Aspect Ratio (EAR): Calculates EAR to determine if the eyes are closed.
3. Threshold Check :If EAR remains below a threshold for a number of consecutive frames, an alarm is triggered.
4. Alarm System : Notifies the user using a sound alert.
   
📦 Installation
 1. Clone the repository

git clone https://github.com/yeshika17/driver-drowsiness-detection.git
cd driver-drowsiness-detection


 2. Create a virtual environment (optional but recommended)

python -m venv venv
source venv/bin/activate    # On Windows: venv\Scripts\activate

 3. Install dependencies
pip install -r requirements.txt

🚀 Usage
python drowsiness_detection.py
Make sure your webcam is connected and accessible.

 📁 Project Structure

driver-drowsiness-detection/
│
├── drowsiness_detection.py     # Main script
├── alarm.wav                   # Alarm sound
├── shape_predictor_68_face_landmarks.dat  # Pre-trained facial landmark model (if using dlib)
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation
 🧪 Requirements
* Python 3.7+
* Webcam
* (Optional) Pretrained model files:

  * shape_predictor_68_face_landmarks.dat (for Dlib-based detection)
  * Haar cascade files (for OpenCV)

## 🙋‍♂️ Acknowledgements

* [OpenCV](https://opencv.org/)
* [Dlib](http://dlib.net/)
* [Tereza Soukupova & Jan Cech - Eye Aspect Ratio Paper](https://vision.fe.uni-lj.si/cvww2016/proceedings/papers/05.pdf)

---


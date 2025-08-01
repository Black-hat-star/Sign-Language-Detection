# 🧠 Sign Language Detection

This project aims to bridge the communication gap between the hearing and speech impaired and others by providing a tool that detects and translates **sign language gestures into text**. Built using Python, OpenCV, and Deep Learning, this tool supports real-time gesture recognition via a webcam.

---

## 🔑 Features

- 🎥 **Data Collection**: Capture gesture images from webcam using `collectdata.py`.
- 🧹 **Preprocessing**: Clean and structure images for training.
- 🧠 **Model Training**: Train using `trainmodel.py` (Keras/TensorFlow backend).
- ⚡ **Real-Time Detection**: Recognize signs live via webcam using `app.py`.
- 📦 **Modular Codebase**: Separate modules for data handling, functions, and commands.
- 📝 **Logging**: Application logs stored in the `Logs/` folder.

---

## 📁 Project Structure

| File/Folder      | Description                                 |
|------------------|---------------------------------------------|
| `app.py`         | Main application for real-time sign detection |
| `collectdata.py` | Script to collect gesture images via webcam |
| `trainmodel.py`  | Trains the sign detection model             |
| `model.h5`       | Trained model weights                       |
| `model.json`     | Model architecture                          |
| `function.py`    | Helper functions used across scripts        |
| `data.py`        | Data management and processing utilities    |
| `commands.txt`   | List of supported gestures                  |
| `Image/`         | Raw captured gesture images                 |
| `Logs/`          | Log files for monitoring/debugging          |
| `MP_Data/`       | Preprocessed gesture dataset                |
| `__pycache__/`   | Python cache files                          |
| `.DS_Store`      | System file (can be ignored)                |

---

## 📦 Requirements

- Python 3.x  
- TensorFlow  
- Keras  
- OpenCV (opencv-python)  
- NumPy  

Install dependencies:

```bash
pip install numpy opencv-python tensorflow keras
```
🚀 Usage
📸 Step 1: Collect Gesture Data
```
python collectdata.py
```
🧠 Step 2: Train the Model
```
python trainmodel.py
```
This will generate model.h5 and model.json after training.

👋 Step 3: Run Real-Time Detection
```
python app.py
```
📄 View Supported Commands
Open commands.txt to see a list of recognizable gesture commands.

💡 Notes:

Ensure your webcam is accessible before running the scripts.

Avoid duplicate data collection by capturing each gesture clearly and only once.

Logs are stored inside the Logs/ directory for troubleshooting and tracking.



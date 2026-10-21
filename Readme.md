# 🔍 DeepFake Detective: AI-Powered Image Authenticity Detector

[![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)](https://www.tensorflow.org/)
[![Accuracy](https://img.shields.io/badge/Accuracy-99.996%25-brightgreen.svg)](https://github.com/Ananya419/DeepFakeDetection)
[![Flask](https://img.shields.io/badge/Flask-2.0+-green.svg)](https://flask.palletsprojects.com/)

## 📋 Table of Contents
- [Project Structure](#project-structure)
- [Overview](#overview)
- [Features](#features)
- [Technical Architecture](#technical-architecture)
- [Installation](#installation)
- [Usage](#usage)
- [API Reference](#api-reference)
- [Creators](#creators)
- [License](#license)

## 📁 Project Structure
```
/project-folder
├── app.py                # Flask backend server
├── model.py              # CNN training script
├── Data_Preparation.py   # Dataset loading and preprocessing
├── requirement.txt       # Python dependencies
├── saved_model/         # TensorFlow SavedModel directory
├── templates/
│   └── index.html       # Main webpage template
├── static/
│   └── style.css        # CSS styling
└── Readme.md            # Project documentation
```

## 🎯 Overview
DeepFake Detective is a web-based application that utilizes deep learning to detect fake images with an exceptional accuracy of 99.996%. Built with Flask and TensorFlow, it provides a user-friendly interface for real-time image authenticity verification.

## ✨ Features
- **Real-time Analysis**: Instant image processing and results
- **User-friendly Interface**: Clean and intuitive web design
- **High Accuracy**: 99.996% accurate detection rate
- **Responsive Design**: Works seamlessly across devices
- **Detailed Reports**: Comprehensive analysis results

## 🏗️ Technical Architecture

### Backend
- **Flask Framework**: Handles HTTP requests and serves the application
- **TensorFlow Model**: Pre-trained model for image classification
- **Python 3.x**: Core programming language

### Frontend
- **HTML5**: Structure and content
- **CSS3**: Styling and responsiveness
- **JavaScript**: Client-side interactions and API calls

### Model
- TensorFlow SavedModel format
- CNN architecture optimized for image authenticity detection
- Trained on extensive dataset of real and fake images

## 📥 Installation

1. **Clone the Repository**
```bash
git clone https://github.com/shri-ram07/DeepFakeDetection.git
cd project-name
```

2. **Create Virtual Environment (Recommended)**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install Dependencies**
```bash
pip install -r requirement.txt
```

4. **Run the Application**
```bash
python app.py
```

## 💻 Usage

1. **Start the Server**
   - Run `python app.py`
   - Access the application at `http://localhost:5000`

2. **Upload Image**
   - Click the upload button
   - Select an image file (supported formats: JPG, PNG)

3. **View Results**
   - The analysis will be displayed automatically
   - Results show authenticity percentage and classification

## 🔌 API Reference

### Image Analysis Endpoint
```
POST /predict
Content-Type: multipart/form-data

Parameters:
- file: File (required)

Response:
{
    "fake_probability": float,   // percentage, 0-100
    "real_probability": float    // percentage, 0-100
}
```

## 👥 Creators
- [Ananya419](https://github.com/Ananya419)
- [shri-ram07](https://github.com/shri-ram07)

## 📧 Contact
For support or inquiries:
- Email: raunakd511@gmail.com

## 📄 License
This project is licensed under the MIT License.

## 🔧 Requirements
```
flask>=2.0.0
tensorflow>=2.0.0
numpy>=1.19.0
pillow>=8.0.0
```

## ⚠️ Important Notes
- Ensure you have sufficient RAM for model loading
- GPU support is recommended for faster processing
- Keep the model file in the `saved_model` directory
- Maintain proper file permissions for uploads

---

<p align="center">
  Made with ❤️ by Team DeepFake Detective
</p>

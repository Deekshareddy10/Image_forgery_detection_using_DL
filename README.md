# Image Forgery Detection Using Deep Learning

Built as part of a Deep Learning course project.

## Overview

This project focuses on detecting image forgery using deep learning techniques. The application allows users to upload images and predicts whether the image has been manipulated or forged.

The model is integrated into a Flask web application for easy interaction and testing.

---

## Features

- Deep learning based image forgery detection
- Flask web application interface
- Image upload and prediction support
- Pretrained model integration
- Local deployment support

---

## Tech Stack

- Python
- TensorFlow / Keras
- Flask
- HTML/CSS
- Git LFS

---

## Local Setup and Installation

Follow the steps below to run the project locally.

### 1. Prerequisites

Make sure the following are installed on your system:

- Python 3.10 or higher
- Git
- Git LFS

---

### 2. Clone the Repository

```bash
git clone https://github.com/Shubham-711/image-forgery-detector.git
cd image-forgery-detector
```

---

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

---

### 4. Activate the Virtual Environment

#### Windows

```bash
.\venv\Scripts\activate
```

#### macOS/Linux

```bash
source venv/bin/activate
```

---

### 5. Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 6. Download the Model Files

The trained model is tracked using Git LFS.

```bash
git lfs pull
```

---

### 7. Configure the Secret Key

Open `app.py` and replace the placeholder `app.secret_key` with a securely generated secret key.

Generate one using:

```python
import secrets
secrets.token_hex(24)
```

---

### 8. Run the Application

```bash
flask run
```

The application will run at:

```text
http://127.0.0.1:5000
```

---

## Project Structure

```text
image-forgery-detector/
│
├── app.py
├── requirements.txt
├── templates/
├── static/
├── models/
├── uploads/
└── README.md
```

---

## Notes

- Ensure Git LFS is installed before pulling model files
- Large datasets and model weights are not included directly in the repository
- Recommended to use a virtual environment for dependency management

---

## Future Improvements

- Improve model accuracy using advanced architectures
- Add support for multiple forgery detection techniques
- Deploy application using cloud platforms
- Add user authentication and image history tracking

---

## License

This project was developed for academic and educational purposes.

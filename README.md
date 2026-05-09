# Image_forgery_detection_using_DL
Built as a part of deep learning course 

## Local Setup & Installation ⚙️
Follow these steps to run the project on your local machine.

1. Prerequisites:

Python 3.10 or higher
Git and Git LFS (for handling the large model file)
2. Clone the Repository:

git clone (https://github.com/Shubham-711/image-forgery-detector.git)
cd image-forgery-detector
3. Set up the Virtual Environment:

# Create a virtual environment
python -m venv venv

# Activate it
# Windows
.\venv\Scripts\activate
# macOS/Linux
source venv/bin/activate
4. Install Dependencies:

pip install -r requirements.txt
5. Download the Model File: The Keras model is tracked by Git LFS. Run the following command to download it.

git lfs pull
6. Configure the Secret Key: Open app.py and replace the placeholder app.secret_key with a real, securely generated key. You can generate one in a Python terminal:

import secrets
secrets.token_hex(24)
7. Run the Application:

flask run
The application will be available at http://127.0.0.1:5000.

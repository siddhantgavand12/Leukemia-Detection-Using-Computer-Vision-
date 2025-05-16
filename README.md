# 🧬 Leukemia Detection Web App

This project is a web-based platform that leverages **deep learning models** to automatically detect leukemia from blood smear images. It provides an intuitive frontend for users (patients, doctors, researchers) to upload an image and receive real-time predictions powered by pre-trained image classification models.

---

## 🚀 Features

- 🧠 Leukemia detection using deep learning (CNN models)
- 📊 Multiple pre-trained models integrated:
  - MobileNetV2
  - EfficientNetB0
  - NasNetMobile
- 📁 Simple file upload system for predictions
- 💻 Flask-based backend API
- 📉 Model prediction confidence and class output
- 🔒 Basic login logic (in progress)

---

## 📂 Project Structure
├── app.py # Flask backend entry point
├── templates/ # HTML templates for Flask
├── static/ # Static files (CSS, JS, Images)
├── uploads/ # Uploaded images directory
├── models/ # Saved model files (.h5, .bin, .json)
├── requirements.txt # Python dependencies
├── README.md # You're reading this :)


---

## 🛠️ Installation

### 1. Clone the repo

```bash
git clone https://github.com/your-username/leukemia-detection.git
cd leukemia-detection
```

### 2. Create virtual environment (optional but recommended)

bash
Copy
Edit
python -m venv venv
source venv/bin/activate        # Linux/Mac
venv\Scripts\activate           # Windows

### 3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt

### 4. Run the Flask app
bash
Copy
Edit
python app.py


🧪 Models Used
All models are trained using transfer learning on blood smear image datasets (e.g., ALL-IDB).
| Model          | Framework | Accuracy | Size   |
| -------------- | --------- | -------- | ------ |
| MobileNetV2    | Keras     | \~90%    | Small  |
| EfficientNetB0 | Keras     | \~93%    | Medium |
| NasNetMobile   | Keras     | \~91%    | Large  |

Models are stored in .h5, .bin, or TensorFlow Lite format in the models/ directory.

📸 How It Works
User uploads a blood smear image.

The backend preprocesses the image.

The image is passed through the selected deep learning model.

The model returns a prediction (e.g., Leukemia Detected or Healthy) with a confidence score.

The result is displayed on the frontend interface.

✅ Todo (Upcoming Features)
 Add login/signup functionality

 Display precautionary tips based on result

 Responsive UI improvements

 Option to choose different models

 Visualization of intermediate CNN layers

📚 Dataset
ALL-IDB Dataset

Other open-access medical imaging datasets

🤝 Contributions
Contributions are welcome!
Feel free to fork the repo, raise issues, or submit pull requests.

👨‍💻 Authors
Siddhant Gavand 
Atharva Gangras
Deepak Choudhry

🚀 Face Recognition Based Attendance System

A smart attendance system powered by deep learning that uses facial recognition to automatically track and record the attendance of students or employees in real time using live video feeds.

Real-time attendance capture using face detection & machine learning
Built with Haar Cascade + KNN, featuring a sleek Flask web interface.

---

✨ Features

* 🎥 Real-time face detection using OpenCV (Haar Cascade)
* 🧠 Face recognition with ML-based K-Nearest Neighbors (KNN)
* 📝 Auto attendance marking with timestamps
* 🌐 Interactive web UI powered by Flask
* 💾 Stores attendance logs in `CSV` (easy to extend to DB)

---

🛠 Tech Stack

* **Python 3.x**
* **OpenCV** (Haar Cascade)
* **scikit-learn** (KNN)
* **Flask** (web backend)
* **HTML / CSS / Bootstrap** (web frontend)
* **Pandas / CSV** (data storage)

---

📂 Project Structure

```
.
├── app.py                 # Flask app
├── train_model.py         # KNN training script
├── haarcascade_frontalface_default.xml
├── knn_model.pkl          # Saved trained model
├── dataset/               # Face images per person
├── attendance.csv         # Attendance log
├── templates/
│   └── index.html         # Web UI
├── static/                # CSS/JS/images
├── requirements.txt
└── README.md
```

---

🚀 Quick Start

1️⃣ Clone the repo

```bash
git clone https://github.com/yourusername/face-recognition-attendance-system.git
cd face-recognition-attendance-system
```

2️⃣ Set up environment & install dependencies

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

---

3️⃣ Prepare dataset & train model

* Organize face images in `dataset/`:

  ```
  dataset/
  ├── John/
  │   ├── img1.jpg
  │   └── img2.jpg
  └── Jane/
      └── img1.jpg
  ```
* Train KNN model:

```bash
python train_model.py
```

---

4️⃣ Run the Flask app

```bash
python app.py
```

Open your browser: [http://localhost:5000](http://localhost:5000)

* Starts webcam, detects & recognizes faces in real-time.
* Logs attendance in `attendance.csv`.

---

🚀 Future Enhancements

* Use advanced models (FaceNet, Dlib, Mediapipe)
* Add secure admin dashboard & user authentication
* Export attendance reports (PDF / Excel)
* Integrate SQL / NoSQL database

---

🤝 Contributing

PRs are welcome! 🚀

1. Fork it
2. Create your feature branch (`git checkout -b feature`)
3. Commit & push (`git commit -m 'Add feature'`, `git push origin feature`)
4. Open a Pull Request

---

📄 License

This project is under the **MIT License**.
See [LICENSE](LICENSE).

---

🙌 Credits

* [OpenCV](https://opencv.org/) for detection
* [scikit-learn](https://scikit-learn.org/) for KNN
* [Flask](https://flask.palletsprojects.com/) for backend

---

⭐ **If you found this helpful, give it a star!**
Ready for your next feature? Ping me to write your `app.py`, `train_model.py`, or even set up deployment instructions. 🚀

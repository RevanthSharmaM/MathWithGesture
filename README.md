# 👋🧠 Math With Gesture

Math With Gesture is an interactive AI-powered application that allows users to **draw math expressions using hand gestures**. Leveraging real-time hand tracking and Google Gemini AI, the app interprets drawn equations and provides solutions—all through intuitive finger gestures.

---

## 🎯 Features

* 🕐️ **Hand Gesture Recognition** using MediaPipe (via `cvzone`)
* 🧠 **Math Expression Solving** using Gemini AI (Gemini 1.5 Flash)
* 🧹 **Draw with Your Index Finger** like a virtual pen
* 🧽 **Erase** using your thumb gesture
* 🖼️ **Live Stream Display** inside Streamlit UI
* 📷 **Real-time Webcam Feed Integration**

---

## 🚀 Demo

<p align="center">
  <img src="MathGestures.png" width="600" alt="App Screenshot">
</p>

---

## 🛠️ Tech Stack

* **Python 3.x**
* [Streamlit](https://streamlit.io/)
* [OpenCV](https://opencv.org/)
* [cvzone](https://github.com/cvzone/cvzone) – for easy hand tracking
* [Google Gemini AI (Generative AI SDK)](https://ai.google.dev/)
* **PIL** for image processing

---

## ✍️ How It Works

1. ✅ **Index finger up** – draw on the virtual canvas
2. 🗑️ **Thumb up** – clear the canvas
3. 🤖 **Middle-Ring-Little fingers up (gesture: `[0, 0, 1, 1, 1]`)** – send the drawing to Gemini AI for math solving
4. 📃 The answer will appear on the right panel in the Streamlit app

---

## ⚙️ Installation

1. **Clone the repository**

```bash
git clone https://github.com/RevanthSharmaM/MathWithGesture.git
cd MathWithGesture
```

2. **Create a virtual environment (optional but recommended)**

```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

> If `requirements.txt` isn't available, you can install manually:

```bash
pip install streamlit opencv-python cvzone numpy Pillow google-generativeai
```

4. **Run the app**

```bash
streamlit run main.py
```

---

## 🔑 API Key

This app uses **Google Gemini AI**.
To use it:

* Visit [https://ai.google.dev/](https://ai.google.dev/)
* Create an API key
* Replace the API key in the code:

```python
genai.configure(api_key="YOUR_API_KEY_HERE")
```

---

## 📌 Requirements

* Python 3.8+
* A working webcam
* Internet connection (for Gemini API)

---

## 🧠 Example Use Case

* Teachers and students can draw math equations in mid-air.
* AI interprets handwritten expressions.
* Quickly evaluate without typing or scanning equations.

---

## 🤝 Contributing

Pull requests are welcome!
Feel free to open issues for bugs, features, or suggestions.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

---

## 👨‍💻 Author

**Revanth Sharma M**
GitHub: [@RevanthSharmaM](https://github.com/RevanthSharmaM)

---

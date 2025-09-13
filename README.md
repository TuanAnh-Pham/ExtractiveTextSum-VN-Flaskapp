# Vietnamese Extractive Text Summarization – Flask App

A simple **Flask web application** that performs **extractive text summarization in Vietnamese**.  
Users can paste text into a web form, and the app generates a concise summary using a pretrained encoder model.

---

## ✨ Features
- **Vietnamese text summarization** using an extractive approach (sentence ranking).
- **Flask backend** with clean HTML templates for a lightweight web UI.
- **Model loading** from local `models/` folder (Word2Vec-style encoder).
- Ready for experimentation and integration into larger NLP projects.

---

## 📂 Project Structure
```
ExtractiveTextSum-VN-Flaskapp/
├── app.py              # Main Flask app
├── models/             # Place pretrained summarization model here
├── static/             # CSS, JS, and static assets
├── templates/          # HTML templates for the UI
├── README.md           # Documentation (this file)
└── requirements.txt    # Python dependencies
```

---

## ⚙️ Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/TuanAnh-Pham/ExtractiveTextSum-VN-Flaskapp.git
   cd ExtractiveTextSum-VN-Flaskapp
   ```

2. **Set up Python environment**
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## 📥 Model Setup

1. Download the pretrained encoder model (link provided by the author).  
2. Place the model file into the `models/` folder.  

Example:
```
ExtractiveTextSum-VN-Flaskapp/models/encoder.bin
```

---

## 🚀 Running the App
```bash
python app.py
```

- Open your browser at **http://127.0.0.1:5000/**
- Paste Vietnamese text into the input form.
- Click **Summarize** to get the extractive summary.

---

## 📊 Methodology
- The summarizer uses a **sentence-embedding + similarity ranking approach**.  
- Sentences are encoded with the pretrained model.  
- Top-ranked sentences are extracted and concatenated to form the final summary.  

---


## 📜 License
This project is open-sourced under the MIT License.  
Feel free to use and modify for research or personal projects.

---

## 🙌 Acknowledgements
- Trained based on referenced papers and datasets.  
- Flask, Python, and open-source NLP libraries that made this possible.

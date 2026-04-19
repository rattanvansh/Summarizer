# 📝 Text Summarizer using HuggingFace T5

An AI-powered web application that generates concise summaries from long text inputs using the T5 Transformer model. Built with FastAPI and an interactive frontend.

---

## 🚀 Features

- Abstractive text summarization using T5 model  
- FastAPI backend for real-time inference  
- Simple and responsive web interface  
- Text preprocessing (removes HTML tags, extra spaces, noise)  
- Supports CPU/GPU execution  

---

## 🧠 Tech Stack

- Backend: FastAPI, Python  
- AI/ML: HuggingFace Transformers (T5), PyTorch  
- Frontend: HTML, CSS, JavaScript  
- Templating: Jinja2  

---

## 📂 Project Structure

.
├── main.py  
├── requirements.txt  
├── templates/  
│   └── index.html  
├── static/  


---

## ⚙️ Installation & Setup

1. Clone the repository  
git clone https://github.com/your-username/text-summarizer.git  
cd text-summarizer  

2. Create virtual environment (optional)  
python -m venv venv  
venv\Scripts\activate  

3. Install dependencies  
pip install -r requirements.txt  

---

## ▶️ Run the Application

uvicorn main:app --reload  

Open in browser:  
http://127.0.0.1:8000  

---

## 🔗 API Endpoint

POST /summarize/  

Request:
{
  "dialogue": "Your long text here..."
}

Response:
{
  "summary": "Generated summary..."
}

---

## ⚠️ Notes

- If using local model: ensure `saved_summary_model/` exists  
- For deployment, you can use:
  T5ForConditionalGeneration.from_pretrained("t5-small")

---

## 🌐 Deployment

Recommended platforms:
- Render  
- Hugging Face Spaces  

---

## 📌 Future Improvements

- Add file upload (PDF/Text)  
- Improve UI/UX  
- Add multiple models (BART, PEGASUS)  
- Optimize inference speed  

---

## 📜 License

This project is for educational purposes.

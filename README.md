# 🌐 AI Web Scraper (Streamlit + LLM)

An intelligent **AI-powered web scraper** built using **Python, Streamlit, Selenium, and Ollama (LLaMA 3)** that allows users to:

* Scrape any website 🌍
* Clean and process DOM content 🧹
* Extract specific information using AI 🤖

---

## 🚀 Features

### 🔍 Web Scraping

* Scrapes full webpage using **Selenium**
* Handles dynamic content and CAPTCHA
* Extracts only `<body>` content for processing

### 🧹 Data Cleaning

* Removes:

  * `<script>` tags
  * `<style>` tags
* Outputs clean, readable text

### 🤖 AI Parsing (LLM Powered)

* Uses **Ollama (LLaMA 3)** via LangChain
* Extracts **only the data you ask for**
* No extra explanations or noise

### 🖥️ Interactive UI

* Built with **Streamlit**
* View scraped DOM content
* Input custom parsing instructions

---

## 🧠 How It Works

1. User enters a website URL
2. Selenium scrapes the page
3. HTML is cleaned and converted to text
4. Content is split into chunks
5. LLM processes chunks based on user query
6. Extracted data is displayed

---

## 🗂️ Project Structure

```id="h3k92p"
├── Main.py
├── Scrape.py
├── Parse.py
├── Requirements.txt
├── chromedriver.exe
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash id="r7m4bz"
git clone <your-repo-url>
cd <repo-folder>
```

---

### 2️⃣ Create Virtual Environment

```bash id="p9x2lm"
python -m venv ai
```

---

### 3️⃣ Activate Virtual Environment

#### Windows:

```bash id="c2q8yt"
ai\Scripts\activate
```

#### macOS/Linux:

```bash id="k5v9sd"
source ai/bin/activate
```

---

### 4️⃣ Install Dependencies

```bash id="u1z8eo"
pip install -r requirements.txt
```

---

### 5️⃣ Install & Run Ollama

```bash id="g6n3va"
ollama run llama3
```

---

## ▶️ Running the App

```bash id="y4t7wk"
streamlit run Main.py
```

---

## 🧪 Usage

1. Enter a website URL
2. Click **"Scrape Site"**
3. View cleaned DOM content
4. Describe what you want (e.g., *"Extract emails"*)
5. Click **"Parse Content"**
6. Get AI-extracted results 🎯

---

## 🧰 Tech Stack

* Streamlit
* Selenium
* BeautifulSoup
* LangChain
* Ollama (LLaMA 3)
* Python

---

## ⚠️ Requirements

* Python 3.8+
* Google Chrome
* `chromedriver.exe` (matching your Chrome version)
* Ollama installed

---

## ⚠️ Notes

* Always activate the virtual environment before running the app
* Large websites may take longer due to AI processing
* CAPTCHA solving depends on external service

---

## 🔮 Future Improvements

* Export results (CSV / JSON)
* Multi-model support (GPT, Claude)
* Better UI design
* Faster processing with parallel chunks

---

## 👨‍💻 Author

AI + Automation Project combining **Web Scraping + LLMs**

---

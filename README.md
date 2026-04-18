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

```id="3k2l9f"
├── Main.py            # Streamlit UI
├── Scrape.py          # Web scraping + cleaning
├── Parse.py           # AI parsing using Ollama
├── Requirements.txt   # Dependencies
├── chromedriver.exe   # Chrome driver (required)
```

---

## ⚙️ Installation

### 1️⃣ Clone the Repository

```bash id="l0k1mz"
git clone <your-repo-url>
cd <repo-folder>
```

### 2️⃣ Install Dependencies

```bash id="d9xw21"
pip install -r requirements.txt
```

### 3️⃣ Install Ollama

Make sure you have Ollama installed and running:

```bash id="y7m2qp"
ollama run llama3
```

---

## ▶️ Running the App

```bash id="w8v3an"
streamlit run Main.py
```

---

## 🧪 Usage

1. Enter a website URL
2. Click **"Scrape Site"**
3. View cleaned DOM content
4. Describe what you want (e.g., *"Extract all product names"*)
5. Click **"Parse Content"**
6. Get AI-extracted results 🎯

---

## 🧰 Tech Stack

* **Frontend/UI:** Streamlit
* **Web Scraping:** Selenium
* **Parsing:** BeautifulSoup
* **LLM Integration:** LangChain + Ollama (LLaMA 3)
* **Language:** Python

---

## ⚠️ Requirements

* Python 3.8+
* Chrome Browser
* Compatible `chromedriver.exe`
* Ollama installed and running

---

## ⚠️ Limitations

* Requires local Ollama setup
* CAPTCHA solving depends on external service
* Large pages may take longer due to chunking

---

## 🔮 Future Improvements

* Add support for multiple LLMs (GPT, Claude, etc.)
* Export results (CSV / JSON)
* Add scraping history
* Improve UI/UX
* Parallel chunk processing for speed

---

## 👨‍💻 Author

Built as an **AI + Web Scraping project** combining automation and LLM capabilities.

---

# 🕷️ AI Powered WebScrapper

An interactive **Streamlit application** that scrapes any webpage, indexes its content, and lets you **ask questions about it in natural language**.  
Powered by [LangChain](https://www.langchain.com/), [Ollama](https://ollama.ai/), and [Selenium](https://www.selenium.dev/), this tool extracts information, chunks it intelligently, embeds it, and lets you query it like your own mini search engine.

---

## 🚀 Features
- 🌐 **Scrape webpages** using Selenium.  
- 📑 **Chunk and embed** content with LangChain’s text splitter + Ollama embeddings.  
- 🤖 **Ask questions** in natural language about any scraped webpage.  
- ⚡ **Local vector store** for similarity search.  
- 🖥️ **Interactive Streamlit interface** with chat-style Q&A.  

---

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/webscrapper.git
   cd webscrapper
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Install Ollama**  
   Follow the instructions at [Ollama Download Page](https://ollama.ai/download) and make sure you have the `llama3.2` model installed:
   ```bash 
   ollama pull llama3.2
   ```

   *💡 Tip for Windows:* By default, Ollama will be installed on your **C:** drive. If you want to install it elsewhere, open a terminal near the Ollama installer and run:
   ```bash
   .\OllamaSetup.exe /DIR=D:\Your\Desired\Location
   ```

---

## ▶️ Usage

1. **Run the app**
   ```bash
   streamlit run app.py
   ```

2. **Open your browser** at  
   👉 [http://localhost:8501](http://localhost:8501)

3. **Enter a URL** in the input box.  
   Example:
   ```
   https://en.wikipedia.org/wiki/Artificial_intelligence
   ```

4. **Ask questions** in the chat box.  
   Example:
   ```
   What is artificial intelligence?
   ```

---

## 🛠️ Project Structure
```
webscrapper/
│── app.py              # Main Streamlit app
│── requirements.txt    # Python dependencies
│── README.md           # Project documentation
```

---

## ⚙️ Requirements
- Python 3.9+  
- [Ollama](https://ollama.ai/) installed locally  
- Chrome / Chromium (required for Selenium)  

---

## 📌 Roadmap
- [ ] Add support for multiple URLs at once  
- [ ] Store embeddings in a persistent database (e.g., FAISS, Pinecone)  
- [ ] Export answers and context to Markdown / PDF  
- [ ] Add authentication for private deployments  

---

## 🐞 Issues & Contributions
- Found a bug? [Open an issue](https://github.com/danielgavrila2).  
- Want to improve it? Feel free to submit a pull request.  

---

## 📜 License
MIT License – Free to use, modify, and distribute.  

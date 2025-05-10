

# 🧠 Enhanced Q\&A Chatbot with Ollama

This is a simple but powerful Streamlit web app that lets users interact with open-source large language models (LLMs) like **Gemma 2** and **LLaMA 3** using a conversational interface.

Built with `LangChain`, `Ollama`, and `Streamlit`, the app enables users to ask natural language questions and receive intelligent responses.

## 🚀 Features

* Switch between **Gemma 2** and **LLaMA 3** models
* Adjustable **temperature** and **max tokens** for output tuning
* Clean, interactive UI using **Streamlit**
* Uses **LangChain** prompt templates and response parsing
* Supports **LangSmith** for experiment tracking

---

## 🛠️ Technologies & Libraries Used

* [Streamlit](https://streamlit.io/) - for building the web interface
* [Ollama](https://ollama.com/) - to run open-source LLMs locally
* [LangChain](https://www.langchain.com/) - to manage prompts and LLM chains

  * `langchain_core`
  * `langchain_openai`
  * `langchain_community`
* [OpenAI SDK](https://github.com/openai/openai-python) - general integration
* `dotenv` - to manage environment variables securely

---

## ⚙️ Setup Instructions

1. **Clone the repo**

   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. **Create and activate a virtual environment (optional but recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows: venv\Scripts\activate
   ```

3. **Install the required libraries**

   ```bash
   pip install -r requirements.txt
   ```

4. **Create a `.env` file** and add your LangSmith API key:

   ```
   LANGCHAIN_API_KEY=your_langsmith_api_key
   ```

5. **Run the Streamlit app**

   ```bash
   streamlit run appwithollama.py
   ```

---

## 🧪 How It Works

* The user types a question into the input box.
* The selected LLM (via Ollama) is initialized with LangChain.
* The prompt is wrapped using `ChatPromptTemplate`.
* Output is parsed with `StrOutputParser`.
* The response is rendered on the Streamlit interface.

---

## 📌 Note

* Ensure you have [Ollama installed](https://ollama.com/download) and models like `gemma2` or `llama3` available locally.
* This app assumes a local model running environment and may require downloading models via the Ollama CLI beforehand.

---



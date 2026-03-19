# 🚀 AI Sales & Compliance Intelligence Agent

This repository features an advanced AI agent designed to streamline sales engineering and legal compliance. By leveraging **Hierarchical Auto-merging Retrieval (RAG)**, the system analyzes complex legal contracts and technical manuals to provide high-fidelity, context-aware insights.

## 🧠 Core Technical Features

* **Hierarchical Auto-merging Retrieval:** Optimized context window management that automatically merges smaller leaf nodes into parent chunks for superior semantic accuracy.
* **Intelligent Multi-Engine Routing:** A dynamic router that autonomously selects the appropriate knowledge base—whether technical documentation, customer email history, or legal TOS—based on the user's intent.
* **RAGAS Evaluation Framework:** Integrated quality assurance that measures **Faithfulness** (hallucination mitigation) and **Answer Relevancy** in real-time using NLP metrics.
* **Streamlit UI:** A clean, production-ready interface for interactive querying, system status monitoring, and metric visualization.

---

## 🛠️ Installation & Setup

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
cd your-repo-name

### 🛠️ Install Dependencies
    Ensure you have Python 3.9+ installed, then run:
    pip install -r requirements.txt

### 3. Environment Configuration
    Create a .env file in the root directory and add your Google API credentials:
    GOOGLE_API_KEY=your_gemini_api_key_here

🚀 Execution
    You can try the AI Sales & Compliance Intelligence Agent live here:
    👉 [Live Demo - Try the App here!]()

📊 Project Architecture

    main.py: The primary entry point. Manages the Streamlit state, UI components, and the orchestration of the RAG engine.

    src/engine.py: The core logic for index construction, hierarchical node parsing, and the multi-tool routing agent.

    src/evaluator.py: Implementation of the RAGAS framework for automated response auditing and performance metrics.

📁 Suggested Data Structure (Demo Mode):

To test the system immediately, organize your local files as follows:

    /
    ├── main.py
    ├── requirements.txt
    ├── .env
    ├── src/
    │   ├── engine.py
    │   ├── evaluator.py
    │   └── LOGO.png
    └── data/
        ├── technical/   <-- Place technical PDFs here
        ├── contracts/   <-- Place legal/TOS PDFs here
        └── emails/
            └── emails.csv <-- Place customer interaction history here
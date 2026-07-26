# 🌍 TourismGPT: Industry-Specific Large Language Model Using Phi-3 Mini, QLoRA & RAG

## 📖 Overview

TourismGPT is an industry-specific conversational AI assistant developed for the **Tourism and Hospitality** sector. The project demonstrates how a pre-trained Large Language Model (LLM) can be adapted to a specific domain using **Parameter-Efficient Fine-Tuning (QLoRA)** and enhanced with **Retrieval-Augmented Generation (RAG)**.

Instead of relying solely on the model's internal knowledge, TourismGPT retrieves relevant tourism information from a FAISS vector database built from Wikivoyage content before generating responses. This significantly improves contextual accuracy while reducing hallucinations.

This project was developed as part of the **IndustryGPT: Specialized LLM Bot Using Pre-Trained Models** capstone project.

---

# 🎯 Project Objectives

* Build an industry-specific conversational AI assistant.
* Fine-tune Microsoft's Phi-3 Mini model using tourism-specific instruction-response data.
* Improve factual accuracy using Retrieval-Augmented Generation (RAG).
* Deploy an interactive chatbot using Gradio.
* Demonstrate the practical application of domain-specific Large Language Models.

---

# 🏗️ Project Architecture

```text
                User Query
                     │
                     ▼
            Gradio User Interface
                     │
                     ▼
          Sentence Transformer
             (Query Embedding)
                     │
                     ▼
              FAISS Vector Search
                     │
       Top Relevant Tourism Chunks
                     │
                     ▼
     Fine-Tuned Microsoft Phi-3 Mini
             (QLoRA Adapter)
                     │
                     ▼
            TourismGPT Response
```

---

# 🚀 Features

* Industry-specific Tourism chatbot
* Microsoft Phi-3 Mini language model
* QLoRA-based parameter-efficient fine-tuning
* Retrieval-Augmented Generation (RAG)
* FAISS vector database
* Semantic search using Sentence Transformers
* Interactive Gradio web interface
* Tourism-focused question answering

---

# 🛠️ Tech Stack

### Programming Language

* Python

### Large Language Model

* Microsoft Phi-3 Mini

### Fine-Tuning

* Hugging Face Transformers
* PEFT (QLoRA)
* TRL
* Unsloth

### Retrieval

* FAISS
* Sentence Transformers

### Deployment

* Gradio

### Development Environment

* Google Colab (T4 GPU)

---

# 📂 Dataset

The training dataset contains tourism-specific instruction-response pairs collected from publicly available tourism resources.

### Data Sources

* Wikivoyage
* Tourism FAQs
* Public travel information
* Destination descriptions
* Tourism-related articles

The dataset was cleaned, organized, and converted into instruction-response format before fine-tuning.

---

# 🔄 Project Workflow

1. Collect tourism-related data.
2. Clean and preprocess the dataset.
3. Convert data into instruction-response format.
4. Fine-tune Microsoft Phi-3 Mini using QLoRA.
5. Build a FAISS vector database.
6. Generate semantic embeddings using Sentence Transformers.
7. Implement Retrieval-Augmented Generation (RAG).
8. Deploy the chatbot using Gradio.
9. Evaluate responses using tourism-related queries.

---

TourismGPT/
│
├── notebooks/
│   ├── tourismgpt_pipeline.ipynb
│   ├── finetune_phi3.ipynb
│   ├── rag_pipeline.ipynb
│   ├── tourismgpt_ui.ipynb
│   └── TourismGPT_ML_Classification.ipynb
│
├── datasets/
│   └── tourism_finetune.jsonl
│
├── scripts/
│   ├── pipeline.py
│   └── generate_ai_pairs.py
│
├── screenshots/
├── README.md

> **Note:** The original Wikivoyage XML dump used to build the knowledge base is not included in this GitHub repository because of its large size. The processed training dataset and the scripts required to recreate the knowledge base are provided.

> **Note:** The fine-tuned LoRA adapter is available in the project submission package (Google Drive). It is not stored in this repository due to its size.
> 
GOOGLE DRIVE LINK : https://drive.google.com/drive/folders/1BsEIst98ry41Ra8TfYI7zbFpVkPBwM0D?usp=sharing
---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/Lenikaaa/IndustryGPT-Specialized-LLM-Bot-Using-Pre-Trained-Models
```

Navigate to the project folder:

```bash
cd TourismGPT
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

# ▶️ Running the Project

1. Open the notebooks in Google Colab or Jupyter Notebook.
2. Run the fine-tuning notebook to train the model (or use the saved adapter).
3. Execute the RAG pipeline notebook to create the FAISS index.
4. Launch the Gradio notebook to interact with TourismGPT.

---

# 💬 Sample Questions

Example questions you can ask the chatbot:

* Suggest a 5-day itinerary for Japan.
* What are the top attractions in Paris?
* Which season is best to visit Switzerland?
* Recommend family-friendly destinations in Europe.
* What should I pack for a trip to Iceland?
* How can I travel from Delhi to Manali?
* What are the must-visit places in Rajasthan?
* Suggest budget-friendly destinations in Southeast Asia.

---

# 📊 Results

TourismGPT successfully demonstrates:

* Domain-specific response generation
* Context-aware tourism recommendations
* Improved factual accuracy through RAG
* Reduced hallucinations using external knowledge retrieval
* Interactive conversational experience through Gradio

---

# ⚠️ Limitations

* Knowledge is limited to the available tourism dataset and indexed documents.
* Real-time travel information (weather, flight schedules, hotel availability) is not included.
* Responses may be less accurate for destinations outside the knowledge base.
* The chatbot does not currently integrate live travel APIs.

---

# 🔮 Future Improvements

* Integrate real-time travel APIs.
* Expand the tourism knowledge base.
* Support multilingual conversations.
* Deploy on Azure or Hugging Face Spaces.
* Implement hybrid retrieval techniques.
* Add user feedback for continuous improvement.

---

# 📚 Learning Outcomes

This project provided practical experience in:

* Large Language Models (LLMs)
* Transfer Learning
* Parameter-Efficient Fine-Tuning (QLoRA)
* Retrieval-Augmented Generation (RAG)
* Vector Databases (FAISS)
* Semantic Search
* Hugging Face Ecosystem
* Conversational AI Deployment using Gradio

---

# 🙏 Acknowledgements

* Microsoft Phi-3
* Hugging Face
* Unsloth
* FAISS
* Sentence Transformers
* Gradio
* Wikivoyage
* Google Colab

---

# 📜 License

This project is intended for educational and research purposes as part of the IndustryGPT capstone project.

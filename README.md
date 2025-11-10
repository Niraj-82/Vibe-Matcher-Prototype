# 🎧 Vibe Matcher – AI-Powered Fashion Discovery

### 🚀 Developed by: *Niraj Ravindra Sawant*

---

## 🧠 Overview

**Vibe Matcher** is an AI-powered recommendation prototype developed as part of the **Nexora Internship Task**.  
It demonstrates how **semantic embeddings** and **vector similarity search** can be used to match a user’s *“vibe”* (mood, emotion, or style) to suitable product descriptions, outfits, or aesthetic categories.

Unlike traditional keyword-based recommendation systems, **Vibe Matcher** understands the *context and emotion* behind the input — delivering results that truly “match the mood.”

---

## 🎯 Objective

To build a **vibe-based semantic matching system** that:
- Understands user intent beyond keywords.
- Maps product descriptions into vector space using **text embeddings**.
- Finds semantically similar items using **cosine similarity**.
- Evaluates model efficiency through **accuracy, latency, and good match rate**.

---

## 🧩 Tech Stack

| Component | Technology Used |
|------------|-----------------|
| Language | Python |
| Environment | Google Colab / Jupyter Notebook |
| Libraries | `pandas`, `numpy`, `sklearn`, `matplotlib`, `openai` |
| Model | `text-embedding-ada-002` |
| Matching Metric | Cosine Similarity |
| Visualization | Matplotlib |
| Optional Future Tools | FAISS / Pinecone for scalable vector search |

---

## ⚙️ How It Works

1. **Dataset Preparation**  
   A small dataset (`desc` column) containing sample product or vibe descriptions is loaded into a DataFrame.

2. **Embedding Generation**  
   Each text description is converted into a numerical vector using OpenAI’s `text-embedding-ada-002` model.

3. **Similarity Matching**  
   The system computes cosine similarity between the user’s query embedding and all item embeddings.

4. **Top-N Recommendation**  
   The three most similar descriptions are displayed along with similarity scores.

5. **Evaluation Metrics**  
   - **Average Similarity Score**
   - **Good Match Rate** (% of queries scoring > 0.7)
   - **Mean Latency per Query**

---

## 🧪 How to Run

1. **Clone this repository:**
   ```bash
   git clone https://github.com/Niraj-82/Vibe-Matcher-Prototype.git
   cd Vibe-Matcher-Prototype

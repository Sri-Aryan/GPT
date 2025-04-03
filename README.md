# **Bigram Language Model – GPT Implementation** 🚀  

A **Transformer-based Bigram Language Model** built using **PyTorch**. This project implements **self-attention mechanisms** and **embedding layers** for text generation. The model is trained on **Shakespeare's dataset** and generates text using a **causal transformer** approach.  

---

## 📌 **Features**  
✅ **Character-Level Text Generation** using a **bigram-based** self-attention model.  
✅ **Positional Encoding** for better contextual understanding.  
✅ **Masked Attention** to prevent information leakage during training.  
✅ **Trained on Shakespeare’s dataset**, enabling natural text generation.  
✅ **Optimization using AdamW** for efficient training.  

---

## 🛠️ **Tech Stack**  
- **Framework**: PyTorch  
- **Training Data**: Tiny Shakespeare dataset  
- **Model Architecture**: Transformer-based bigram model  
- **Optimization Algorithm**: AdamW  
- **Hardware**: CUDA-enabled GPU (if available)  

---

## 🚀 **How It Works**  

### **1️⃣ Data Preprocessing**  
- Download **Tiny Shakespeare Dataset**.  
- Encode characters into numerical tokens for processing.  
- Create a **lookup table** (stoi & itos) for character mapping.  

### **2️⃣ Model Architecture**  
- **Embedding Layers**: Convert input tokens into dense representations.  
- **Positional Encoding**: Adds positional context to embeddings.  
- **Masked Self-Attention**: Prevents future token access during training.  
- **Feedforward Network**: Processes token embeddings to generate logits.  

### **3️⃣ Training Process**  
- Splits dataset into **train & validation** sets.  
- Uses **Cross Entropy Loss** for optimization.  
- Trained for **10,000 steps** using **AdamW optimizer**.  

### **4️⃣ Text Generation**  
- Starts with a random seed token.  
- Uses **Softmax sampling** to predict next characters.  
- Generates text by iteratively predicting the next token.  

---

## 🔄 **Model Training Flow**  
1️⃣ **Data Encoding** – Convert text into token sequences.  
2️⃣ **Batch Generation** – Extract batches for training.  
3️⃣ **Embedding & Attention Mechanism** – Generate meaningful representations.  
4️⃣ **Training Loop** – Backpropagation and weight updates.  
5️⃣ **Text Generation** – Predict the next token using trained weights.  

---

## 📈 **Performance & Results**  
- Generates **realistic Shakespearean-style text** after training.  
- Uses **self-attention** for context-aware text generation.  
- **Future Improvements**: Multi-head attention, larger datasets, hyperparameter tuning.  


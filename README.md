# 🧠 Hate Speech Classifier – NLP Project using DistilRoBERTa

This project presents a high-accuracy Natural Language Processing (NLP) system for classifying hate speech using transformer models. Built with PyTorch and fine-tuned on a large-scale social media dataset, this model enables real-time prediction via an interactive Streamlit web interface.

## 🚀 Highlights

- 🏗 **Model**: Fine-tuned **DistilRoBERTa** using PyTorch.
- 📊 **Accuracy**: Achieved **87.4% test accuracy** on a balanced dataset of over **700,000 labeled samples**.
- 🔬 **Benchmarking**: Compared and analyzed 5+ transformer models including **RoBERTa**, **DistilBERT**, and **BERT-base**, evaluating overfitting, training time, and accuracy trade-offs.
- 🌐 **Deployment**: Developed an intuitive **Streamlit web interface** for live text classification of user input as either **"Hateful"** or **"Non-Hateful"**.

## 🛠 Tech Stack

- **Language**: Python
- **Libraries**: PyTorch, Transformers (HuggingFace), Streamlit
- **Model**: DistilRoBERTa (fine-tuned)
- **Frontend**: Streamlit (deployed as an interactive UI)
- **Dataset**: >700k social media posts, pre-balanced for binary classification

## 🖥 Project Structure

hate_speech_AI/
├── app/
│ ├── Hate_Speech_UI.py # Streamlit frontend script
│ ├── tokenizer.json # Tokenizer settings
│ ├── vocab.json # Vocabulary data
│ ├── merges.txt # Merge operations (for BPE)
│ ├── tokenizer_config.json # Tokenizer config
│ ├── special_tokens_map.json # Token mapping
│ └── model.safetensors # 🚫 Excluded from Git (see below)
├── .gitignore
└── README.md #


## ▶️ How to Run the Application

### 1. Clone the Repository
git clone https://github.com/MShaswat03/50.021-Artificial-Intelligence_Hate_Speech_Classifier-.git
cd hate_speech_AI

2. Install Dependencies
pip install -r requirements.txt

3. Place Model Weights
Download model.safetensors from the provided external link (e.g., Hugging Face or Google Drive), and place it inside the app/ directory.

4. Launch the Streamlit App
streamlit run app/Hate_Speech_UI.py

⚠️ Notes
app/model.safetensors is excluded from Git due to GitHub’s 100MB file size limit.

You can share large models using Git LFS, Hugging Face Hub, or Google Drive.

👤 Author
Manishansh Shaswat
📫 GitHub: @MShaswat03


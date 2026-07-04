# Chat-Based Music Recommendation System using Natural Language Inference (NLI)

## Overview:

This project presents a Chat-Based Music Recommendation System developed for the ACM RecSys Challenge 2026.

The system recommends music by understanding the user's conversation, emotional state, listening preferences, and recommendation goal. It combines traditional information retrieval with deep learning models to improve recommendation quality.

---

## Features:

- Multi-turn conversation understanding
- BM25 lexical retrieval
- Semantic retrieval using BGE embeddings
- Reciprocal Rank Fusion (RRF)
- Cross-Encoder re-ranking
- Natural Language Inference (NLI) based ranking
- Emotion-aware recommendations
- Large Language Model (LLM) generated conversational responses
- Cold-start user handling

---

## System Architecture

The recommendation pipeline follows these stages:

1. User conversation processing
2. Emotion detection
3. Query construction
4. BM25 retrieval
5. Semantic retrieval using sentence embeddings
6. Reciprocal Rank Fusion (RRF)
7. Cross-Encoder re-ranking
8. Natural Language Inference (NLI) ranking
9. Final Top-20 track recommendation
10. LLM-generated natural language response

---

## Models Used

Component| Model
Semantic Embeddings| BAAI/bge-small-en-v1.5
Cross Encoder| cross-encoder/ms-marco-MiniLM-L-6-v2
NLI Model| Fine-tuned DeBERTa
Response Generation| Llama 3.1 8B Instant (Groq API)

---

## Dataset

This project uses the datasets provided for the ACM RecSys Challenge 2026, including:

- Blind-A Dataset
- Blind-B Dataset
- Track Metadata Dataset

---

## Technologies

- Python
- Google Colab
- PyTorch
- Hugging Face Transformers
- Sentence Transformers
- Rank BM25
- Groq API
- NumPy
- Scikit-learn

---

## Recommendation Pipeline

Conversation
↓
Emotion Detection
↓
BM25 Retrieval+ Semantic Retrieval
↓
Reciprocal Rank Fusion (RRF)
↓
Cross-Encoder Re-ranking
↓
Natural Language Inference (NLI)
↓
Top-20 Music Recommendations
↓
LLM Response Generation

---

## Repository Contents

- "blindb_predictions.ipynb" — Main notebook
- "README.md" — Project documentation
- "LICENSE" — MIT License

---

## Author

Dilli Priya Athipatla

B.Tech Student

Research Internship Project

Developed under the guidance of Prof.Alapan Kuila

ACM RecSys Challenge 2026

---

## License

This project is released under the MIT License.

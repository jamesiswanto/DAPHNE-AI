# DAPHNE AI - Document-Based Conversational AI System

DAPHNE AI is an intelligent, document-based question-answering system designed to generate relevant and context-aware responses. By integrating machine learning techniques and state-of-the-art neural network models, DAPHNE AI can accurately interpret and answer user queries. This project leverages pretrained models for natural language understanding and combines text similarity methods to provide a hybrid approach to conversational AI.

---

## Table of Contents
1. [Project Overview](#project-overview)
3. [Tech Stack](#tech-stack)
4. [Setup Instructions](#setup-instructions)
7. [Model Details](#model-details)
8. [Contributing](#contributing)
9. [License](#license)

---

## Project Overview
DAPHNE AI is built to handle conversational AI tasks that rely on document-based question answering. It combines pretrained language models with traditional text similarity methods, allowing it to select or generate accurate responses based on user queries. This project was developed to demonstrate practical applications of natural language processing (NLP) in real-world scenarios, such as customer support, educational resources, and information retrieval systems.

## Tech Stack
- **Programming Language**: Python
- **Frameworks and Libraries**:
  - [Transformers (Hugging Face)](https://huggingface.co/transformers/) for pretrained model integration
  - [Sentence Transformers](https://www.sbert.net/) for semantic similarity
  - [Scikit-Learn](https://scikit-learn.org/) for TF-IDF vectorization
  - [Gradio](https://gradio.app/) for interactive UI
  - [PyTorch](https://pytorch.org/) for model computations
  - [Pandas](https://pandas.pydata.org/) for data manipulation

---

## Setup Instructions

### Prerequisites
- Python 3.7 or higher
- Git (for cloning the repository)
- GPU (optional, but recommended for faster processing)

### Installation
1. **Clone the Repository**
    ```bash
    git clone https://github.com/jamesiswanto/DAPHNE-AI.git
    cd DAPHNE-AI
    ```
2. **Download the Dataset**
   Ensure the dataset is stored in the correct location if using a custom dataset. The repository uses a CSV file stored at `Conversation.csv` in GitHub for demonstration purposes.

3. **Run the Application**
    ```bash
    python app.py
    ```
    
---

## Model Details

### TF-IDF Vectorizer
The TF-IDF Vectorizer is used to calculate text similarity between the input question and questions in the dataset. This serves as a preliminary filter to identify potentially relevant answers.

### Sentence Transformer
A pretrained model that generates sentence embeddings to enhance the semantic understanding of input text. It works alongside the TF-IDF vectorizer to ensure that DAPHNE AI captures both lexical and semantic relevance.

### DialoGPT (Fallback Model)
If no suitable response is found in the dataset, DAPHNE AI uses the DialoGPT model from Hugging Face to generate a coherent fallback response, ensuring continuous user engagement.

---

## Contributing
We welcome contributions from the community to enhance DAPHNE AI! If you would like to contribute, please follow these steps:

1. **Fork the repository**.
2. **Create a new branch**:
    ```bash
    git checkout -b feature/YourFeatureName
    ```
3. **Commit your changes**:
    ```bash
    git commit -m 'Add new feature'
    ```
4. **Push to the branch**:
    ```bash
    git push origin feature/YourFeatureName
    ```
5. **Open a Pull Request**.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contact
For any questions or feedback, please reach out to the project developer: **James Siswanto** via [LinkedIn](https://www.linkedin.com/in/jamesiswanto/) or [GitHub](https://github.com/jamesiswanto).

Question Answering System using BERT and RoBERTa

This project implements a Question Answering (QA) system using pre-trained transformer models, specifically BERT and RoBERTa, fine-tuned on the SQuAD 2.0 dataset. The system compares the performance of these models and includes an interactive user interface for testing custom questions.
Features

Fine-tuning BERT and RoBERTa on the SQuAD 2.0 dataset.
Evaluation of Exact Match (EM) and F1 Scores.
Comparison of model performance with visualizations (tables and graphs).
Interactive user interface using Gradio for custom QA testing.
Ability to test the models with custom contexts and questions.
Dataset

SQuAD 2.0: A dataset containing over 100,000 questions, including answerable and unanswerable questions.
Technologies Used

Python
Hugging Face Transformers
Datasets Library
Evaluate Library
Gradio
Matplotlib
Pandas
Installation

Step 1: Clone the Repository
git clone "repo link"
Step 2: Install Dependencies
pip install -r requirements.txt
Usage

1. Fine-tune Models
Fine-tune BERT or RoBERTa on the SQuAD 2.0 dataset:
python train.py
2. Evaluate Models
Run evaluation on the validation dataset to compare Exact Match (EM) and F1 Scores:
python evaluate.py
3. Launch Interactive UI
Start the Gradio interface to test custom questions:
python app.py
How to Use the Interactive UI

Enter a context (a paragraph of information).
Input a question related to the context.
Select a model (BERT or RoBERTa).
Click Submit to view the answer and confidence score.
Examples

Sample Input
Context:
"Python is a high-level programming language known for its simplicity and versatility. It supports object-oriented, procedural, and functional programming paradigms."
Question:
"What is Python known for?"
Selected Model:
RoBERTa
Sample Output
Answer: "simplicity and versatility"
Confidence: 0.98
Performance Comparison

Model	Exact Match (EM)	F1 Score
BERT	72.43%	75.74%
RoBERTa	79.87%	82.91%
Visualization

Bar chart comparing the Exact Match and F1 Scores of BERT and RoBERTa models:

Folder Structure

qa-system/
├── app.py                # Gradio interactive UI
├── train.py              # Model fine-tuning script
├── evaluate.py           # Evaluation and comparison script
├── requirements.txt      # Project dependencies
├── README.md             # Project documentation
├── datasets/             # SQuAD 2.0 dataset (auto-downloaded)
├── models/               # Saved fine-tuned models
└── results/              # Evaluation results and visualizations
Dependencies

Ensure the following Python libraries are installed:
transformers
datasets
evaluate
gradio
matplotlib
pandas
Install them with:
pip install transformers datasets evaluate gradio matplotlib pandas
Credits

Hugging Face Transformers and Datasets Library
SQuAD 2.0 Dataset
License

This project is licensed under the MIT License. See the LICENSE file for details.

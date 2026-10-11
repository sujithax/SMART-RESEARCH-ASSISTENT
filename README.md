# SMART-RESEARCH-ASSISTENT
An AI-powered Smart Research Assistant that uses FLAN-T5 and TinyLlama models to summarize research articles and answer questions based on their content. Built with Python, Pandas, PyTorch, and Hugging Face Transformers, this project simplifies research by making information easier to understand and retrieve.


### AI-Powered Article Summarization and Question Answering using LLMs

##  Project Overview

The **Smart Research Assistant** is a Generative AI project designed to help users understand lengthy technical articles quickly and efficiently. It uses Large Language Models (LLMs) to generate concise summaries and answer questions based on article content.

The project explores two transformer-based models, **FLAN-T5 Large** and **TinyLlama**, for text summarization and evaluates TinyLlama's ability to answer questions using the provided article as context.

The goal is to reduce information overload and make technical knowledge easier to access.

##  Objectives

- Summarize lengthy technical articles into concise, meaningful summaries.
- Generate answers to user questions based on article content.
- Explore and compare different transformer-based language models.
- Understand prompt engineering for summarization and question answering.
- Demonstrate how Generative AI can support research and information extraction.

##  Key Features

- **Text Summarization:** Converts long articles into shorter summaries.
- **Question Answering:** Generates answers using the supplied article as context.
- **Multiple LLMs:** Experiments with FLAN-T5 Large and TinyLlama.
- **Prompt Engineering:** Uses task-specific prompts to guide model responses.
- **Article Dataset Processing:** Loads and analyzes article data using Pandas.
- **Transformer-Based NLP:** Uses pretrained language models from Hugging Face.

##  Technologies Used

- Python
- Pandas
- PyTorch
- Hugging Face Transformers
- FLAN-T5 Large
- TinyLlama 1.1B Chat
- Google Colab / Jupyter Notebook
- Streamlit (planned application interface)

##  Models Used

### 1. FLAN-T5 Large

FLAN-T5 Large is an encoder-decoder transformer model used for text-to-text tasks.

In this project, it is used to generate summaries of technical articles. The notebook also explores its limitations when processing longer inputs.

### 2. TinyLlama 1.1B Chat

TinyLlama is a lightweight, decoder-only language model.

In this project, it is used for:
- Generating concise article summaries.
- Answering questions using article content as context.
- Exploring prompt-based text generation.

##  Project Workflow

1. **Import Libraries:** Load the required Python libraries, including Pandas, PyTorch, and Transformers.
2. **Load the Dataset:** Read the CSV file containing article titles and article text.
3. **Explore the Data:** Examine the dataset structure and its contents.
4. **Load Pretrained Models:** Initialize FLAN-T5 Large and TinyLlama with their tokenizers.
5. **Summarize Articles:** Generate summaries using model-specific prompts and generation parameters.
6. **Ask Questions:** Provide an article and a question to TinyLlama to generate a context-based answer.
7. **Analyze Outputs:** Examine the generated summaries and answers to understand the models' performance.

##  Dataset Description

The project uses a CSV dataset named `Articles.csv` containing two columns:

| Column | Description |
|---|---|
| `Title` | Headline describing the article's main topic |
| `Article` | Full text containing detailed information |

The notebook accesses this dataset through Google Drive. You must configure the file path for your own environment.

##  Example Use Cases

- Summarizing lengthy technology articles.
- Understanding emerging AI and NLP trends.
- Extracting important information from research content.
- Answering specific questions about a given article.
- Reducing the time required to review technical information.

##  Limitations

- Long articles may be truncated because of model input token limits.
- Generated summaries may omit important details.
- Answers may contain inaccurate information or details not supported by the article.
- Model performance depends on the input text and generation settings.
- Running pretrained models locally may require significant memory and processing resources.

##  Future Enhancements

- Develop an interactive Streamlit web application.
- Allow users to upload their own articles or documents.
- Add source highlighting to show where answers originate.
- Improve handling of long documents through chunking.
- Compare models using consistent evaluation metrics.
- Explore Retrieval-Augmented Generation (RAG) for larger collections of documents.
- Deploy the application using Hugging Face Spaces.

##  Disclaimer

This project is developed for educational and demonstration purposes. Generated summaries and answers should be reviewed for accuracy before being used for research or decision-making.

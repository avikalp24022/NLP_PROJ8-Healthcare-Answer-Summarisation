# NLP Project Baseline Benchmark

This repository contains the baseline benchmarking implementation for the **Healthcare Answer Summarization** project. The project aims to generate perspective-based summaries of healthcare-related answers while preserving intent and context.

## Dataset
The project utilizes the **PuMA dataset**, which consists of healthcare-related question-answer pairs. This dataset is used to train and evaluate the summarization model.

## Baseline Model
The model used for zero-shot training is **Deepseek-r1-distill-qwen-1.5B** and **facebooks BART-large-cnn**. These models are employed one after the other to generate summaries without explicit fine-tuning, leveraging its pre-trained capabilities.

## Evaluation
The summarization quality is assessed using:
- **BERTScore**
- **BLEU Score**

## Usage
To run the benchmark:
1. Ensure all required dependencies are installed.
2. Open the Jupyter Notebook.
3. Run the cells sequentially to process the dataset, generate summaries, and evaluate results.

## Dependencies
- Python 3.x
- Transformers
- Numpy
- Pandas
- Scikit-learn
- Torch
- Hugging Face Libraries

## Team Members
- Avikalp Rewatkar MT24022
- Sai Krishna Kota MT24078
- Shubhankar Tiwary MT24139
For more details, refer to the notebook in this repository.


# TOPSIS on Pre-Trained "Text Summarization" Models

## Overview
This project evaluates various pre-trained text summarization models using multiple performance metrics and ranks them using the TOPSIS (Technique for Order of Preference by Similarity to Ideal Solution) method. The models used in this study include:

- **BART** (facebook/bart-large-cnn)
- **T5** (t5-small)
- **PEGASUS** (google/pegasus-xsum)
- **LED** (allenai/led-base-16384)

## Features
- Generates text summaries using pre-trained models from Hugging Face.
- Evaluates the summaries using **BLEU** and **ROUGE** metrics.
- Compares models based on inference time and memory usage.
- Applies **TOPSIS** to rank models based on performance metrics.
- Visualizes results using Matplotlib and Seaborn.
- Saves evaluation results to CSV files.

## Installation
To run this project, install the required dependencies:
```bash
pip install numpy pandas matplotlib seaborn transformers evaluate
```

## Usage
Run the script to evaluate the text summarization models and compute their rankings.
```bash
python summarization_topsis.py
```

## Evaluation Metrics
The following metrics are used to assess the performance of each model:
- **BLEU Score**: Measures n-gram overlap between the generated summary and reference text.
- **ROUGE Scores (ROUGE-1, ROUGE-2, ROUGE-L)**: Evaluate recall-oriented n-gram matching.

## TOPSIS Evaluation
TOPSIS is used to rank models based on their evaluation metrics.
The models are ranked based on their similarity to the ideal best solution.

## Results
The project generates the following outputs:
- **summarization_results.csv**: Summaries and evaluation scores for each model.
- **topsis_results.csv**: TOPSIS scores and rankings of the models.
- **Comparison Plots**: Bar charts visualizing the performance of different models.
  
## License
This project is open-source and available for modification and distribution.

---
For any issues or contributions, feel free to open a pull request or raise an issue.


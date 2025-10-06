# Text Summarization Using Pre-trained Models

This project implements text summarization using pre-trained encoder-decoder models (T5, BART, Pegasus) as part of the Elevvo Pathway.

## 🎯 Project Goals

- Generate concise summaries from long documents using NLP models
- Use an encoder-decoder architecture (BART, T5, or Pegasus)
- Preprocess long texts and truncate to model input limits
- Evaluate summary quality using ROUGE scores

## 📊 Datasets

- **CNN/DailyMail**: News articles and human-written highlights
- **DialogSum**: Multi-turn dialogues and their summaries

## 🧠 Models Used

- `sshleifer/distilbart-cnn-12-6` — A smaller, faster version of BART fine-tuned on CNN/DM

## 🚀 Key Results

### Evaluation on CNN/DailyMail (Test Set, 100 samples)

| Metric     | Score   |
|------------|---------|
| ROUGE-1    | 0.3564  |
| ROUGE-2    | 0.1608  |
| ROUGE-L    | 0.2660  |

### Fine-tuning on DialogSum (Test Set, 100 samples)

| Metric     | Score   |
|------------|---------|
| ROUGE-1    | 0.4080  |
| ROUGE-2    | 0.1470  |
| ROUGE-L    | 0.3310  |

✅ **Improvement**: +5.2% ROUGE-1 compared to CNN/DM baseline

## 🛠️ Tools & Libraries

- Hugging Face Transformers
- Datasets
- ROUGE Score
- Pandas
- Matplotlib / Plotly (for visualization)

# EmoMix-3L: A Code-Mixed Dataset for Bangla-English-Hindi Emotion Detection

**Publication**: *The 7th Workshop on Indian Language Data: Resources and Evaluation (WILDRE) under LREC-COLING-2024.*

**Read in [arXiv](coming soon)** 

---

## 📝 Citation

If you utilize this dataset, kindly cite our paper.

```bibtex
@article{raihan2024emomix,
  title={EmoMix-3L: A Code-Mixed Dataset for Bangla-English-Hindi Emotion Detection},
  author={Raihan, Md Nishat and Goswami, Dhiman and Mahmud, Antara and Anstasopoulos, Antonios and Zampieri, Marcos},
  journal={Proceedings of The 7th Workshop on Indian Language Data: Resources and Evaluation (WILDRE) (LREC-COLING)},
  year={2024}
}
```
---

## 📖 Introduction

Code-mixing is a well-studied linguistic phenomenon that occurs when two or more languages are mixed in text or speech. Several studies have been conducted on building datasets and performing downstream NLP tasks on code-mixed data. Although it is not uncommon to observe code-mixing of three or more languages, most available datasets in this domain contain code-mixed data from only two languages. In this paper, we introduce EmoMix-3L, a novel multi-label emotion detection dataset containing code-mixed data from three different languages. We experiment with several models on **EmoMix-3L** and we report that MuRIL outperforms other models on this dataset.

---

## 📊 Dataset Details

We introduce **EmoMix-3L**, a novel three-language code-mixed test dataset with gold standard labels in Bangla-Hindi-English for the task of Emotion Detection, containing 1,071 instances.

> We are presenting this dataset exclusively as a test set due to the unique and specialized nature of the task. Such data is very difficult to gather and requires significant expertise to access. The size of the dataset, while limiting for training purposes, offers a high-quality testing environment with gold-standard labels that can serve as a benchmark in this domain.

---

## 📈 Dataset Statistics

| | **All** | **Bangla** | **English** | **Hindi** | **Other** |
|------------------|---------|------------|-------------|-----------|-----------|
| Tokens | 98,011 | 36,784 | 6,587 | 15,560 | 39,080 |
| Types | 21,766 | 9,118 | 1,237 | 1,523 | 10,022 |
| Avg | 91.51 | 34.35 | 6.15 | 14.53 | 36.49 |
| Std Dev | 20.24 | 9.13 | 2.88 | 5.94 | 10.64 |

*The row 'Avg' represents the average number of tokens with its standard deviation in row 'Std Dev'.*

---

## 📉 Results

| Models | F1 Score |
|-----------------|----------|
| MuRIL  | **0.54** |
| XLM-R | 0.51 |
| GPT 3.5 Turbo | 0.51 |
| BanglishBERT | 0.44 |
| HingBERT | 0.43 |
| emoBERTa | 0.42 |
| roBERTa | 0.41 |
| BERT | 0.38 |
| mBERT | 0.35 |
| DistilBERT | 0.24 |
| IndicBERT | 0.22 |
| BanglaBERT | 0.16 |
| HindiBERT | 0.14 |


*Weighted F-1 score for different models: training on synthetic, testing on natural data.*

---


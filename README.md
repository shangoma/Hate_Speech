# Multilingual_Fairness_LREC
Data and code repository to evaluate multilingual fairness for hate speech detection for the LREC 2020 paper [Multilingual Twitter corpus and baselines for evaluating demographic bias in hate speech recognition](https://arxiv.org/pdf/2002.10361.pdf).


# How to run evaluations
1. Install required packages;
    * Install conda;
    * Install pytorch;
    * Final: `pip install -r requirements.txt`.

2. Process pre-trained word embeddings;
    * Follow the [instructions](https://github.com/xiaoleihuang/Multilingual_Fairness_LREC/blob/master/resources/emb_steps.md).

3. Run python scripts
    * Test logistic regression classifier: `python lr.py`;
    * Test RNN classifier: `python rnn.py`;
    * Test CNN classifier: `python cnn.py`;
    * Test BERT classifier: `python bert.py`.


# Contact
To request non-binary demographic labels or if you have any issues,
please email **xiaolei.huang@colorado.edu**.


# Citation
If you use our corpus in your publication, please kindly cite this [paper](https://arxiv.org/pdf/2002.10361.pdf)):

```
@inproceedings{huang2020-lrec,
    title = "Multilingual Twitter Corpus and Baselines for Evaluating Demographic Bias in Hate Speech Recognition",
    author = "Huang, Xiaolei  and
      Linzi, Xing  and
      Dernoncourt, Franck  and
      Paul, Michael J.",
    booktitle = "Proceedings of the Twelveth International Conference on Language Resources and Evaluation ({LREC} 2020)",
    month = may,
    year = "2020",
    address = "Marseille, France",
    publisher = "European Language Resources Association (ELRA)",
    url = "https://arxiv.org/pdf/2002.10361.pdf",
    abstract = "Existing research on fairness evaluation of document classification models mainly uses synthetic monolingual data without ground truth for author demographic attributes. In this work, we assemble and publish a multilingual Twitter corpus for the task of hate speech detection with inferred four author demographic factors: age, country, gender and race/ethnicity. The corpus covers five languages: English, Italian, Polish, Portuguese and Spanish. We evaluate the inferred demographic labels with a crowdsourcing platform, Figure Eight. To examine factors that can cause biases, we take an empirical analysis of demographic predictability on the English corpus. We measure the performance of four popular document classifiers and evaluate the fairness and bias of the baseline classifiers on the author-level demographic attributes.",
}
```

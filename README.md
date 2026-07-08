# ShortTextAdversarialBenchmark

It is a comprehensive benchmark repository of adversarial short-text datasets designed for standardized robustness evaluation of natural language processing (NLP) models. The repository contains adversarial corpora generated using two widely adopted attack strategies: **TextFooler** and **adversarial paraphrasing**.

The benchmark has been developed to facilitate reproducible evaluation of NLP models under lexical and semantic adversarial attacks across multiple standard benchmark datasets.

---

## Repository Structure

```text
ShortTextAdvBench/
│
├── TextFooler/
│   ├── AGNews/
│   │   ├── agnews_minmul_All_K.csv
│   │   ├── agnews_minmul_k1.csv
│   │   ├── agnews_minmul_k2.csv
│   │   ├── agnews_minmul_k3.csv
│   │   ├── agnews_minmul_k4.csv
│   │   └── agnews_minmul_k5.csv
│   │
│   ├── Amazon/
│   │   ├── Amazon_minmul_All_K.csv
│   │   ├── Amazon_minmul_k1.csv
│   │   ├── Amazon_minmul_k2.csv
│   │   ├── Amazon_minmul_k3.csv
│   │   ├── Amazon_minmul_k4.csv
│   │   └── Amazon_minmul_k5.csv
│   │
│   ├── DBpedia/
│   └── YahooAnswers/
│
└── Paraphrased/
    ├── AGNews/
    │   ├── AGNews_T5.csv
    │   └── AGNews_BART.csv
    │
    ├── COCO/
    ├── HC3/
    └── Yelp/
```

---

## TextFooler-Based Adversarial Corpora

The **TextFooler** directory contains perturbation-controlled adversarial datasets generated using the TextFooler attack.

The following benchmark datasets are included:

* AG News
* Amazon Reviews
* DBpedia
* Yahoo Answers

Each dataset directory contains six CSV files:

* One combined file containing adversarial samples from all perturbation levels.
* Five individual CSV files corresponding to perturbation levels:

  * k = 1
  * k = 2
  * k = 3
  * k = 4
  * k = 5

This organization enables robustness evaluation at different perturbation strengths as well as on the complete adversarial corpus.

---

## Paraphrased Adversarial Corpora

The **Paraphrased** directory contains adversarial datasets generated using paraphrasing-based attacks.

The following benchmark datasets are included:

* AG News
* COCO
* HC3
* Yelp

Each dataset directory contains two CSV files:

* T5-generated adversarial paraphrases
* BART-generated adversarial paraphrases

These datasets enable evaluation against semantic-preserving adversarial attacks produced by different neural paraphrasing models.

---

## Benchmark Summary

| Attack Type  | Datasets                                        | Files per Dataset |
| ------------ | ----------------------------------------------- | ----------------- |
| TextFooler   | AG News, Amazon Reviews, DBpedia, Yahoo Answers | 6 CSV files       |
| Paraphrasing | AG News, COCO, HC3, Yelp                        | 2 CSV files       |

---

## Intended Use

This benchmark is intended for:

* Adversarial robustness evaluation
* Benchmarking NLP classification models
* Comparing heavyweight and lightweight transformer models
* Adversarial training
* Robustness analysis under lexical and semantic attacks
* Reproducible research

---

## Citation

If you use this benchmark in your research, please cite our paper.

**Citation information will be added after publication.**

---

## Updates

This repository will be continuously updated with:

* Additional benchmark datasets
* New adversarial attack methods
* Baseline implementations
* Evaluation scripts
* Documentation
* Citation information

---

## Contact

For questions, suggestions, or collaborations, please open an issue in this repository.


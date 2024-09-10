# IndicOOV
[![Paper](https://img.shields.io/badge/arXiv-2403.16973-brightgreen.svg?style=flat-square)](https://arxiv.org/pdf/2407.13435)
[![Website](https://img.shields.io/badge/website-indicoov)](https://ai4bharat.iitm.ac.in/indicoov/)

> 🎉 Accepted at INTERSPEECH 2024

We release IndicOOV, a benchmark for Hindi and Tamil with ~1300 words, spread over 6-7 categories, consisting of both In-Vocabulary (IV) and Out-of-Vocabulary (OOV) words.

We show in the paper that pronunciations of TTS models with poor vocabulary coverage can be improved by recording and finetuning on small amounts of carefully curated data, specifically improving the bigram coverage of the data. We release a benchmark to demonstrate the problem and hence exhibit the improvements via our proposed solution.

**Authors:** Srija Anand, Praveen S V, Ashwin Sankar, Giri Raju, Mitesh M. Khapra

## Abstract
Publicly available TTS datasets for low-resource languages like
Hindi and Tamil typically contain 10-20 hours of data, leading to poor vocabulary coverage. This limitation becomes evident in downstream applications where domain-specific vocab-
ulary coupled with frequent code-mixing with English, results in many OOV words. To highlight this problem, we create a benchmark containing OOV words from several real-world applications. Indeed, state-of-the-art Hindi and Tamil TTS systems perform poorly on this OOV benchmark, as indicated by intelligibility tests. To improve the model’s OOV performance, we propose a low-effort and economically viable strategy to obtain more training data. Specifically, we propose using volunteers as opposed to high quality voice artists to record words containing character bigrams unseen in the training data. We show that using such inexpensive data, the model’s performance improves on OOV words, while not affecting voice quality and in-domain performance.

## IndicOOV Benchmark
###  Hindi
The Hindi benchmark covers 6 categories:
1. abbreviations
2. brands
3. code_mixed
4. company_names
5. govt_schemes
6. proper_nouns

### Tamil
The Tamil benchmark covers 7 categories:
1. abbreviations
2. brands
3. code_mixed
4. proper_nouns
5. healthcare_medical_terms
6. education_literature
7. navigation

## Citation
If you want to use our benchmark, templates or recording scripts, please cite our work as follows:
```
@article{anand2024enhancingoutofvocabularyperformanceindian,
      title={Enhancing Out-of-Vocabulary Performance of Indian TTS Systems for Practical Applications through Low-Effort Data Strategies}, 
      author={Srija Anand and Praveen Srinivasa Varadhan and Ashwin Sankar and Giri Raju and Mitesh M. Khapra},
      year={2024},
      eprint={2407.13435},
      url={https://arxiv.org/abs/2407.13435}, 
}
```

We used the implementation of VITS by [jaywalnut310](https://github.com/jaywalnut310/vits) and the [Indic-TTS](https://github.com/AI4Bharat/Indic-TTS) Fastpitch model released by AI4Bharat trained in the Coqui framework.



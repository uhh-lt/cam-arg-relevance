# cam-arg-relevance

This repo contains code and data for the paper "How to Compare Things Properly? A Study of Argument Relevance in Comparative Question Answering" accepted to Main ACL 2025. Here you could find the instructions to reproduce all our results.

The repo is structured as follows:

In the `data/` folder the following files can be found:

### Argument relevance data

- [`expert_annotation.xlsx`](data/expert_annotation.xls) with the expert annotations for argument relevance
- [`assignments_from_pool_42774131__05-02-2024.tsv`](data/assignments_from_pool_42774131__05-02-2024.tsv) with the annotations from Toloka for argument relevance
- [`dataset_cqa_all_gpt.json`](data/dataset_cqa_all_gpt.json) is the final dataset with the final human annotations and GPT4 annotations for argument relevance. The human annotations are collected as the "most common" annotations from toloka and experts whenever possible. This dataset is to be used for further experiments for argument relevance

### Comparative QA datasets

- [`gold_40_plus_10x4.json`](data/gold_40_plus_10x4.json)
- [`silver_112x3.json`](data/silver_112x3.json)
- [`silver_50x3.json`](data/silver_50x3.json)

in the root path `/` the following files can be found:

- [`relevance vs quality instructions.pdf`](relevance vs quality instructions.pdf)
- [`experiments.ipynb`](experiments.ipynb)
- [`Toloka_Annotator_Agreement.ipynb`](Toloka_Annotator_Agreement.ipynb)

### Link to the paper: [link](TBD)

### Citation

```
TBD
```

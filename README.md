# cam-arg-relevance

This repo contains code and data for the paper "How to Compare Things Properly? A Study of Argument Relevance in Comparative Question Answering" accepted to Main ACL 2025. Here you could find the instructions to reproduce all our results.

The repo is structured as follows:

In the `data/` folder the following files can be found:

### Argument relevance data

- [`expert_annotation.xlsx`](data/expert_annotation.xls) with the expert annotations for argument relevance
- [`assignments_from_pool_42774131__05-02-2024.tsv`](data/assignments_from_pool_42774131__05-02-2024.tsv) with the annotations from Toloka for argument relevance
- [`dataset_cqa_all_gpt.json`](data/dataset_cqa_all_gpt.json) is the final dataset with the final human annotations and GPT4 annotations for argument relevance. The human annotations are collected as the "most common" annotations from toloka and experts whenever possible. This dataset is to be used for further experiments for argument relevance

### Comparative QA datasets

- [`silver_112x3.json`](data/silver_112x3.json) To create the comparative answers based on the retrieved arguments using the developed prompt, we used the ChatGPT model (gpt-3.5-turbo, default parameters) from OpenAI. We returned top $3$ answers to evaluate possible variations of the answer and checked how well the model follows the required structure.
- [`gold_40_plus_10x4.json`](data/gold_40_plus_10x4.json) To construct the __Gold dataset__ of better quality, we engaged four expert annotators to refine and improve 50 selected outputs. As a part of the calibration process, all experts first annotated the same set of 10 summaries and discussed each other’s revisions. Subsequently, each expert independently edited 10 additional summaries. The resulting __Gold dataset__ consists of 50 comparative questions and 80 manually curated summaries (10 shared and 10 individual questions and answers for four experts).
- [`silver_50x3.json`](data/silver_50x3.json) A subset of __Silver dataset__ for the corresponding questions from __Gold__

in the root path `/` the following files can be found:

- [`relevance vs quality instructions.pdf`](relevance vs quality instructions.pdf) with the annotation instructions for the argument relevance
- [`Annotator_Agreement.ipynb`](Annotator_Agreement.ipynb) is the IPython notebook with the annotation agreement calculations for all annotated dat
- [`experiments.ipynb`](experiments.ipynb) is the IPython notebook with the framework evaluation code

### Link to the paper: [link](TBD)

### Citation

```
TBD
```

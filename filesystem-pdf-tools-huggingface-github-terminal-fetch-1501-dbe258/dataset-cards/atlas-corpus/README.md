---
license: cc-by-sa-4.0
pretty_name: Atlas Pre-Training Corpus
language:
- en
tags:
- text-generation
- pre-training
dataset_info:
- config_name: code-mini
  features:
  - name: blob_id
    dtype: string
  - name: repo_name
    dtype: string
  - name: path
    dtype: string
  - name: length_bytes
    dtype: int64
  - name: score
    dtype: float64
  splits:
  - name: train
    num_examples: 1840000
- config_name: web-prose
  features:
  - name: url
    dtype: string
  - name: text
    dtype: string
  - name: language
    dtype: string
  splits:
  - name: train
    num_examples: 9200000
- config_name: math-reasoning
  features:
  - name: problem
    dtype: string
  - name: solution
    dtype: string
  splits:
  - name: train
    num_examples: 410000
configs:
- config_name: code-mini
  data_files: data/code-mini/*.parquet
- config_name: web-prose
  data_files: data/web-prose/*.parquet
- config_name: math-reasoning
  data_files: data/math-reasoning/*.parquet
---

# Atlas Pre-Training Corpus

The Atlas Pre-Training Corpus is a curated collection of code, web prose and
mathematical reasoning records assembled for pre-training language models.

Each configuration listed in the card metadata is stored under `data/` and
follows the feature schema declared for that configuration. The corpus is
released under the terms stated in the card metadata.

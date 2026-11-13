---
license: mit
pretty_name: code-mini annotations
tags:
- annotations
- evaluation
dataset_info:
- config_name: annotations
  features:
  - name: annotation_id
    dtype: string
  - name: blob_id
    dtype: string
  - name: label
    dtype: string
  - name: rationale
    dtype: string
  - name: annotator
    dtype: string
  splits:
  - name: train
    num_examples: 24000
configs:
- config_name: annotations
  data_files: annotations/annotations.jsonl
---

# code-mini annotations

Human review annotations collected over a sample of code-mini records. This
folder holds annotation artifacts produced by the evaluation group for quality
review. It is not a copy of the training corpus.

Each annotation record contains `annotation_id`, `blob_id`, `label`, `rationale`
and `annotator`.

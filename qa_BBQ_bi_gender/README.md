---
configs:
- config_name: default
  data_files:
  - split: validation
    path: data/validation-*
dataset_info:
  features:
  - name: example_id
    dtype: int64
  - name: question_index
    dtype: string
  - name: question_polarity
    dtype: string
  - name: context_condition
    dtype: string
  - name: category
    dtype: string
  - name: answer_info
    struct:
    - name: ans0
      sequence: string
    - name: ans1
      sequence: string
    - name: ans2
      sequence: string
  - name: additional_metadata
    struct:
    - name: source
      dtype: string
    - name: stereotyped_groups
      sequence: string
    - name: subcategory
      dtype: string
    - name: version
      dtype: string
  - name: context
    dtype: string
  - name: question
    dtype: string
  - name: ans0
    dtype: string
  - name: ans1
    dtype: string
  - name: ans2
    dtype: string
  - name: label
    dtype: int64
  - name: audio
    dtype:
      audio:
        sampling_rate: 16000
  - name: ASR_LLM_Prompt
    dtype: string
  - name: SLLM_Prompt
    dtype: string
  - name: tts_provider
    dtype: string
  - name: speaker
    dtype: string
  - name: __index_level_0__
    dtype: int64
  splits:
  - name: validation
    num_bytes: 1575148772.928
    num_examples: 5136
  download_size: 717986547
  dataset_size: 1575148772.928
---
# Dataset Card for "qa_BBQ_bi_gender"

[More Information needed](https://github.com/huggingface/datasets/blob/main/CONTRIBUTING.md#how-to-contribute-to-the-dataset-cards)
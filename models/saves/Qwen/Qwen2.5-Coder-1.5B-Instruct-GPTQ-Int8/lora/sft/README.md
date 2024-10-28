---
base_model: /home/zane/models/Qwen/Qwen2.5-Coder-1.5B-Instruct-GPTQ-Int8
library_name: peft
license: other
tags:
- llama-factory
- lora
- generated_from_trainer
model-index:
- name: sft
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sft

This model is a fine-tuned version of [/home/zane/models/Qwen/Qwen2.5-Coder-1.5B-Instruct-GPTQ-Int8](https://huggingface.co//home/zane/models/Qwen/Qwen2.5-Coder-1.5B-Instruct-GPTQ-Int8) on the intebull_data_zh_json_1377_trainset, the alpaca_zh_demo and the identity datasets.
It achieves the following results on the evaluation set:
- Loss: 0.9508

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 0.0001
- train_batch_size: 1
- eval_batch_size: 1
- seed: 42
- gradient_accumulation_steps: 10
- total_train_batch_size: 10
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: cosine
- lr_scheduler_warmup_ratio: 0.1
- num_epochs: 3.0

### Training results

| Training Loss | Epoch  | Step | Validation Loss |
|:-------------:|:------:|:----:|:---------------:|
| 1.6797        | 0.1241 | 20   | 1.5946          |
| 1.3769        | 0.2483 | 40   | 1.3096          |
| 1.3993        | 0.3724 | 60   | 1.1146          |
| 1.192         | 0.4966 | 80   | 1.0488          |
| 1.0924        | 0.6207 | 100  | 1.0258          |
| 1.237         | 0.7449 | 120  | 1.0122          |
| 1.0941        | 0.8690 | 140  | 1.0047          |
| 1.1428        | 0.9932 | 160  | 0.9919          |
| 0.9865        | 1.1173 | 180  | 0.9849          |
| 1.0094        | 1.2415 | 200  | 0.9802          |
| 0.9474        | 1.3656 | 220  | 0.9658          |
| 1.0501        | 1.4898 | 240  | 0.9575          |
| 1.151         | 1.6139 | 260  | 0.9540          |
| 0.9522        | 1.7381 | 280  | 0.9558          |
| 0.9346        | 1.8622 | 300  | 0.9522          |
| 1.0998        | 1.9863 | 320  | 0.9489          |
| 0.8902        | 2.1105 | 340  | 0.9534          |
| 0.8351        | 2.2346 | 360  | 0.9545          |
| 0.8782        | 2.3588 | 380  | 0.9508          |
| 0.8926        | 2.4829 | 400  | 0.9516          |
| 0.8596        | 2.6071 | 420  | 0.9517          |
| 0.903         | 2.7312 | 440  | 0.9507          |
| 0.9322        | 2.8554 | 460  | 0.9501          |
| 1.0011        | 2.9795 | 480  | 0.9511          |


### Framework versions

- PEFT 0.12.0
- Transformers 4.45.2
- Pytorch 2.4.1+cu121
- Datasets 2.21.0
- Tokenizers 0.20.1
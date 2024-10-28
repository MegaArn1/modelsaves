---
base_model: /home/zane/models/Qwen/Qwen2.5-Coder-1.5B-Instruct-GPTQ-Int8
library_name: peft
license: other
tags:
- llama-factory
- lora
- generated_from_trainer
model-index:
- name: sft_2
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sft_2

This model is a fine-tuned version of [/home/zane/models/Qwen/Qwen2.5-Coder-1.5B-Instruct-GPTQ-Int8](https://huggingface.co//home/zane/models/Qwen/Qwen2.5-Coder-1.5B-Instruct-GPTQ-Int8) on the intebuil_data_zh_json_trainset_2_edi, the alpaca_zh_demo and the identity datasets.
It achieves the following results on the evaluation set:
- Loss: 1.3532

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
- gradient_accumulation_steps: 8
- total_train_batch_size: 8
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: cosine
- lr_scheduler_warmup_ratio: 0.1
- num_epochs: 3.0

### Training results

| Training Loss | Epoch  | Step | Validation Loss |
|:-------------:|:------:|:----:|:---------------:|
| 1.6442        | 0.1279 | 20   | 1.7679          |
| 1.6603        | 0.2558 | 40   | 1.6014          |
| 1.5204        | 0.3837 | 60   | 1.4685          |
| 1.4968        | 0.5116 | 80   | 1.3978          |
| 1.373         | 0.6395 | 100  | 1.3858          |
| 1.1256        | 0.7674 | 120  | 1.3753          |
| 1.4524        | 0.8953 | 140  | 1.3633          |
| 1.3205        | 1.0232 | 160  | 1.3535          |
| 1.3637        | 1.1511 | 180  | 1.3545          |
| 1.1435        | 1.2790 | 200  | 1.3520          |
| 1.1793        | 1.4069 | 220  | 1.3486          |
| 1.2259        | 1.5348 | 240  | 1.3487          |
| 1.2985        | 1.6627 | 260  | 1.3440          |
| 1.1612        | 1.7906 | 280  | 1.3405          |
| 1.3262        | 1.9185 | 300  | 1.3401          |
| 1.1695        | 2.0464 | 320  | 1.3408          |
| 1.1854        | 2.1743 | 340  | 1.3458          |
| 1.1312        | 2.3022 | 360  | 1.3488          |
| 1.1352        | 2.4301 | 380  | 1.3513          |
| 1.2237        | 2.5580 | 400  | 1.3526          |
| 0.9727        | 2.6859 | 420  | 1.3533          |
| 1.038         | 2.8137 | 440  | 1.3531          |
| 1.1218        | 2.9416 | 460  | 1.3536          |


### Framework versions

- PEFT 0.12.0
- Transformers 4.45.2
- Pytorch 2.4.1+cu121
- Datasets 2.21.0
- Tokenizers 0.20.1
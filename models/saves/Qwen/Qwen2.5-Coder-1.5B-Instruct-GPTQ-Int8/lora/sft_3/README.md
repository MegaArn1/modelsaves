---
base_model: /home/zane/models/Qwen/Qwen2.5-Coder-1.5B-Instruct-GPTQ-Int8
library_name: peft
license: other
tags:
- llama-factory
- lora
- generated_from_trainer
model-index:
- name: sft_3
  results: []
---

<!-- This model card has been generated automatically according to the information the Trainer had access to. You
should probably proofread and complete it, then remove this comment. -->

# sft_3

This model is a fine-tuned version of [/home/zane/models/Qwen/Qwen2.5-Coder-1.5B-Instruct-GPTQ-Int8](https://huggingface.co//home/zane/models/Qwen/Qwen2.5-Coder-1.5B-Instruct-GPTQ-Int8) on the intebuil_data_zh_json_trainset_2_edi, the alpaca_zh_demo and the identity datasets.
It achieves the following results on the evaluation set:
- Loss: 1.5852

## Model description

More information needed

## Intended uses & limitations

More information needed

## Training and evaluation data

More information needed

## Training procedure

### Training hyperparameters

The following hyperparameters were used during training:
- learning_rate: 5e-05
- train_batch_size: 2
- eval_batch_size: 1
- seed: 42
- gradient_accumulation_steps: 5
- total_train_batch_size: 10
- optimizer: Adam with betas=(0.9,0.999) and epsilon=1e-08
- lr_scheduler_type: linear
- lr_scheduler_warmup_ratio: 0.1
- num_epochs: 3.0

### Training results

| Training Loss | Epoch  | Step | Validation Loss |
|:-------------:|:------:|:----:|:---------------:|
| 1.7804        | 0.3994 | 50   | 1.8317          |
| 1.5086        | 0.7987 | 100  | 1.7283          |
| 1.6525        | 1.1981 | 150  | 1.6724          |
| 1.6763        | 1.5974 | 200  | 1.6298          |
| 1.5592        | 1.9968 | 250  | 1.6079          |
| 1.7004        | 2.3962 | 300  | 1.5929          |
| 1.4992        | 2.7955 | 350  | 1.5856          |


### Framework versions

- PEFT 0.12.0
- Transformers 4.45.2
- Pytorch 2.4.1+cu121
- Datasets 2.21.0
- Tokenizers 0.20.1
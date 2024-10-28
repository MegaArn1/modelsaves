---
base_model: /home/zane/models/Qwen/Qwen2.5-Coder-7B-Instruct-GPTQ-Int8
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

This model is a fine-tuned version of [/home/zane/models/Qwen/Qwen2.5-Coder-7B-Instruct-GPTQ-Int8](https://huggingface.co//home/zane/models/Qwen/Qwen2.5-Coder-7B-Instruct-GPTQ-Int8) on the intebuil_data_zh_json_trainset_2_edi, the alpaca_zh_demo and the identity datasets.
It achieves the following results on the evaluation set:
- Loss: 1.3877

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
| 1.6163        | 0.3994 | 50   | 1.6648          |
| 1.352         | 0.7987 | 100  | 1.5333          |
| 1.4665        | 1.1981 | 150  | 1.4726          |
| 1.4775        | 1.5974 | 200  | 1.4326          |
| 1.3467        | 1.9968 | 250  | 1.4110          |
| 1.4752        | 2.3962 | 300  | 1.3966          |
| 1.3146        | 2.7955 | 350  | 1.3889          |


### Framework versions

- PEFT 0.12.0
- Transformers 4.45.2
- Pytorch 2.4.1+cu121
- Datasets 2.21.0
- Tokenizers 0.20.1
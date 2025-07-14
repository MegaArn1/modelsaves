# Configuration Files

This directory contains configuration files used for training and model setup.

## Structure

- `training_configs/` - Training configuration files for LLaMA-Factory
- `model_configs/` - Model configuration and hyperparameter files

## Training Configs

Training configurations should include:
- Learning rate schedules
- Batch sizes and gradient accumulation
- LoRA/QLoRA parameters
- Dataset configurations
- Training objectives

## Model Configs

Model configurations should specify:
- Model architecture parameters
- Tokenizer settings
- Special tokens configuration
- Model-specific hyperparameters

## File Format

All configuration files should be in JSON or YAML format for easy version control and readability.

Example structure:
```
training_configs/
├── llama2_7b_lora.json
├── llama2_13b_qlora.yaml
└── base_training_config.json

model_configs/
├── llama2_7b_config.json
├── custom_tokenizer_config.json
└── deployment_config.yaml
```
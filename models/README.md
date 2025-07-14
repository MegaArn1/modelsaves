# Models Directory

This directory contains all trained models and their variations.

## Structure

- `checkpoints/` - Training checkpoints saved during the training process
- `final_models/` - Final trained models ready for deployment
- `adapters/` - LoRA/QLoRA adapters for parameter-efficient fine-tuning

## Naming Convention

Models should follow this naming pattern:
```
{model_base}_{task}_{version}_{date}
```

Example: `llama2_7b_chat_v1.0_20241028`

## File Formats

- `.pt` / `.pth` - PyTorch model files
- `.bin` - Hugging Face model weights
- `.safetensors` - Safe tensor format (recommended)
- `.json` - Model configuration files

## Usage

All model files should be tracked with Git LFS. To add a new model:

```bash
git lfs track "models/**/*.bin"
git lfs track "models/**/*.pth"
git lfs track "models/**/*.safetensors"
git add .gitattributes
git add models/
git commit -m "Add new model: [model_name]"
```
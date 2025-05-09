# LayoutDiffusion-Repro

A PyTorch-based reproduction of the LayoutDiffusion model proposed in the paper:  
**"LayoutDiffusion: Content-Aware Layout Generation with Denoising Diffusion Models"**  
[[arXiv:2305.18252](https://arxiv.org/abs/2305.18252)]

---

## 🚧 Project Status

This is a work-in-progress implementation aiming to reproduce key components and results from the LayoutDiffusion paper.

- [x] Paper reading and model structure analysis  
- [x] Dataset preparation (PubLayNet / RICO or custom layouts)  
- [ ] Layout encoder & DDPM forward process  
- [ ] Cross-modal conditioning (category, image, text embedding)  
- [ ] Loss functions and training pipeline  
- [ ] Sampling & layout rendering  

---

## 📄 Paper Summary

LayoutDiffusion is a content-aware layout generation method that formulates layout synthesis as a denoising diffusion process. Key contributions include:

- Category-conditional layout generation  
- Cross-modal embeddings for alignment  
- Transformer-based architecture with DDPM backbone  

---

## 📁 Folder Structure
.
├── configs/ # YAML or JSON training configs
├── datasets/ # Processed layout datasets
├── models/ # Diffusion model, transformer blocks, encoders
├── scripts/ # Training and evaluation scripts
├── utils/ # Data loaders, metrics, visualizations
└── main.py # Entry point

---

## 📦 Requirements

```bash
pip install torch torchvision einops matplotlib numpy
pip install diffusers transformers # optional if using Huggingface tools


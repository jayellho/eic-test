# EIC Lab Application

## Prerequisites
1. `uv` package manager

## Getting started.
1. Set up virtual environment `eic-test-venv` using `uv` and install packages.
```bash
uv venv eic-test-venv
source eic-test-venv/bin/activate
uv pip install -r requirements.txt
```
1. d
2. 
## To-do
- [ ] Set-up GPT-2 model and SQuAD dataset.
- [ ] Read "LLM-QAT - Data-Free Quantization Aware Training"
- [ ] Read "LoRA - Low-Rank Adaptation of LLMs"
- [ ] Read "InstantNet - Automated Generation and Deployment"
- [ ] Integrate quantization into pretrained GPT-2 model.
- [ ] Add LoRA modules to all linear layers.
- [ ] Implement function to adaptively activate different LoRA modules in each layer during inference based on input config.
- [ ] Tune GPT-2 model for 1000 iterations on SQuAD dataset with different per-layer quantization bit-width configurations at the same time (i.e. enable switchable precision).
- [ ] Evaluate performance of tuned model under different quantization bit-width configurations on SQuAD dataset.
- [ ] Instead of jointly training on all bit-widths, use cyclic precision training to dynamically change the training bit-widths throughout the tuning process and investigate performance of this quantization strategy.
- [ ] On top of a pretrained GPT-2, examine whether random precision switch can improve GPT-2's adversarial robustness via literature review.
- [ ] Pick arbitrary widely used adversarial attacks within 3 years to evaluate GPT-2's adversarial robustness.
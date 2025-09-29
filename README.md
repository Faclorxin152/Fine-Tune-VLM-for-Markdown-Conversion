# Fine-Tune-VLM-for-Markdown-Conversion

![Example 01](/Fine-Tune-VLM-for-Markdown-Conversion/output/01/input.jpg)  
![Example 02](/Fine-Tune-VLM-for-Markdown-Conversion/output/02/input.jpg)

This repository fine-tunes a 3B Vision-Language Model (VLM) for the task of converting financial tables from images into clean Markdown format.  

By referring to the paper **"Fine-Tuning Vision-Language Models for Markdown Conversion of Financial Tables in Malaysian Audited Financial Reports"**, we have applied the same method and datasets from [jinkhye/MyFinMarkdown-sample](https://huggingface.co/datasets/jinkhye/MyFinMarkdown-sample).  

The model being fine-tuned is **Qwen/Qwen2.5-VL-3B-Instruct**, trained only on 10 samples of data. We use **LoRA adapter** and **4-bit quantization**, with minimal additional parameters to make training feasible on limited resources (in this case, a GTX 1060 6GB).  

---

## Reference

- [Fine-tuning VLM with TRL Cookbook](https://huggingface.co/learn/cookbook/en/fine_tuning_vlm_trl)  
- [TRL SFT Trainer Documentation](https://huggingface.co/docs/trl/en/sft_trainer)  
- [MyFinMarkdown-sample Dataset](https://huggingface.co/datasets/jinkhye/MyFinMarkdown-sample)  
- [MyFinMarkdown-bench Dataset](https://huggingface.co/datasets/jinkhye/MyFinMarkdown-bench)  
- [MyFinMarkdown GitHub](https://github.com/jinkhye/MyFinMarkdown)  
- [Paper (arXiv:2508.05669)](https://arxiv.org/pdf/2508.05669)  

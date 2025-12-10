# Fine-Tuning-Google-Gemma-2B-Using-LoRA-QLoRA
This project demonstrates how to fine-tune the Google Gemma 2B Instruct model using LoRA (Low-Rank Adaptation) and QLoRA (Quantized LoRA) to efficiently adapt a large language model for specialized tasks. 
The goal was to explore Parameter Efficient Fine-Tuning (PEFT) techniques to:  
Reduce training cost  Enable training on consumer-grade hardware 
Enable training on consumer-grade hardware
Maintain performance and general knowledge of the base model
Achieve specialization for domain-specific responses

This project serves as a complete reference pipeline for modern fine-tuning workflows.

Why LoRA / QLoRA?

Traditional full fine-tuning requires modifying all model weights, which is costly and often unnecessary.

LoRA and QLoRA modify only a small subset (low-rank matrices) while keeping most of the base model frozen.

Technologies Used

Model: Google Gemma-2B-Instruct

Frameworks: Transformers, PEFT, Datasets, BitsAndBytes

Training Method: LoRA & QLoRA (4-bit NF4 quantization)

Deployment: Inference notebook (optional Gradio/Streamlit UI)

Hardware: Google Colab T4 / local RTX GPU

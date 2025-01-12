
# Speculative Decoding with TopK-ImpSpecDec

## Overview

This repository presents a new speculative decoding method introduce in a deep learning class project, **TopK-ImpSpecDec**, designed to accelerate inference in Large Language Models (LLMs) while maintaining high-quality outputs. By combining **Top-K candidate selection** and **importance sampling**, this method addresses critical challenges in token generation, achieving:

- **Significantly higher token acceptance rates** compared to standard speculative decoding.
- **Enhanced inference speed** in long-text generation.
- **Improved resource efficiency**, making it suitable for memory-constrained environments.

## Highlights

1. **Novel Approach**: Integrates advanced statistical sampling techniques to overcome the limitations of traditional speculative decoding methods, such as low acceptance rates and memory inefficiency.
2. **Extensive Evaluation**: The method is rigorously tested across diverse datasets (e.g., WikiText-103, Alpaca, CNN/DailyMail) and parameter configurations, demonstrating its robustness and scalability.
3. **Real-World Application**: Offers a practical solution for faster, coherent, and resource-efficient LLM inference, ideal for applications in natural language processing, content generation, and summarization.

## Key Features

- **Dual Algorithm Implementation**: Includes both the original speculative decoding algorithm and the enhanced TopK-ImpSpecDec method.
- **Dataset Compatibility**: Preprocessed for compatibility with major datasets, including Alpaca, ensuring reproducibility and seamless integration.
- **Detailed Analysis**: Experimental results, including acceptance rate improvements and speed-up metrics, are available in the accompanying report for in-depth insights.
- **Work Example**: The repository includes code and an example implementation using the Alpaca dataset.
- **LLM Utilization**: The methodology leverages the LLaMA models, using LLaMA-160M as the draft model and LLaMA-7B as the target model, ensuring efficient token generation with robust alignment.

## Getting Started

The repository contains:

- The implementation of **TopK-ImpSpecDec** and baseline speculative decoding.
- Scripts for dataset preprocessing and experimental evaluation.
- Comprehensive documentation for replicating results and adapting the method to other tasks.
- **Code specific to the Alpaca dataset** as a working example.

### Prerequisites

- Python 3.8+
- TensorFlow or PyTorch (tested with NVIDIA A100 GPUs)
- Required libraries (listed in `requirements.txt`)

## Experimental Results

Our approach outperforms standard speculative decoding, achieving:

- **~3x improvement in token acceptance rates**.
- **Competitive speed-ups** with enhanced coherence in generated text.
- **Seamless scalability** for resource-limited setups.

For a complete analysis of our results, including parameter optimization and dataset-specific insights, refer to the detailed report in this repository.

## Acknowledgments

This work builds on foundational research in speculative decoding and statistical sampling. Special thanks to the contributors of the Alpaca dataset, the authors of key speculative decoding frameworks, and the developers of the LLaMA model family for their inspiration and groundwork.



# PEFT Approaches: LoRA, DoRA, and QLoRA

This repository contains the implementation of several **Parameter-Efficient Fine-Tuning (PEFT)** methods, including **LoRA**, **DoRA**, and **QLoRA**, applied to large models like GPT-2 and compared against Full Fine-Tuning. We explore the trade-offs in model size, training time, and validation accuracy, showcasing the efficiency of these methods in fine-tuning large models on small datasets.

This repo goes with the article [Exploring Parameter-Efficient Fine-Tuning (PEFT)](https://app.readytensor.ai/publications/exploring_parameter-efficient_fine-tuning_peft_r95vGYcr1shK)

## Overview

In this repository, you'll find:
- **LoRA**: Low-Rank Adaptation of pre-trained models.
- **DoRA**: Weight-decomposed Low-Rank Adaptation.
- **QLoRA**: Quantized Low-Rank Adaptation for highly efficient memory usage.
- Comparisons of these approaches with **Full Fine-Tuning** on the SST-2 dataset.

## Key Features
- **Memory Efficiency**: Significant reductions in model size using QLoRA.
- **Training Time**: Execution time comparisons showing the speedup gained with PEFT methods.
- **Generalization**: Analysis of how overfitting can occur in Full Fine-Tuning and how PEFT methods help prevent it.

## Results
- **QLoRA** reduces model size by **84%**, cutting down from 2.88GB to 0.46GB.
- **LoRA** achieves better validation accuracy than Full Fine-Tuning, demonstrating its generalization capability.
- **Full Fine-Tuning** has the lowest training loss but tends to overfit on smaller datasets.

## Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/peft-approaches.git
   cd peft-approaches
   ```

2. **Install dependencies**:
   Create a virtual environment and install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the experiments**:
   Execute the provided notebook to run the training and evaluation of the different approaches.


## Visualizations

The repository includes various plots to compare inside the **`/imgs`** directory:
- **Training Loss & Validation Accuracy** across the approaches.
- **Model Size** comparison, demonstrating the reduction in memory footprint using QLoRA.
- **Execution Time** comparisons showing the speedup with PEFT methods.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


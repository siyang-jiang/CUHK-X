# CUHK-X
A large-scale, multimodal dataset and benchmark for Human Action Recognition, Understanding and Reasoning

## Introduction

CUHK-X is a large-scale, multimodal dataset and benchmark designed for human action recognition, understanding, and reasoning. The dataset covers a wide range of action categories and includes video, audio, and text modalities, aiming to advance research in human behavior understanding.

## Dataset Features

- **Multimodal**: Includes video, audio, and text data for each sample.
- **Large-scale**: Contains tens of thousands of annotated action samples, suitable for deep learning.
- **Diversity**: Rich action categories and diverse scenarios for various downstream tasks.
- **Detailed Annotation**: Each sample is carefully annotated for accurate training and evaluation.

## Usage

1. **Download**
   Please visit the official website or contact the authors to request access to the dataset.

2. **Data Structure**
   The dataset consists of multiple modalities:
   - `videos/`: Action videos
   - `audios/`: Audio recordings
   - `annotations/`: Action annotations (JSON/CSV)
   - `texts/`: Text descriptions

3. **Quick Start**
   - Install dependencies:
     ```sh
     pip install -r requirements.txt
     ```
   - Load data example (Python):
     ```python
     from cukhx import CUHKXDataset
     dataset = CUHKXDataset(data_root='path/to/data')
     for sample in dataset:
         print(sample['video'], sample['audio'], sample['text'], sample['label'])
     ```

4. **Benchmark Evaluation**
   Baseline models and evaluation scripts are provided in the `benchmark/` directory.

## Contact

For dataset access or questions, please contact:
- Email: siyangjiang@cuhk.edu.hk

## Citation

If you use CUHK-X in your research, please cite our paper (see PDF for details).

---

For more details, please refer
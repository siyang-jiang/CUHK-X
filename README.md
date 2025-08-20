# CUHK-X
A large-scale, multimodal dataset and benchmark for Human Action Recognition, Understanding and Reasoning

# CUHK-X

CUHK-X 是一個大規模、多模態的人體行為識別、理解與推理數據集與基準。該數據集涵蓋了豐富的行為類型，包含視頻、語音、文本等多種模態，旨在推動人類行為理解領域的研究。

## 數據集特點

- **多模態**：包含視頻、語音、文本等多種數據模態。
- **大規模**：涵蓋數萬條行為樣本，支持深度學習模型訓練。
- **多樣性**：行為類型豐富，場景多樣，適用於多種下游任務。
- **標註詳盡**：每條數據均有詳細行為標註，便於模型訓練與評估。

## 使用方法

1. **下載數據集**  
   請訪問官方網站或聯繫作者獲取數據集下載方式。

2. **數據格式**  
   數據以多模態文件組成，包含：
   - `videos/`：行為視頻
   - `audios/`：語音數據
   - `annotations/`：行為標註文件（JSON/CSV）
   - `texts/`：文本描述

3. **快速開始**
   - 安裝依賴：
     ```sh
     pip install -r requirements.txt
     ```
   - 加載數據示例（Python）：
     ```python
     from cukhx import CUHKXDataset
     dataset = CUHKXDataset(data_root='path/to/data')
     for sample in dataset:
         print(sample['video'], sample['audio'], sample['text'], sample['label'])
     ```

4. **基準評測**
   數據集附帶多種基準模型與評測腳本，詳見 `benchmark/` 目錄。

## 聯繫我們

如需獲取數據集或有任何問題，請聯繫作者：  
- Email: siyangjiang@cuhk.edu.hk

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
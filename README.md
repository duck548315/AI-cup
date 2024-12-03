# AI-cup

此repository包含可復現實驗方法的程式碼、所使用到的資料集以及此說明文件

## Project Description

此程式碼主要包含三個部分:
- 訓練集之前處理與合併
- 測試集之前處理與特徵預測
- 目標模型訓練與預測

## File Structure

- `aicup_final.ipynb`: 主要程式碼
- Input data:
  - `base_path = '/content/drive/MyDrive/data'`: 將此path改為data所在之path
  - `add_path = '/content/drive/MyDrive/data/addit'`: 將此path改為addit所在之path(addit已在data內)
  - `testset.csv'`:位於
- Output:
  - Model predictions and performance metrics.

## Prerequisites

To run this project, you need the following:

- Python 3.8 or higher
- Required libraries: `numpy`, `pandas`, `sklearn`, `matplotlib`, `seaborn`, `lightgbm`
- Jupyter Notebook (for running the `.ipynb` file)

You can install the dependencies using:
```bash
pip install -r requirements.txt

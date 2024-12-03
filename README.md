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
  - `test_file = os.path.join(os.getcwd(), 'testset.csv')`:將testset.csv上傳至google colab即可(testset.csv在data內)
- Output:
  - output之訓練集、測試集、模型、結果皆在google colab預設的位置

## Prerequisites

環境需求:

- Google Colab
- Python 3.10.12以上
- Required libraries:`os`, `numpy`, `pandas`, `sklearn.model_selection`, `sklearn.metrics`, `xgboost`, `pickle`

## Usage

只要依照儲存格順序依序執行即可，以下檔案皆儲存在google colab /content之下
- 執行完第一個儲存格會得到:
- `full_train_data.csv`: 訓練資料集
  
- 執行完第二個儲存格會得到:
- `(feature_name)_model.pkl`: 特徵模型1
- `(feature_name)_model_v2.pkl`: 特徵模型2
- `xgbBoost_test_final.csv`: 測試資料集

- 執行完第三個儲存格會得到:
- `xgb_model.pkl`: 發電量模型
- `XGBoost_Predictions_xgb.csv.csv`: 預測結果

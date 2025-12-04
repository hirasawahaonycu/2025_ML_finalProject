# 2025_ML_finalProject

### 主題：一個簡單的音樂評分模型


## 簡介

本專案訓練了一個音樂評分模型，它會評斷出一段有「嚴重錯誤」的樂譜（如，結構割裂、跑調、有雜音），並基於這個模型設計了一個簡單的音樂生成模型。\
詳情見 `report.md`


## 文件

- 主程式：`./src/finalProject.ipynb`
- 音樂生成模型：`./src/music_henerator.ipynb`
- 模型存檔：`./model/best_model.pth`
- 模型成果：`./figure/`
- 原數據：`./data/maestro-v3.0.0/`


## 運行方法

- `finalProject.ipynb`：請嘗試在 colab 上運行，或自行於本地環境上進行修改。如果要使用音樂生成模型，記得下載模型存檔 `best_model.pth`，並在資料夾 `model` 中將原存檔覆蓋掉。
- `music_henerator.ipynb`：本地即可運行，請確保你的環境安裝了相關的庫，具體需要的庫請見源碼。生成的音樂會自動保存到 `figure` 資料夾。


## 結果展示

可以看出，對於一個出現局部跑調的樂譜，我們的模型堅定不移地給出了低分。
![test_offKey](./figure/test_offKey.png)


## 資料來源

資料取自網絡上的免費開放數據集：MAESTRO v3.0.0 \
鏈接：https://magenta.withgoogle.com/datasets/maestro

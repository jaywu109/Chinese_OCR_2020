# Chinese_OCR_2020
T-Brain 繁體中文手寫影像辨識 OCR 競賽   
將目標 formulate 為***影像分類以***及 ***Out-of-Distribution/Open Set*** 辨識問題。    
針對影像分類問題採用 Pre-trained 模型搭配對抗式網路架構用以減少不同書寫 風格造成分類上的困難；針對 OOD 問題則採用 Temperature Scaling 機制與 Outlier Exposure 方法設法使模型能分辨出從未出現在訓練集中的資料。在將模型利用 Flask 部屬在 Server 後獲得 **F1-Score 0.87** 的結果

---
Soving Chinese OCR problem by formulating it to classic image classification problem and Out-of-Distribution problem.  
''Energy-based Out-of-distribution Detection'' is adopted to differentiate the image that has never appeared in training set.

## Method of Energy Score
![image](https://user-images.githubusercontent.com/36630295/125031595-73bbe080-e0bf-11eb-9c9c-f4351e7b648e.png)

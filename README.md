# Data-Analysis

## HW1 Introduction: 

資料集 : Titanic - Machine Learning from Disaster (https://www.kaggle.com/c/titanic/overview)  
預測目標 : 乘客生還與否

1. 進行資料分析與前處理
 - 資料視覺化
   - 不同性別死亡率比較
   - 不同Class死亡率比較 
   - 相關係數圖
 - 填補缺失值
 - 轉換數值資料
   - 利用區間將 Fare 和 Age 做分群
 - 轉換類別資料(Sex、Embarked)
 - 新增欄位 FamilySize(家人數目(包括自己)) 和 Alone(家人數目為1則表示為單獨)
 - 去掉不必要的欄位(e.g.,Name)

2. 模型訓練
 - 分別選擇使用 Decision Tree、SVC、XGBClassifier 進行訓練
 - ensemble 模型選擇使用 RandomForestClassifier 進行訓練
3. 將模型套用至 test.csv 進行預測後上傳到 Kaggle 上評分
 - 預測準確度(accuracy) : 78.947 %
 - Kaggle Public Leaderboard : 約 9.9 % (2021/4/26)
 <img src="https://i.imgur.com/meoxDOe.png" alt="alt text" width="510" height="200">

## HW2 Introduction: 

資料集 : Boston House Prices (https://www.kaggle.com/vikrishnan/boston-house-prices)  
預測目標 : 預測房價

1. 利用 Seaborn 畫箱型圖，觀察每一個 features 的數值分佈
2. 利用 Seaborn 進行 Heatmap 作圖，觀察每一個特徵與房價 (MEDV) 的關聯程度
3. 挑選出與房價關聯性較高的特徵形成新的 dataframe
4. 針對挑選出的特徵與房價畫成散佈圖觀察
5. 切分資料後進行訓練(使用 Linear Regression、 Random Forest Regressor、XGBRegressor 模型)
6. 利用 Grid search 找出最佳參數
7. My Score :
 - R2: 0.9235766423321546
 - Test loss (MSE): 7.631333638672149

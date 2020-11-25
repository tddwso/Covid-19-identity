# Covid-19-identity
## 背景介紹:
建構能分辨是否感染covid-19的AI辨識模型
## 預計完成目標:
以卷積神經網絡(Convolutional Neural Network)學習分辨OK及NG品。
運用Transfer Learning(遷移式學習)，將他人訓練好的(pre-trained model)參數複製過來，當作我們模型參數，
使用的模型: VGG16、Nasnet、Resnet50、Xception
## 資料集:
Train Data : 50
## 使用環境:
Python 3.8

TensorFlow 2.3.1 
## 訓練和測試結果
結果為VGG16最佳，模型訓練準確度100%
 
Xception最佳的訓練模型準確率(accuracy): 80%

Resnet50最佳的訓練模型準確率(accuracy): 60%

Nasnet最佳的訓練模型準確率(accuracy): 60%
 

![image](https://github.com/tddwso/Covid-19-identity/blob/main/ACC.PNG)

ROC曲線 (Receiver operating characteristic curve) & AUC (Area Under Curve)

ROC曲線會以對角線為基準，曲線下的面積(AUC)來判別ROC曲線的鑑別力，AUC數值的範圍從0到1，數值愈大，代表模型的鑑別力越好。

![image](https://github.com/tddwso/Covid-19-identity/blob/main/ROC.PNG)

實際測試結果

![image](https://github.com/tddwso/Covid-19-identity/blob/main/test.PNG)

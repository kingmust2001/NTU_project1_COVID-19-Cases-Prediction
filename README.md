# NTU_project1_COVID-19-Cases-Prediction

## 專案介紹
Given survey results in the past 3 days in a specific state in U.S., then predict the percentage of new tested positive cases in the 3rd day.

Conducted surveys via facebook (every day & every state)

Survey: symptoms, COVID-19 testing, social distancing, mental health, demographics, economic effects, ...

![image](https://user-images.githubusercontent.com/77257138/148672365-0cf33013-f441-43bb-a35c-c185efda76ee.png)
![image](https://user-images.githubusercontent.com/77257138/148672380-f9ec68d6-3f6c-4578-be73-927ce5cf70d0.png)

## 軟硬體配置
* CPU: Intel(R) Xeon(R) (6-cores)
* GPU: Tesla K80 (11.44GB)
* OS： Window10
* Pytorch: 1.10.0
* keras: 2.7.0
* tensorflow: 2.7.0
* Memory: 12.69GB
## 資料來源
Source: Delphi group @ CMU

A daily survey since April 2020 via facebook.
## 資料基本資訊
training set: 2700 (20% validation)
testing set: 893
![image](https://user-images.githubusercontent.com/77257138/148673292-8fa41a9e-4085-43b2-bf81-3a4ee3974cf1.png)
![image](https://user-images.githubusercontent.com/77257138/148673377-b3f74719-928d-4043-86a4-0e04bf84d7c1.png)

## 前處理
feature standardization ((sample-mean)/std)
## 模型
stack two fully connected network
## Metrics
Root mean square error (RMSE)
![image](https://user-images.githubusercontent.com/77257138/148673339-43a67bb5-b192-4988-832c-688ea227897b.png)
## 成果
training loss: 0.8682

validation loss: 3.1614 

![image](https://user-images.githubusercontent.com/77257138/148673527-c7d41744-417c-4db8-ab5d-d210fc465f8f.png)
## Reference
https://speech.ee.ntu.edu.tw/~hylee/ml/2021-spring.html

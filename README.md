# base_TCN_emotion_recognition
## 1、数据预处理及特征提取
`DEAP`数据集是由英国伦敦玛丽皇后大学的研究人员通过实验开发的一个用于分析人类情感状态的多模态数据集，<br>
记录了32个被试者的生理信号（脑电信号、眼电信号、肌电信号和皮肤电信号）和面部表情。<br>
通过小波包分析方法分解出脑电信号的各个频段，通过设置验证集分别得出不同频段的识别精度以及总的识别精度，探讨脑电信号的频段与情感的联系。<br>
选取最好的频段，提取小波系数的能量值作为模型的输入特征。<br>
## 2、主程序
该实验是通过`keras`框架编写的TCN网络，`model_ensemble.py`用来对实验模型进行集成

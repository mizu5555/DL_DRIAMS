# DL_DRIAMS
2024 Fall NCU  Introduction to Deep Learning class's final project

Dataset ：[DRIAMS - 抗生素抗藥性](https://www.kaggle.com/datasets/drscarlat/driams/codehttps://www.kaggle.com/datasets/drscarlat/driams/code)

ppt ： [Final Project Presentation - DRIAMS](https://docs.google.com/presentation/d/1C0Y9o0IngL1HkrAskizLj9HDPhQHzfP4xMjeHphG_4k/edit#slide=id.g323f05ea976_6_756)

## 操作
1. Kaggle下載資料集
2. final_group1.ipynb打開就可以跑 (原先有先做預處理的文件，但每個都GB等級，上傳不了)

## Dataset introduction
### Data type

* binned_6000：分箱後的數據，6000 維特徵
    * bin_index：表示質量電荷比(m/z)的分箱索引，代表質量電荷比的一個區間(例如3Da)。
    * binned_intensity：表示該分箱中信號強度的聚合值。

### Analyze goals

- 二元分類問題：判斷此細菌是否為金黃色葡萄球菌(Staphylococcus aureus)
    - 大腸桿菌(Escherichia coli) 0
    - 糞腸球菌(Enterococcus faecalis) 0
    - 肺炎克雷伯氏菌(Klebsiella pneumoniae) 0 

    - 綠膿桿菌(Pseudomonas aeruginosa) 0
    - 金黃色葡萄球菌(Staphylococcus aureus) 1

對SA做mRMR篩選出很多個關鍵區間，再對另外四個取相同區間

### Result
- For DRAIMS-A
![image](https://github.com/user-attachments/assets/b38c2d55-b339-4b38-a2fe-f99e506d8fda)

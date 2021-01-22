## How to evaluate feature importance and select feature ?

Why do we need to care about it ? 
 
Simple model Vs black-box model

## How to evaluate model feature importance for black-box ML models

A classical method to measure the importance of an attribute is to calculate the loss of accuracy of classification caused by the random permutation of attribute values between objects. However,we need to decide whether the importance of any given attribute is significant, that is, whether it
is discernible from importance which may arise from random fluctuations. To be specific, categorical variables and related variables can inflate the variable importance value. Several methods have been developed to build an distribusion of the variable importance value, so that the significant level of attributes can be calculated. 

- Permutation methods: Calculate score change after removing feature
  Cons: requires re-train model, which is not effective 
 
- Replace feature with random noise and then calculate score change based on trained model

[Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)  
Paper evaluate variable importance by permutating dependent variable <img src="https://latex.codecogs.com/gif.latex?\dpi{150}&space;\small&space;y_{i}" title="\small y_{i}" /></a>
.P-value can also be caculated through permutation test. Also check this [Kaggle post](https://www.kaggle.com/ogrellier/feature-selection-with-null-importances)

[Feature Selection with the Boruta Package](https://www.jstatsoft.org/article/view/v036i11)  Miron B. Kursa, Witold R. Rudnicki  
[Boruta for those in a hurry](https://cran.r-project.org/web/packages/Boruta/vignettes/inahurry.pdf)

[Interpretable Machine Learning - A Guide for Making Black Box Models Explainable](https://christophm.github.io/interpretable-ml-book/feature-importance.html)
This book gives good example

[Please Stop Permuting Features - An Explanation and Alternatives](https://arxiv.org/pdf/1905.03151.pdf)  
Paper provide a good overview of existing feature importance measurment methods. It also explains why correlated variable will inflate misleading results. 

[Bias in random forest variable importance measures: Illustrations,sources and a solution](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-8-25).
Paper shows CRT based RF will favor attributes with more cut-off points. 

https://zhuanlan.zhihu.com/p/144553342

[Definitions, methods, and applications in interpretable
machine learning](https://www.pnas.org/content/116/44/22071)
Bin Yu
High level overview

[All Models are Wrong, but Many are Useful: Learning a
Variable’s Importance by Studying an Entire Class of
Prediction Models Simultaneously](https://arxiv.org/pdf/1801.01489.pdf)  


[大数据：“人工特征工程+线性模型”的尽头](https://cloud.tencent.com/developer/article/1060878)

[Tunability: Importance of Hyperparameters of Machine
Learning Algorithms](https://www.jmlr.org/papers/volume20/18-444/18-444.pdf)

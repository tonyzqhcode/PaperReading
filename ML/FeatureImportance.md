## How to evaluate model feature importance for black-box ML models
- Calculate score change after removing feature
  Cons: requires re-train model, which is not effective 
 
- Replace feature with random noise and then calculate score change based on trained model



[Please Stop Permuting Features - An Explanation and Alternatives](https://arxiv.org/pdf/1905.03151.pdf)  
Paper provide a good overview of existing feature importance measurment methods. It also explains why correlated variable will inflate misleading results. 

[Bias in random forest variable importance measures: Illustrations,sources and a solution](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-8-25).
Paper shows CRT based RF will favor attributes with more cut-off points. 

[Permutation importance: a corrected feature importance measure](https://academic.oup.com/bioinformatics/article/26/10/1340/193348)  
Paper evaluate variable importance by permutating dependent variable <img src="https://latex.codecogs.com/gif.latex?\dpi{150}&space;\small&space;y_{i}" title="\small y_{i}" /></a>
.P-value can also be caculated through permutation test

[Interpretable Machine Learning - A Guide for Making Black Box Models Explainable](https://christophm.github.io/interpretable-ml-book/feature-importance.html)
This book gives good example

[All Models are Wrong, but Many are Useful: Learning a Variable's Importance by Studying an Entire Class of Prediction Models Simultaneously](https://arxiv.org/pdf/1801.01489.pdf)

https://zhuanlan.zhihu.com/p/144553342

[Definitions, methods, and applications in interpretable
machine learning](https://www.pnas.org/content/116/44/22071)
Bin Yu
High level overview

[All Models are Wrong, but Many are Useful: Learning a
Variable’s Importance by Studying an Entire Class of
Prediction Models Simultaneously](https://arxiv.org/pdf/1801.01489.pdf)

[Tunability: Importance of Hyperparameters of Machine
Learning Algorithms](https://www.jmlr.org/papers/volume20/18-444/18-444.pdf)

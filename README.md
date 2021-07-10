# Covid-19-classification

Dataset 1: https://www.kaggle.com/pranjallk1995/covid-xrays

Task is to classfy thoracic X-ray images into three categories. We have used CNNs and transfer learning for this purpose. Transfer learning has been an important step in the feature extraction process. This was required because to extract the features two CNNs have been used (VGG16 and VGG19). Since these are complex neural architectures that require large datasets to train them. The dataset used for our purposes only consists of 950 files. Therefore, the CNNs were used with weights of their training on ImageNet dataset. 

After the feature extraction process, three methods were used to perform classification: Decision trees, Softmax Regression, and SVMs. 


Results:

The first dataset was found to have discrepancy between test and training sets. For this reason, another dataset was used. 
The accuracies are shown below:

| Accuracy | | | |
|------------|----|-----|----|
| Classifier | Train | Val | Test |
|------------|-------|-----|------|
| Decision Tree | 90 | 71 | 71 |
| VGG16 + Softmax | 100 | 83 | 3 |
| VGG19 + Softmax | 100 | 82 | 5 |
| PCA + SVM | 92 | 84 | 4|


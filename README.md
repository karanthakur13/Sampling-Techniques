# Sampling Techniques for creating a balanced dataset for a machine learning model

## Introduction

There are various sampling techniques used in machine learning to select training, validation, and testing data sets. Here are five commonly used sampling techniques:

The following five sampling techniques were used in this project:

1. **Simple Random Sampling:** A basic sampling technique where each data point in the dataset has an equal probability of being selected in the sample.

2. **Stratified Sampling:** A sampling technique where the population is divided into subgroups (strata) based on a specific characteristic, and samples are taken from each stratum in proportion to the population.

3. **Systematic Sampling:** A sampling technique where every nth element in the population is selected for the sample, with n being a fixed interval.

4. **Cluster Sampling:** A sampling technique where the population is divided into clusters, and a sample of clusters is randomly selected. Then, all members of the selected clusters are included in the sample.

5. **Multi Stage Sampling:** In multi-stage clustering sampling, the population is divided into larger clusters, such as cities or states, which are then divided into smaller clusters, such as neighborhoods or census tracts.

## Comparison Table

The table below shows the accuracies of each sampling technique on five different machine learning models. The dataset used for all models is a balanced version of the original unbalanced dataset using random over-sampling and under-sampling techniques.

|Sampling Technique	| Quadratic Discriminant Analysis	| Random Forest Classifier	| Light Gradient Boosting Machine	| Extra Trees Classifier	| Ada Boost Classifier|
|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|
|Simple Random Sampling |	1	| 0.9963	| 0.9852	| 0.9926	| 0.9815 |
|Stratified Sampling	| 0.9833	| 0.9944 | 0.9944	| 0.9963	| 0.9869 |
|Systematic Sampling	| 0.9981	| 0.9887	| 0.9831	| 0.9944	| 0.9718 |
|Cluster Sampling	| 1	| 1 |	0.9927	| 0.9976	| 0.9927 |
|Multi Stage Sampling |	0.8095	| 0.9571	| 0.9571	| 0.9429	| 0.9286 |

Based on these results, it can be concluded that Cluster Sampling performs the best on all five models. Multi Stage Sampling performs the worst on all five models. The other sampling techniques have varying performance depending on the model. 

## Conclusion

It is recommended to use cluster sampling for this dataset, as it consistently gives the best performance across all models. However, other sampling techniques may be worth considering for different datasets or models.
 

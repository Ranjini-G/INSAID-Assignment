# Gender recognition by voice and speech analysis

![voicepic2](https://github.com/Ranjini-G/INSAID-Assignment/blob/master/Images/voicepic2.jpg "voicepic2")

## Problem Statement

This database was created to __identify a voice as male or female__, based upon acoustic properties of the voice and speech. The dataset consists of recorded voice samples, collected from male and female speakers. The voice samples are pre-processed by acoustic analysis in R using the seewave and tuneR packages, with an analyzed frequency range of 0hz-280hz (human vocal range).

------------

## Data Description

The dataset consists of 3168 samples and 21 features.  

| Column Name  | Description  |
| ------------ | ------------ |
| meanfreq  | mean frequency (in kHz)  |
| sd  | standard deviation of frequency  |
| median  | median frequency (in kHz)  |
| Q25  | first quantile (in kHz)  |
| Q75  | third quantile (in kHz)   |
| IQR  | interquantile range (in kHz)  |
| skew  | skewness (see note in specprop description)  |
| kurt  | kurtosis (see note in specprop description)   |
| sp.ent  | spectral entropy   |
| sfm  | spectral flatness  |
| mode  | mode frequency  |
| centroid  | frequency centroid (see specprop)  |
| peakf  | peak frequency (frequency with highest energy)  |
| meanfun  | average of fundamental frequency measured across acoustic signal  |
| minfun  | minimum fundamental frequency measured across acoustic signal  |
| maxfun  | maximum fundamental frequency measured across acoustic signal  |
| meandom  | average of dominant frequency measured across acoustic signal  |
| mindom  | minimum of dominant frequency measured across acoustic signal  |
| maxdom  | maximum of dominant frequency measured across acoustic signal  |
| dfrange  | range of dominant frequency measured across acoustic signal  |
| modindx  | modulation index  |
| label  | male or female  |

------------

## Classifier Model

Various classifier models used to predict the gender using the voice dataset.  These models are evaluated on different metrics to know the level of performance.  The results are listed here:

| Algorithm  | Accuracy  |  Precision | Recall  | f1_Score  | AUC_ROC_Score  |
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |
| LogisticRegression  | 0.897476  | 0.858333 | 0.956656  | 0.904832  | 0.896335  |
| DecisionTree  | 0.970032  | 0.984076  | 0.956656  | 0.970173  | 0.970290 |
| RandomForest  | 0.973186  | 0.981132  | 0.965944  | 0.973479  | 0.973326  |
| **KNN**  | 0.974763  | 0.981191  | 0.969040  | 0.975078  | 0.974874  |
| SVM  | 0.960568  | 0.954268  | 0.969040  | 0.961598  | 0.960404  |
| NaiveBayes  | 0.869085  | 0.877358  | 0.863777  | 0.870515  | 0.869188  |

From the above, we observe that **KNN** model has performed well with highest scores in all the metrics.

# Machine-Learning-with-Java
Classification of weather (Windy day (TRUE or FALSE) and Outlook(sunny, cloudy, rainy) through weka.

This Project relies heavily on the weka library for classification purposes so be sure to have it installed to run correctly.
download link if needed http://www.cs.waikato.ac.nz/ml/weka/index.html

# weather.txt

Note that we are using a .txt where weka documentation will say .arff because arff do not work in ides as they are intended 
for weka gui use not inside ides where .txt work fine

This text file includes the @relation, @attributes, and @data fields.

@relation is used somewhat like a title
@attributes list all the features anly with the types of the features
@data is the raw input of these features

Since I gave a simplfied explaination of this here is a link with more details http://www.cs.waikato.ac.nz/ml/weka/arff.html

The weather.txt file consist of weather data from april 2015-2017 which was take from https://www.wunderground.com/history/airport/KFAY/2015/4/21/MonthlyCalendar.html?req_city=Fayetteville&req_state=NC&req_statename=&reqdb.zip=28306&reqdb.magic=15&reqdb.wmo=99999&MR=1

# MachineLearningProject.java

I will not dive into any of the code but give a brief explaination of the output
This is the results of classifying for a windy day

#First 4 are accuracy of 4 different models

Accuracy of J48: 81.93%                                             
---------------------------------
Accuracy of PART: 78.31%                                            
---------------------------------
Accuracy of DecisionTable: 81.93%
---------------------------------
Accuracy of DecisionStump: 81.93%
 ---------------------------------
# Correctly Classified Instances          68               81.9277 %
# Incorrectly Classified Instances        15               18.0723 %
# Kappa statistic                          0     
# Mean absolute error                      0.2966
# Root mean squared error                  0.3857
# Relative absolute error                 98.2441 %
# Root relative squared error             99.9852 %
# Total Number of Instances               83  
 ---------------------------------
#For the confusion matrixhe row indicates the true class, the column indicates the classifier output.
#That is in our case 15 false negatives that were incorrectly marked as false with 68 true negatives correcty classified

# === Confusion Matrix ===

#  a   b   <-- classified as
#  0  15 |  a = TRUE
#  0  68 |  b = FALSE
  
#Note that this program generates two sets of data this being a 2x2 confusion matrix and the other a 3x3

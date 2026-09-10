## Topics learned:
Types of ML. based on presence of human intervention.

## key concepts:
The types of Ml are :
 # i)supervised learning:-
   dataset contains input and output/label.
   ## There are two parts of supervised learning :-
      a)regression:if the output/target column is numerical then its regression.
       for exmaple:-
    (input)     | (output)
| IQ | CGPA | package |
|------|-----|--------|
| 100 | 10 | 50 |
| 50 | 4 | 5 |
| 120 | 10 | 60 |
 # here as the output columns (package) contains numerical values its regression .
     b)classification:-if the output columns contains categorical data the its classification.
     for example:-
     (input)     | (output)
| IQ | CGPA | placement(Y/N) |
|------|-----|--------|
| 100 | 10 | Y|
| 50 | 4 | N|
| 120 | 10 | Y |
----------------------------------------------------------
 # ii)unsupervised learning:-
 here only input is present in data no output/labels.the model finds its strutur in its own .

  for example:-
  (input)     | 
| IQ | CGPA | 
|------|-----|
| 100 | 10 | 
| 50 | 4 |
| 120 | 10 | 
 # only input columns in data
  
  ## the types of unsupervised learning are :-
    a)clustering:- group similar data together wihtout having predefined labels.
    eg:-
| customer | Age | spending |
| -------- | --- | -------- |
| A        | 20 | 10k        |
| B        | 21  | 15k       |
| C        | 50  | 90K      |
| D        | 45 | 80k         |

using clustering algorithm(PCA),
      cluster 1:- young,low spending customers
      cluster 2:-older ,high spending customers

    b)dimensionality reduction:-
     if the dataset contains large number of columns it  it merge and makes new single cloumns form the data of multiple columns .which also  called feature engineering.
    ------------------------------------------------------
    
    c)Anamoly detection:-detects outliers.
    eg:- finding manufacturing defecat and removing them 

    ------------------------------------------------------
    d)Association learning:-arranging similar data in same place .eg :- puting milk and eggs in  same place in supermarkets . also the famous walmart store survey which shows to keep beer and diapers at the same place beacause while buying diapers there is higher probability that the person  also buys beer.
----------------------------------------------------------

 # iii)  semi_supervised learning :-
 mix of little lablled data and lots of unlabelled data.
 
 eg:-google photos grouping face ,that if we label one photo  let say "mom" then it all labels the rest of mom photo and make collection containg those photos where mom is present.
 -------------------------------------------------------- 
 # iv)Reinforcement leaning:-
 agent learns by taking actioins in and environment and  geting rewards/penalties ,here are no fixed datasetsat all.the agent leanrns by prcatice /mistakes.

 eg: robotics/self driving cars
 
## Tomorrow:-
types of ml ny how the model learns over times (batch /online learning ) 
Project Name - Mercedes-Benz Greener Manufacturing  

DESCRIPTION  

Reduce the time a Mercedes-Benz spends on the test bench.  

**Problem Statement Scenario:** 
Since the first automobile, the Benz Patent Motor Car in 1886, Mercedes-Benz has stood for important automotive innovations.  
These include the passenger safety cell with the crumple zone, the airbag, and intelligent assistance systems. Mercedes-Benz applies for nearly 2000 patents per year,  
making the brand the European leader among premium carmakers. Mercedes-Benz cars are leaders in the premium car industry.  
With a huge selection of features and options, customers can choose the customized Mercedes-Benz of their dreams.  

To ensure the safety and reliability of every unique car configuration before they hit the road, Daimler's engineers have developed a robust testing system.  
As one of the world's biggest manufacturers of premium cars, safety and efficiency are paramount on Daimler's production lines.  
However, optimizing the speed of their testing system for many possible feature combinations is complex and time-consuming without a powerful algorithmic approach.  

You are required to reduce the time that cars spend on the test bench. Others will work with a dataset representing different permutations of features in  
a Mercedes-Benz car to predict the time it takes to pass testing. Optimal algorithms will contribute to faster testing, resulting in lower carbon dioxide  
emissions without reducing Daimler's standards.  

**Following actions should be performed:**  

-If for any column(s), the variance is equal to zero, then you need to remove those variable(s).  
-Check for null and unique values for test and train sets.  
-Apply label encoder.  
-Perform dimensionality reduction.  
-Predict your test_df values using xgboost.  

[Please follow this URL to my proposed solution](https://github.com/samuel-ntsua/Machine_Learning_with_Python/blob/b8cca00c8289dc373d1b0619b8238738c9a392e9/Machine_Learning_Project_mercedes_sntsua.ipynb)  

```Python pandas
## We can get the dataset directly from github <br>
## We just need the path to the raw data location. To do that, we add ""?raw=true" to the url link.
import pandas as pd

train_path ="https://github.com/Simplilearn-Edu/Machine-Learning--Projects/blob/master/Projects/Projects%20for%20Submission/Project%201%20-%20Mercedes-Benz%20Greener%20Manufacturing/Dataset%20for%20the%20project/train.zip?raw=true"
test_path ="https://github.com/Simplilearn-Edu/Machine-Learning--Projects/blob/master/Projects/Projects%20for%20Submission/Project%201%20-%20Mercedes-Benz%20Greener%20Manufacturing/Dataset%20for%20the%20project/test.zip?raw=true"

## load the dataset

mbtrain_df = pd.read_csv(train_path, compression='zip', header=0, sep=',', quotechar='"')
mbtest_df = pd.read_csv(test_path, compression='zip', header=0, sep=',', quotechar='"')

```


Background of Problem Statement:  

IBM HR Analytics Employee Attrition Modeling.  
DESCRIPTION  
IBM is an American MNC operating in around 170 countries with major business vertical as computing, software, and hardware.  
Attrition is a major risk to service-providing organizations where trained and experienced people are the assets of the company.  
The organization would like to identify the factors which influence the attrition of employees.  

Data Dictionary  
Age: Age of employee  
Attrition: Employee attrition status  
Department: Department of work  
DistanceFromHome  
Education: 1-Below College; 2- College; 3-Bachelor; 4-Master; 5-Doctor;  
EducationField  
EnvironmentSatisfaction: 1-Low; 2-Medium; 3-High; 4-Very High;  
JobSatisfaction: 1-Low; 2-Medium; 3-High; 4-Very High;  
MaritalStatus  
MonthlyIncome  
NumCompaniesWorked: Number of companies worked prior to IBM  
WorkLifeBalance: 1-Bad; 2-Good; 3-Better; 4-Best;  
YearsAtCompany: Current years of service in IBM  

Analysis Task:  

Exploratory data analysis  
Find the age distribution of employees in IBM  
Explore attrition by age  
Explore data for Left employees  
Find out the distribution of employees by the education field  
Give a bar chart for the number of married and unmarried employees  
Build up a logistic regression model to predict which employees are likely to attrite.  

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

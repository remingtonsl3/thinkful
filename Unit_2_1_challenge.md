# Challenge: Preparing a dataset

Data: IBM HR Analytics Employee Attrition and Performance data data

Outcome Variable: I am attempting to find model to predict attrition.

These are the variables I will be using: 

* Attrition (Outcome variable, categorical)
* Age (continuous, ratio)
* MonthlyIncome (continuous, ratio)
* JobSatisfaction (outcome variable) (continuous, ord)
* TotalWorkingYears (continuous, ratio)
* JobRole (categorical)
* YearsWithCurrManager (continuous, ratio)
* DistanceFromHome (continuous, ratio)


#Possible features:

1. InSales: Sales job role/Non-sales Job role.
The Sales roles seem to vary differently from the non-sales jobs in attrition.

2. Biome: Life Sciences and Medical/Other Education
Those that come in with medical and life science education appear to differ from other academic areas

3. SecondaryDegree: HasDegree/NoDegree
Whether people have completed college may relate to their attrition

4. InResearch: Research/OtherDepartment
The Research and Development jobs seem to discourage attrition.

5. OverForty: Age>40/Age<40
Looking at the data indicates this is a cutoff that shows some clear differences

6. TenK: Monthly Income over/under $10000

7. MYTA
The values for 'MonthlyIncome','YearsWithCurrManager','TotalWorkingYears', 'Age' seem to be colinear. I combined them into one feature.

8. Normalized Monthly Income
The monthly income is weighted heavily to the lower end. The log values are much more normal.

9. Putting values on the same scale. 
Some of these values share a similar scale, but most do not, e.g., Age and MonthlyIncome. In order to compare these, I scaled all the numerical values to give them a mean of zero and a standard deviation of 1.

10. Distance/Working Years relationship
I wanted to create a non-linear feature, so I looked at the relationship between DistanceFromHome and TotalWorkingYears.




*Other Variables*

* JobInvolvement (continuous, ord)
* JobLevel (continuous, ord)
* TrainingTimesLastYear (continuous, ratio)

* Education (continuous, ord)
* PerformanceRating (continuous, ord)
* PercentSalaryHike (continuous, ratio)
* BusinessTravel (categorical)
* Department (categorical)
* EducationField (categorical)
* Gender (categorical)



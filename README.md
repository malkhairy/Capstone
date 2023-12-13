# Capstone

## The research question:

The objective of this research is to forecast adherence among individuals diagnosed with Type 2 Diabetes and/or Heart failure. This will be achieved by constructing a predictive model utilizing electronic medical records.

This is a retrospective observational study conducted between January 1,2020, to April 30, 2021, of adult patients 18 years and older with Diabeties or heart failure. Patients who had a minimum of 1 insurance claim within the study period and prescribed or were taking any of the following canagliflozin, dapagliflozin, empagliflozin, ertugliflozin, as monotherapy or in a combination drug formulation were included.


## Data 
Data was collected and deindetified from medical institution - IRB approved

Data collected included age, gender, race/ethnicity, diagnosis, medication, copay, laboratory values and insurance plan payment from the electronic health record (EHR). Duplicate data entries and irrelevant insurance claims were removed. 

The primary outcome for measuring adherence amongst study subjects was the proportion of days covered (PDC) based on pharmacy insurance claims. The PDC is used to estimate medication adherence by calculating the proportion of days in which a patient has access to the medication, over a given period of interest. PDC was calculated over the study period defined as the period of interest:

PDC = number of days covered by the pharmacy-supplied medication / number of days a medication is needed

PDC was treated as a binomial variable with a cut point of ≥ 0.8 to divide the cohort into two groups: high (≥ 0.8) and low (<0.8) adherence groups



## Techniques
Following technicques were used:
    1- EDA
    2- Feature engineering to prepare data.
    3- Various Regression and Classifier algorithms such as:
          -Knearest Neighbor
          -Decision Tree
          -Logistic Regression
          -SVM

We used accuaracy for training and test sets as evaluation metrics and ROC curves


## Results
Among all the tested predictive models, tree model had the highest accuracy and area under the curve (AUC) compared to KNN, Logistic Regression, and SVC models (accuracy = 82%).

Following table summarizes the result of accuracy:

<img width="242" alt="image" src="https://github.com/malkhairy/Capstone/assets/138996938/6ec7ea09-b48e-4de4-b216-ddcdc6e86d11">

ROC graph is shown here: 

![image](https://github.com/malkhairy/Capstone/assets/138996938/01466ca4-983b-425e-a266-1f368fb11fb0)

In conclusion, we found that HbA1c, age, gender and payor plan payments are important predictors of medication adherence for diabetes care. Using these variables, the community pharmacist can identify patients at risk and design comprehensive medication management programs to improve adherence and diabetes outcomes. . Higher adherence will reduce comorbidities, decrease hospitalizations, and reduce overall healthcare costs specifically in chronic conditions, including diabetes mellitus, and heart failure. Thus, a predictive analytics approach could be used to demonstrate how event-based data can form the basis for identifying patients who are at risk for future non-adherence and, consequently, more complications


Full analysis can be found @: https://github.com/malkhairy/Capstone/blob/dcecd75d7246c281dfff4033f45381413258e8f5/Capstone_Analysis.ipynb

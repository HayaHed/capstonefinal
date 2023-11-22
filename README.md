# Capstone Project : Cancer Predictive Model

## Part 1: Introduction
Cancer diagnosis and risk prediction remains a significant public health challenge globally, representing a complex interplay of genetic, environmental, and behavioral factors. One of the key challenges in healthcare is the early and accurate diagnosis of various diseases, which is essential for improving patient outcomes and reducing healthcare costs. The opportunity my project could address is developing machine learning solutions that can aid in the early detection and prediction of cancer. The project predicts the risk of cancer presence or absence. Therefore , enabling timely interventions and personalized treatment plans. 

## Part 2: The User

The users who experience these problems are healthcare professionals such as doctors and genetic counsellors, patients, radiologists and healthcare systems. Healthcare professionals would benefit from improved risk prediction tools that can assist in making more accurate and early diagnoses and therefore performing further analysis as required. Patients would benefit from early cancer detection, leading to better treatment outcomes. Healthcare systems would benefit from reduced costs associated with late-stage disease treatments. 

## Part 3: Machine Learning and Cancer Prediction

Machine learning can bring significant solutions to cancer prediction by leveraging its ability to analyze and learn from large datasets, identify patterns, and make predictions.It can assess a person's risk of developing lung cancer by considering various factors, including their medical history (chronic diseases and allergies), genetic profile, and lifestyle choices.Specifically, it can assess the risk associated with predominant risk factors like  age,chronic diseases , being overweight or obese , and poor health condition. Predictive models can help identify individuals who may benefit from early screening or lifestyle interventions. Overall , different variables can be analyzed using machine learning algorithms to identify patterns and correlations, the predictive model can provide assessment of a patient's risk of developing cancer.

## Part 4: The Impact

The impact of improving disease diagnosis and prediction using machine learning is substantial.Cancer typically takes several years to manifest symptoms, and once it does, the progression will be fast and painful.Therefore, early detection can lead to more effective treatments, potentially saving lives and improving the quality of life for patients. Moreover, it can significantly reduce healthcare costs by shifting the focus from late-stage, expensive treatments to cost-effective preventive and early intervention strategies. The scale of the problem is vast, with millions of lives affected, trillions of dollars spent on healthcare worldwide, and significant time and resources allocated to treating advanced diseases. 

## Part 5: Cancer prediction Dataset

We've condensed our dataset from 438,693 rows and 303 columns down to just 18 columns. These specific columns were identified as the most critical features following our exploratory data analysis (EDA).

|Features|Description|Values| 
|-----|:-----|:-----|
|_RFHLTH|Adults with good or better health|1:Good or Better Health, 2:Fair or Poor Health, 9:Don’t know/Not Sure Or Refused/Missing 
|SEXVAR|Sex of Respondent|1:Male, 2:Female|
| TOLDHI3 |High cholesterol levels|1:Yes, 2:No , 7:Don’t know/Not Sure Or Refused/Missing| 
| CHECKUP1 |About how long has it been since a person visited a doctor for a routine checkup|1:within past year, 2:Within past 2 years, 3:Within past 5 years ,4: 5 or more years ago , 7:Don’t know/Not sure, 8:Never , 9:Refused  |
| CHCCOPD3 |A person had C.O.P.D. (chronic obstructive pulmonary disease), emphysema or chronic bronchitis|1:Yes, 2:No , 7:Don’t know/Not Sure, 9: Refused  |
| HAVARTH5 | A person had some form of arthritis, rheumatoid arthritis, gout, lupus, or fibromyalgia|1:Yes, 2:No , 7:Don’t know/Not Sure, 9: Refused  |
 | DIABETE4 | A person had diabetes|1:Yes, 2:Yes, but female told only during pregnancy , 3:No , 4:No, pre-diabetes or borderline diabetes, 7:Don’t know/Not Sure, 9: Refused  |
| _RFHYPE6  | Adults who have been told they have high blood pressure|1:No, 2:Yes, 9:Don’t know/Not Sure/Refused/Missing|
| _PHYS14D |  3 level not good physical health status: 0 days, 1-13 days, 14-30 days|1:Zero days when physical health not good, 2:(1-13) days when physical health not good, 3:(14+) days when physical health not good , 9:Don’t know/Not Sure/Refused/Missing|
|_AGE_G | Six-level imputed age category|1:Age 18 to 24, 2:Age 25 to 34, 3: Age 35 to 44  , 4:Age 45 to 54 , 5:Age 55 to 64 , 6:Age 65 or older|
|_IMPRACE | Imputed race/ethnicity value|1: White, Non-Hispanic, 2: Black, Non-Hispanic, 3: Asian, Non-Hispanic,4:American Indian/Alaskan Native, Non-Hispanic, 5:Hispanic, 6:Other race, Non-Hispanic   |
|_RFBMI5 | Adults who have a body mass index greater than 25.00 (Overweight or Obese) |1:No , 2:Yes, 9:Don’t know/Refused/Missing |
|_SMOKER3 | Four-level smoker status: Everyday smoker, Someday smoker, Former smoker, Non-smoker |1:Current smoker, 2:Current smoker, 3:Former smoker , 4:Never smoked, 9:Don’t know/Refused/Missing |
|_RFDRHV7 | Heavy drinkers (adult men having more than 14 drinks per week and adult women having more than 7 drinks per week)  |1:No , 2:Yes, 9:Don’t know/Refused/Missing |
|_TOTINDA | Adults who reported doing physical activity or exercise during the past 30 days other than their regular job  |1:Had physical activity or exercise, 2:No physical activity or exercise in last 30 days, 9:Don’t know/Refused/Missing |
|CHCKDNY2 |kidney disease presence|1:Yes, 2:No , 7:Don’t know / Not sure , 9:refused |
|_FRTLT1A |Consume Fruit 1 or more times per day|1:Consumed fruit one or more times per day, 2:Consumed fruit < one time per day , 9:Don´t know, refused or missing values |
|Cancer |Risk of presence or absence of Cancer|1:Presence of Cancer ,0:Absence of Cancer |

## Part 6: Data Cleaning & Exploratory Data Analysis

In this project, during data cleaning, we processed 438,693 rows and 303 columns, handling missing values, outliers, and inconsistencies. We performed transformations, removals, and imputations to refine the dataset, resulting in a focused set of 18 crucial features for analysis. Moreover , we explored the intricate relationship between diverse demographic and health-related categorical variables and the occurrence of cancer using the Behavioral Risk Factor Surveillance System (BRFSS) dataset. Through an exploratory data analysis (EDA) on this dataset, we comprehensively examined categorical factors such as health checkup frequencies, chronic health conditions, lifestyle habits, and demographic characteristics. The EDA process allowed us to gain initial insights into the distributions, correlations, and potential associations among these variables concerning the presence or absence of cancer. Employing both chi-square tests for association and Cramér's V measurement, our investigation seeks to unearth statistically significant correlations between these variables and the presence or absence of cancer. Understanding these associations can provide valuable insights into the nuanced interplay of these factors, offering a basis for targeted interventions and risk assessment strategies in cancer prevention and management. Here are some key observations from the EDA:

- Each predictor displays a varying weak correlation with our target variable, evaluated by different chi-square statistics to assess their significance.
- Among cancer patients, the majority had a recent routine checkup within the past year (within the last 12 months).This could be explained that those who go for routine checkups might also be more proactive about their health, leading to earlier cancer detection. Also , People with preexisting health conditions might be more inclined to go for routine checkups. These conditions might increase the risk of cancer, leading to a higher correlation between checkup frequency and cancer presence.
  
- Females (_SEXVAR_2.0) constitute a higher number within the group of patients diagnosed with cancer. This could be because of lifestyle choices, environmental exposures, or genetic predispositions can influence the likelihood of developing cancer, and these factors might affect females differently than males.
- Individuals diagnosed with cancer commonly experience coexisting conditions such as chronic obstructive pulmonary disease (COPD), emphysema, or chronic bronchitis. Arthritis, including rheumatoid arthritis, gout, lupus, or fibromyalgia, is also frequently reported among cancer patients.
  
- Patients reporting fair or poor health conditions exhibit a higher risk of developing cancer.
- A notable proportion of cancer patients have reported high cholesterol levels.
- _RFBMI5_1.0 has a very low chi-square statistic of approximately 0.0183, along with a high p-value of 0.8925. This suggests a lack of statistically significant association between this BMI category and the presence or absence of cancer.
- DIABETE4_7.0 demonstrates a notably higher p-value (0.71), signifying a lack of statistically significant association between this particular variable and the incidence of cancer in this dataset.
- Diabetes and high blood pressure prevail among those diagnosed with cancer. Additionally, individuals with cancer often report experiencing more than 14 days of compromised physical health.
- There is a higher association between older age groups and cancer presence.The longer exposure to risk factors and a potentially compromised immune system in older individuals could further contribute to the elevated prevalence of cancer within these age groups.
- Individuals of White, Non-Hispanic ethnicity are notably overrepresented among those diagnosed with cancer. This may be influenced by various factors such as disparities in healthcare access, genetic predispositions, environmental exposures, and socioeconomic factors.
- A significant portion of individuals diagnosed with cancer are overweight or obese.This could be attributed to lifestyle choices, dietary habits, and metabolic factors that contribute to cancer development.
- Former smoking habits were prevalent among individuals diagnosed with cancer, and a majority showed non-heavy drinking behavior. This could reflect past lifestyle choices that have contributed to their health conditions.
- Individuals diagnosed with cancer commonly had kidney disease. Kidney disease and cancer share risk factors such as aging, certain genetic predispositions, lifestyle habits like smoking or poor diet, and exposure to specific environmental toxins or treatments that could affect both conditions.
- '_FRTLT1A_1.0' and '_FRTLT1A_2.0' shows very weak association (Cramér's V ≈ 0.022 ,0.013) with cancer.Consuming a diet abundant in fruits and vegetables is often linked to a reduced risk of specific cancers. However, certain fruits, particularly those high in sugar, might indirectly contribute to weight gain or obesity, potentially increasing the likelihood of developing certain types of cancer.







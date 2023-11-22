# Capstone Project : Cancer Predictive Model

## Part 1: Introduction
Cancer diagnosis and risk prediction remains a significant public health challenge globally, representing a complex interplay of genetic, environmental, and behavioral factors. One of the key challenges in healthcare is the early and accurate diagnosis of various diseases, which is essential for improving patient outcomes and reducing healthcare costs. The opportunity my project could address is developing machine learning solutions that can aid in the early detection and prediction of cancer. The project predicts the risk of cancer presence or absence. Therefore , enabling timely interventions and personalized treatment plans. 

## Part 2: The User

The users who experience these problems are healthcare professionals such as doctors and genetic counsellors, patients, radiologists and healthcare systems. Healthcare professionals would benefit from improved risk prediction tools that can assist in making more accurate and early diagnoses and therefore performing further analysis as required. Patients would benefit from early cancer detection, leading to better treatment outcomes. Healthcare systems would benefit from reduced costs associated with late-stage disease treatments. 

## Part 3: The Big Idea

Machine learning can bring significant solutions to lung cancer prediction by leveraging its ability to analyze and learn from large datasets, identify patterns, and make predictions.It can assess a person's risk of developing lung cancer by considering various factors, including their medical history (chronic diseases and allergies), genetic profile, and lifestyle choices.Specifically, it can assess the risk associated with predominant risk factors like  age,chronic diseases , being overweight or obese , and poor health condition. Predictive models can help identify individuals who may benefit from early screening or lifestyle interventions. Overall , different variables can be analyzed using machine learning algorithms to identify patterns and correlations, the predictive model can provide assessment of a patient's risk of developing cancer.

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



## Part 6: Data Download, Cleaning & Exploratory Data Analysis





The resource for the main dataset: https://www.cdc.gov/brfss/annual_data/annual_2021.html

Useful research article for lung cancer risk level determination: 

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3399915/ 




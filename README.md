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

- _RFHLTH	Adults with good or better health	(1:Good or Better Health, 2:Fair or Poor Health, 9:Don’t know/Not Sure Or Refused/Missing)
- dteday : date
- season : season (1:springer, 2:summer, 3:fall, 4:winter)
- yr : year (0: 2011, 1:2012)
- mnth : month ( 1 to 12)
- hr : hour (0 to 23)
- holiday : whether day is holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
- weekday : day of the week
- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
+ weathersit : 
	- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
	- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
	- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
	- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
- temp : Normalized temperature in Celsius. The values are divided to 41 (max)
- atemp: Normalized feeling temperature in Celsius. The values are divided to 50 (max)
- hum: Normalized humidity. The values are divided to 100 (max)
- windspeed: Normalized wind speed. The values are divided to 67 (max)
- casual: count of casual users
- registered: count of registered users
- cnt: count of total rental bikes including both casual and registered

## Part 6: Data Download, Cleaning & Exploratory Data Analysis


The resource for the main dataset: https://www.cdc.gov/brfss/annual_data/annual_2021.html

Useful research article for lung cancer risk level determination: 

https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3399915/ 




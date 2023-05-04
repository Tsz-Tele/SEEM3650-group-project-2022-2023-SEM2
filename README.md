# SEEM3650-group-project-2022-2023-SEM2
SEEM3650 group project 2022-2023 SEM2



The Minimum Air Temperature is obtained from Hong Kong Observatory with the average of 
Kowloon City minimum air temperature and Wong Tai Sin minimum air temperature. Same as
the Minimum Air Temperature, the Maximum Air Temperature is the mean of Kowloon City
maximum air temperature and Wong Tai Sin maximum air temperature. The Relative Humidity
(%) and Rainfall (mm) are also obtained from the Hong Kong Observatory, both datasets are
from King’s Park. For Weekday, Weekend, Holiday, Day After Holiday, we obtained its
information from the Hong Kong Calendar. The data is represented in 0 and 1, where 0 means
negative, 1 means positive.


The structure of the data for model building (X-axis):

	 Minimum Air Temperature ||	Maximum Air Temperature ||	Relative Humidity (%) ||	Rainfall (mm) ||	Weekday ||	Weekend ||	Holiday ||	Day after holiday


(picture of the table)
![image](https://user-images.githubusercontent.com/102592609/236302458-40ca7aad-4bea-44d5-8716-7876fafd6407.png)

While the No. of A&E first attendances,	total adult patient and	total children patient are the y axis for the model building of total, adult and children patients respectively.

This prediction process is supervised, the total number of patients is obtained from the dataset
Daily Services Statistic. We use No. of A&E first attendances of Kwong Wah Hospital and
Queen Elizabeth Hospital as our total number of patients in Kowloon central cluster. For the
number of adult patients and children patients, we used the number of adult and children bed in
Kwong Wah Hospital and Queen Elizabeth Hospital multiple with the occupancy rate of the
hospital bed.

In the study of the datasets, we have tried to use linear regression, ridge regression and LASSO
to handle the data. The number of patients data in our study represents the total number of
patients that are occupying hospital beds. In the processes, we have divided the data into the total
number of patients, total adult patients, and the total children patients.


 (due date: 5 May, midnight)

References:
Jan Kirenz. Lasso Regression with Python (2021)
https://www.kirenz.com/post/2019-08-12-python-lasso-regression-auto/

Number of Hospital Beds by Specialty and Cluster / Hospital (as at 31 March of respective years) (English)
https://data.gov.hk/en-data/dataset/hospital-hadata-service-ipdp/resource/67f59331-b4e9-4509-a465-9c68b80006b0

Public Hospitals Key Statistics during Service Demand Surge (English)
https://data.gov.hk/en-data/dataset/hospital-hadata-key-statistics-during-surge/resource/f121cbb1-8bc6-4c75-b9b0-afeef197e984

Current Weather Report (English)
https://data.gov.hk/en-data/dataset/hk-hko-rss-current-weather-report/resource/923a02ae-4a14-4a28-8a2b-1215d3dff08f

Department of Paediatrics of Queen Elizabeth Hospital
https://www3.ha.org.hk/qeh/eng/healthcare-professionals/dept/paed/index.htm

Department of Paediatrics, Kwong Wah Hospital
https://www3.ha.org.hk/kwh/main/en/service-introduction.asp?service=pd


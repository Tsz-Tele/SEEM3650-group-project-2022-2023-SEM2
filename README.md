# SEEM3650-group-project-2022-2023-SEM2
SEEM3650 group project 2022-2023 SEM2

-- Background

Although Hong Kong’s healthcare system always achieves better rankings compared to many
countries, it is unavoidable to say that the city’s medical system is at a “boiling point”. Especially
during the peak season, there is a rise in the number of patients looking for treatment for chronic
diseases and flu during persistent cold weather.
When hospitals were so overcrowded that the occupancy rate was over 100 percent. The
occupancy rate on all medical wards in many public hospitals has constantly been around 110
percent, with some as high as 130 percent, meaning temporary beds have even filled up all
spaces in corridors. Besides, the average waiting time for patients at the accident and emergency
departments was more than eight hours. While, some patients criticized that they have to wait for
days in observation units before they could be moved into a room.
We notice that one of the main problems is the insufficient of beds in the hospital. Therefore, we
are interested in doing an investigation on the problem of the lack of beds in the hospital. But for
the result to be more meaningful we decide it to do it focusing on the peak season or the winter
season.

--Dataset

The dataset we use includes the data of Minimum Air Temperature, Maximum Air Temperature,
Relative Humidity (%), Rainfall (mm), whether the day is weekday, weekend , holiday and day
after holiday. The No. of A&E first attendances, total adult patient and total children patient
are also in the data set. Due to the insufficient data, the dataset is ranged from December 2019 
to February 2020, December 2020 to April 2021, December 2021 to April 2022, December 2022 to February 2023.


The Minimum Air Temperature is obtained from Hong Kong Observatory with the average of 
Kowloon City minimum air temperature and Wong Tai Sin minimum air temperature. Same as
the Minimum Air Temperature, the Maximum Air Temperature is the mean of Kowloon City
maximum air temperature and Wong Tai Sin maximum air temperature. The Relative Humidity
(%) and Rainfall (mm) are also obtained from the Hong Kong Observatory, both datasets are
from King’s Park. For Weekday, Weekend, Holiday, Day After Holiday, we obtained its
information from the Hong Kong Calendar. The data is represented in 0 and 1, where 0 means
negative, 1 means positive.

For the patient dataset, we tried to focus on of Kwong Wah Hospital and Queen Elizabeth Hospital, 
which are the major hospitals in Kowloon central cluster.

The No. of A&E first attendances is obtained from the data of Hospital Authority. While the total adult
patient and total children patient are obtained from the calculation on data of occupancy rate of the
hospital beds from Hospital Authority.

Data from Hospital Authority: (Public Hospitals Key Statistics during Service Demand Surge (English) and Number 
of Hospital Beds by Specialty and Cluster / Hospital (as at 31 March of respective years) (English),
also with the hospital bed data from the two hospitals webpage)

The patient_data.csv stores the dataset that we will be used to load the data to the program.

Structure of the patient_data.csv

![image](https://user-images.githubusercontent.com/102592609/236422880-f06c65a6-9221-42a5-b667-de432338cba8.png)




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

mily Tsang and Celine Ge, South China Morning Post (2016), Hong Kong hospital crisis: overcapacity, overworked doctors — and peak flu season will make it worse. https://www.scmp.com/news/hong-kong/health-environment/article/1922697/hong-kong-hospital-crisis-overcapacity-overworked?module=perpetual_scroll_0&pgtype=article&campaign=1922697

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


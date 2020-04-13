# Guide-to-Health (Team Paz)

## 'Guide to Health' project was created for "Code For Venezuela" hackathon by Team Paz.

This project was intended to address the general public and the press for basic health care services in Venezuela. Our team cleaned and translated the data using python (Juypter Notebook), analyzed, created Dashboard for the above specified audience. From our analysis & external research we found that when people are visiting the hospitals, the supplies necessary for their treatment are not available. During emergency, it could be fatal for the patient if there are no supplies. People have no access to data which would help them visit the right hospital according to their preference.

### Data Quality Issues: 
•	The most difficult and time-consuming issue faced in the data was translating the language from Spanish to English (As the team didn’t have any Spanish speakers). 

•	The Google Form had some questions which had checkboxes for answers which allowed the user to input multiple answers where the response was intended to be only one. 

• The data had many missing values. There were some questions on the Google Form which were not mandatory. This could be one of the reasons for multiple missing values. 

•	These forms were filled manually hence this can induce human error or biases in the data collected. 

•	Dropping columns – The columns important for the analysis (The General Public and Press) is only considered. 

•	Unable to clean data row wise – The rows indicated duplicate values, for example the Hospital BOL000 often showed double entries for every reporting week with different values.

### Data Cleaning: 
•	Track 1 was chosen for analysis and the Metrics was chosen carefully to cater to the audience (General Public and Press) 

•	The columns were converted manually from Spanish to English using ‘.replace()’ in Python. 

•	Missing values was filled if there were columns indicating a similarity. For example, columns like Renal replacement therapy availability and Renal replacement therapy operability are similar, where missing values can be filled in one column based on the value in the previous column. 

•	The questions that had a ‘yes’ (‘Si’) or ‘No’ answer was converted to 1 and 0 respectively.

### Data Wrangling: 
•	The metrics important to cater to the audience was identified. These includes the region, hospital code, if the hospital is approachable for an emergency or not, etc. 

•	The hospitals were considered in two different categories such as emergency services and regular services. The metric considered for the analysis is based on the basic requirement a hospital must have such as emergency supplies and ability to perform minor surgeries such as Appendicitis for emergency cases.

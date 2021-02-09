# fraud_detection_on_Insurance_dataset
##Description About the Dataset
     The dataset has 1048575 rows and 24 columns.
>     
      Column                                 Non-Null Count    Dtype  
---  ------                                 --------------    -----  
 0.   Area_Service                           1046119 non-null  object 
 1.   Hospital County                        1046119 non-null  object 
 2.   Hospital Id                            1046119 non-null  float64
 3.   Age                                    1048575 non-null  object 
 4.   Gender                                 1048575 non-null  object 
 5.   Cultural_group                         1048575 non-null  object 
 6.   ethnicity                              1048575 non-null  object 
 7.   Days_spend_hsptl                       1048575 non-null  object 
 8.   Admission_type                         1048575 non-null  object 
 9.   Home or self care,                     1048575 non-null  object 
 10.  ccs_diagnosis_code                     1048575 non-null  int64  
 11.  ccs_procedure_code                     1048575 non-null  int64  
 12.  apr_drg_description                    1048575 non-null  object 
 13.  Code_illness                           1048575 non-null  int64  
 14.  Mortality risk                         1048533 non-null  float64
 15.  Surg_Description                       1048575 non-null  object 
 16.  Weight_baby                            1048575 non-null  int64  
 17.  Abortion                               1048575 non-null  object 
 18.  Emergency dept_yes/No                  1048575 non-null  object 
 19.  Tot_charg                              1048575 non-null  float64
 20.  Tot_cost                               1048575 non-null  float64
 21.  ratio_of_total_costs_to_total_charges  1048575 non-null  float64
 22.  Result                                 1048575 non-null  int64  
 23.  Payment_Typology                       1048575 non-null  int64  
dtypes: float64(5), int64(6), object(13).
>
#missing values and Duplicates in the Dataset
     I have named the dataframe as (fraud_check), there are some missing values in the  dataset to find that we use a [.isnull()](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.isnull.html).
     ```
     fraud_check.isnull().sum()
     ```
* Area_Service                             2456
* Hospital County                          2456
* Hospital Id                              2456
* Age                                         0
* Gender                                      0
*Cultural_group                              0
* ethnicity                                   0
* Days_spend_hsptl                            0
* Admission_type                              0
* Home or self care,                          0
* ccs_diagnosis_code                          0
* ccs_procedure_code                          0
* apr_drg_description                         0
* Code_illness                                0
* Mortality risk                             42
* Surg_Description                            0
* Weight_baby                                 0
* Abortion                                    0
* Emergency dept_yes/No                       0
* Tot_charg                                   0
* Tot_cost                                    0
* ratio_of_total_costs_to_total_charges       0
* Result                                      0
* Payment_Typology                            0

we have missing values on 4 columns __Area_Service__,__Hospital County__,__Hospital Id__,__Mortality risk__ . 
     
     
     

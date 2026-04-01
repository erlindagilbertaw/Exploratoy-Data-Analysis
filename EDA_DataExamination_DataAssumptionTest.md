# Exploratory Data Analysis:<br> Data Examination and Assumption Testing on A Dataset

<table style="text-align:left;">
<tr>
<td style="vertical-align: top; padding-right: 20px;">
  <img src="https://github.com/user-attachments/assets/1311dc05-d9e9-4e77-8042-d84b3be545dd" alt="Foto Erlinda" width="150" style="border:none;"/>
</td>
<td style="vertical-align: top;">
  <h2 style="margin:0; text-align:left; font-size:30px;">By: Ir. Erlinda Gilberta Wibawa, S.T., M.T.</h2>

  <p style="margin:0; text-align:left; font-size:23px;">
    <a href="https://www.instagram.com/erlinda_gilberta/?hl=en" target="_blank">@erlinda_gilberta</a>
  </p>

  <h4 style="margin-top:5px; text-align:left; font-size:23px;">
    <em>Lecturer in Logistics Engineering,<br>
    Universitas Katolik Santo Agustinus Hippo,<br>
    West Kalimantan, Indonesia</em>
  </h4>
</td>
</tr>
</table>

Data is a very valuable asset in making various decisions. However, raw data collected from various sources often cannot be used directly. This can be caused by various constraints that often arise in the data collection process. If used directly without adjusting the feasibility and requirements of certain statistical analysis methods, the data has the potential to produce misleading or inaccurate interpretations. Therefore, a systematic initial process is needed to explore the structure and characteristics of the data before further analysis is carried out. This aims to ensure that the data is in a condition that is suitable for valid and accountable analysis. One approach that is commonly used is Exploratory Data Analysis (EDA).
EDA is the initial stage in data analysis that aims to understand patterns, detect anomalies, and test assumptions through statistical techniques and visualization. In this study, data examination and assumption testing were carried out to identify missing values ​​and outliers from the raw dataset so that it is worthy of further analysis. Without the right examination process, statistical analysis can produce errors and produce invalid interpretations. Furthermore, assumption testing is carried out to ensure that the data meets certain requirements determined by a statistical analysis method. Ignoring assumption testing can lead to errors in decision making and interpretation of results. Data examination and assumption testing are important foundations in statistical data analysis which aim to increase the validity and reliability of analysis results.

This study aims to analyze the importance of data examination and assumption testing in preparing datasets to be statistically feasible. This study is expected to improve the quality of data analysis, so that data-based decision making becomes more accurate and valid.

___
## 1. DATA
This study uses the “HBAT_MISSING” dataset that adopts information from the HATCO Dataset Documentation. The dataset consists of 70 respondents on 14 separate variables. This dataset is used to illustrate the implementation of data examination techniques and assumption tests.


___
## 2. INITIAL NORMALITY TEST
Data examination begins by conducting a Normality Test to determine the normality of quantitative variables. The normality test is carried out using the Kolmogorov-Smirnov method. The Kolmogorov-Smirnov test calculates the level of significance of the difference from the normal distribution. A significance value > significance level indicates that the variable data is normally distributed. Variables V1 to V4 and V6 to V9 have a p-value > alpha, indicating that the variables are normally distributed. In this quantitative data variable, only V5 is not normally distributed (p-value 0.043 < alpha 0.05).
___
## 3. MISSING VALUES
In this case, it is assumed that missing values ​​cannot be ignored because they are known to originate from errors in completing the entire questionnaire.

### **Handling Missing Values**
Missing data can be handled by deleting or filling with a value. If the missing data is relatively small compared to the total data, then deleting incomplete data is one reasonable approach. Variables with at least 15% missing data are candidates for deletion, but higher levels of missing data (20% - 30%) can often be corrected (Hair et al., 2014). As stated by Hair et al., (2014), deletion of missing data is only done if the probability of Missing at Random (MAR) or Missing Completely at Random (MCAR) of the response is independent of the observed/missing data values. If the variables influence each other, then deletion is not the right choice.

<img src="https://private-user-images.githubusercontent.com/85277959/572260476-d626838d-850f-4c50-8a9f-224ff5bc8d0f.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQzNjMsIm5iZiI6MTc3NTAxNDA2MywicGF0aCI6Ii84NTI3Nzk1OS81NzIyNjA0NzYtZDYyNjgzOGQtODUwZi00YzUwLThhOWYtMjI0ZmY1YmM4ZDBmLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMjc0M1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTZhODc5Y2IzNmQxNTMxNGRmMzM4YmVmNTcyMjBhMDU3MDkwZmZhZDlhYjJjYmEzMmY4OTRjNWRmOGM4ZDc4ZWUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.79gd11SZubPGsQLuFk3SVf8N6nZ6wSUgHkRPCjzHne4" width="1000"/>

Missing data can be handled by deleting or filling with a value. If the missing data is relatively small compared to the total data, then deleting incomplete data is one reasonable approach. Variables with at least 15% missing data are candidates for deletion, but higher levels of missing data (20% - 30%) can often be corrected (Hair et al., 2014). As stated by Hair et al., (2014), deletion of missing data is only done if the probability of Missing at Random (MAR) or Missing Completely at Random (MCAR) of the response is independent of the observed/missing data values. If the variables influence each other, then deletion is not the right choice.
___
## 4. NORMALITY TEST
Normality Test can be known from the statistical values ​​for the skewness and kurtosis values. If one of the calculated z values ​​exceeds the specified critical value, then the distribution characteristics are not normal. The critical value comes from the z distribution, based on the specified significance level. The most commonly used critical values ​​are ± 2.58 for a significance level of 0.01 and ± 1.96 for a significance level of 0.05. It can be seen from the 9 quantitative variables, only variables V4 and V9 are normal, the other variables (V1, V2, V3, V5, V6, V7, and V8) show deviations from normality in the Normality Test as a whole.

<img src="https://private-user-images.githubusercontent.com/85277959/572260554-dd111478-59ef-4922-b1ed-eb73dc87c849.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQzODQsIm5iZiI6MTc3NTAxNDA4NCwicGF0aCI6Ii84NTI3Nzk1OS81NzIyNjA1NTQtZGQxMTE0NzgtNTllZi00OTIyLWIxZWQtZWI3M2RjODdjODQ5LmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMjgwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU4MDEyOTJmYzZlYmFiMTQ0NDliMzZkNTNmM2ZkYjM0NGNmYmJmZjQxNjhjYjdjNTc1ZDFkNDQxZTFmY2FmZTgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.syqTNECtbWqaWOwsEccyWkg0ACj2RE76rOfi81pwk0w" width="1000"/>

### **Dealing with Non-normal Data**

Hair et al., (2014) explained that data transformation provides the primary means of correcting for abnormality. Trial error data transformation is done by applying all possible transformations and then selecting the most appropriate transformed variable (Hair et al., 2014). The results of the data transformation will replace the original data from the previous step (handling outliers).
- In V6, there is no transformation that can improve normality, so this variable must be used in its original form.
- In V3, V5, V7, and V8, it can change to increase sharply to a more acceptable level of significance.
- In V1 and V2 there is only a small change in the increase in significance. This can be caused by the number of outliers retained in V1 and V2, thus affecting the distribution of the variables.

<img src="https://private-user-images.githubusercontent.com/85277959/572259870-0308d8f9-90a3-437e-804a-d2ad5080aad2.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQzMjUsIm5iZiI6MTc3NTAxNDAyNSwicGF0aCI6Ii84NTI3Nzk1OS81NzIyNTk4NzAtMDMwOGQ4ZjktOTBhMy00MzdlLTgwNGEtZDJhZDUwODBhYWQyLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMjcwNVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWI1ZmFhMDk1NjJmMjJmOTQ3ODJhOWU4NzJjZWJlYjQwZjczZjczMzU0YWVkYmEzN2Q0MjU5MTg3MjY5M2IxZTgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.-gbvbyFLSx5PrEjyELhnC8AU9ycgQkxHbMDDEnRxwKY" width="1000"/>

___
## 5. OUTLIERS
Outliers are unusual observations that are far from other observations. Outliers are usually treated as abnormal values ​​that can affect the overall observation because of their extreme values ​​that are very high (upper outliers) or low (lower outliers).

### 5.1. Outliers Detection for Univariate Analysis
<img src="https://private-user-images.githubusercontent.com/85277959/572259941-7b89c7ea-78ef-42ae-a980-5960ee6ce740.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQ0MDYsIm5iZiI6MTc3NTAxNDEwNiwicGF0aCI6Ii84NTI3Nzk1OS81NzIyNTk5NDEtN2I4OWM3ZWEtNzhlZi00MmFlLWE5ODAtNTk2MGVlNmNlNzQwLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMjgyNlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWVhNjFmOTE5NjEzYjU3MmE0MGI3NDRjNThiMDgyMDU0ZDZhZTc3MGFkMGJiYjM5MThlMDBhZWRlYTZkYTcxY2MmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.2T0oENitkB7nTKeQt5Pj7WTUsgvSeBrl_6RmB65x4WQ" width="1000"/>

### 5.2. Outliers Detection for Bivariate Analysis

#### 5.2.1. Metric Data V1 – V7 against V9
<img src="https://private-user-images.githubusercontent.com/85277959/572259994-d90df0b0-a4bf-4a59-aa14-68fbf65a34c0.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQ0MjcsIm5iZiI6MTc3NTAxNDEyNywicGF0aCI6Ii84NTI3Nzk1OS81NzIyNTk5OTQtZDkwZGYwYjAtYTRiZi00YTU5LWFhMTQtNjhmYmY2NWEzNGMwLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMjg0N1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTM1NTUxODhlNDEyNDE2NTUzM2U0ZTI5YjQzOWM4NWViODBlNjRkOTc0NDI5NmI5NjRmY2M1ZjQ2YThjYTI1NjgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.DL8WgchFjqix7f5lfGmI_sFEC89s_fwQlZrfy8jIQsI" width="1000"/>

#### 5.2.2. Nonmetric Data V10 – V14 against V9
<img src="https://private-user-images.githubusercontent.com/85277959/572260050-696bab05-0827-4bd9-b75f-586357e3fe86.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQ0NTUsIm5iZiI6MTc3NTAxNDE1NSwicGF0aCI6Ii84NTI3Nzk1OS81NzIyNjAwNTAtNjk2YmFiMDUtMDgyNy00YmQ5LWI3NWYtNTg2MzU3ZTNmZTg2LmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMjkxNVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWE2Y2Q0ODFmZjUzMjg0OTlmZWYwMzQ0NmRjNzFjMTVmMmZkMjE0YmUwNGQzMGQ4ODk3Mzc5MzVjZTk3MjhkOTUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.CvaV5OQcwQX3aoldL_oODrq9kPtKC0v_oWSd2JMbnRk" width="1000"/>

### 5.3. Outliers Detection for Multivariate Analysis
Outliers detection in multivariate analysis is performed on all independent metric variables (Hair, et al., 2014), namely V1, V2, V3, V4, V5, V6, and V7. Outliers detection in multivariate analysis is performed using Mahalanobis D² measurements. The results of the Mahalanobis D² distance are then used to search for the Chi-square probability with the numeric expression of probability transformation in SPSS "1-CDF.CHISQ(MAH_1,7)". The number 7 indicates the degree of freedom that corresponds to the number of variables examined (in this case 7 independent variables). Multivariate outliers will appear if the value of the new probability variable is <0.001 (Statistics Solutions, 2020).

<img src="https://private-user-images.githubusercontent.com/85277959/572260103-6308ad0c-4cb5-4af8-890e-078a247e2ae2.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQ0NzMsIm5iZiI6MTc3NTAxNDE3MywicGF0aCI6Ii84NTI3Nzk1OS81NzIyNjAxMDMtNjMwOGFkMGMtNGNiNS00YWY4LTg5MGUtMDc4YTI0N2UyYWUyLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMjkzM1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWI0NDUzOWQ1YjMxZTA4NDhjOWYyYzY0NGRhM2Q1NTU4N2ViNWQ1YjNlMDhkMjliYzVlNjVmYTc2ZjJlYjIwZjAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.-quaf1IrET5ZD_Wl_-0Efph92Ogo22saaTtExvrIrI8" width="1000"/>

### **Dealing with Outliers**
From 22 cases that have outliers, a decision was made on which cases to delete and which to keep. The decision to keep was made based on the number of cases that appeared more than 1 in the detection of univariate outliers & bivariate outliers. So there were 9 cases that were deleted and 13 cases were kept. 

<img src="https://private-user-images.githubusercontent.com/85277959/572260612-505e77e7-5510-45f8-929d-f5281eec8c29.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQ0OTIsIm5iZiI6MTc3NTAxNDE5MiwicGF0aCI6Ii84NTI3Nzk1OS81NzIyNjA2MTItNTA1ZTc3ZTctNTUxMC00NWY4LTkyOWQtZjUyODFlZWM4YzI5LmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMjk1MlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWQ2ZTg3YzkxYTdlMDkyOTYxODIzOGFkODg2MWEwOTczOWVjZTM2M2VjOGY5YzRkNjdjYjNkZjEzMmQ0OTM2YjgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.5oL-MG43VQ2rL9Uz7JxEHXmQ7L3tPFv97Vj0bwQxxkk" width="1000"/>

___
## 6. HOMOSKEDASTISITAS TEST
Homoscedasticity Test is conducted with Levene Test on the variance mean data whether the variance of a metric variable is the same in a number of groups. In Levene Test, the variance of metric variables is compared across levels of nonmetric variables. Homoscedasticity Test is suitable for the preparation of analysis of variance (ANOVA) or multivariate analysis of variance where nonmetric variables are independent variables. Homoscedasticity Test is also suitable for discriminant analysis where nonmetric variables are dependent measures (Hair, et al., 2014). Levene Test results show that out of 9 metric variables, only V5 shows a heteroscedasticity pattern (p-value <alpha 0.05) in more than one nonmetric variable (V10 and V14). In addition, none of the nonmetric variables have more than one problematic metric variable.

<img src="https://private-user-images.githubusercontent.com/85277959/572260676-d33c3086-14f5-4b27-b8d4-7ed2c0e9416d.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQ1MTIsIm5iZiI6MTc3NTAxNDIxMiwicGF0aCI6Ii84NTI3Nzk1OS81NzIyNjA2NzYtZDMzYzMwODYtMTRmNS00YjI3LWI4ZDQtN2VkMmMwZTk0MTZkLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMzAxMlomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU3MzExYzZhMDA3OWNjZTY4MDBjMjY0MjUwMzdmY2U4NzRjMmE2NDQzOWFiOTFlNWM0NWI0MmU2Njk5YmQ3MDcmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.f1PUOKHBPtiN_69RGRTZZR3WR-55o_J_y_C9F01t7iE" width="1000"/>

### **Dealing with Heteroscedasticity Data**
Heteroscedastic variables can be corrected through data transformations similar to those used in the normality test stage. Most heteroscedasticity is the result of non-normality of one of the variables, and conversely, treating non-normality also corrects unequal variance dispersion. So curing heteroscedasticity will also address the normality issue.

Normal data is not necessarily homogeneous and vice versa. In this case, the variable V5 in the non-normality handling step is normal, but when tested for homogeneity, V5 is heterogeneous with respect to the category variables V10 and V14. To overcome this, the data transformation steps as in the normality handling step are carried out again to overcome the heteroscedasticity problem for V5. After being transformed with a square root, heteroscedastic conditions occur in the nonmetric variables V10, V12, and V14. Levene Test is then re-conducted with adjustment of significance level. Heterogeneous nonmetric variables (V10, V12, and V14) are 0.01, while V11 and V13 use significance level of 0.05. Small significance level in V10, V12, and V14 will increase accuracy to reduce the level of testing error.

<img src="https://private-user-images.githubusercontent.com/85277959/572260733-875d5dcc-af88-4f54-8845-4f8661f15340.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQ1MjksIm5iZiI6MTc3NTAxNDIyOSwicGF0aCI6Ii84NTI3Nzk1OS81NzIyNjA3MzMtODc1ZDVkY2MtYWY4OC00ZjU0LTg4NDUtNGY4NjYxZjE1MzQwLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMzAyOVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTQwMDg1Nzc0NDdhMDFhNzIxOTg5NTUxZmFhODViYjM0MjgzMzI1ZDMxMTQyMjIyMmViNjA5MjkxNWJjNDYxNTgmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.pRt1lXMG1DwRvcki5SkXxySGDPv64ozZ92JBZyXksxQ" width="1000"/>

___
## 7. LINEARITY TEST
Linearity Test is used in bivariate and multivariate analysis to determine whether two or more variables have a significant linear relationship or not. Linearity Test is intended to show that the average obtained from the sample data group lies in straight lines (Jamaluddin & Tommeng, 2018). Linearity test can be done by comparing the significant value (p-value) of Linearity and p-value Deviation from Linearity with the level of significance (alpha). So there are 3 conditions for data linearity assessment criteria. P-value Linearity < alpha and p-value Deviation > alpha indicate a linear relationship. P-value Linearity < alpha and p-value Deviation < alpha indicate a linear relationship. P-value Linearity > alpha and p-value Deviation < or > alpha indicate a relationship cannot be concluded. Bivariate analysis in this case, namely V9 ​​is influenced by V1, V2, V3, V4, V5, V6, & V7. The Linearity Test results show that only V3 is non-linear to V9.

<img src="https://private-user-images.githubusercontent.com/85277959/572260158-db850aac-6cbe-4117-ae4f-0a78fbdc4666.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQ1NTcsIm5iZiI6MTc3NTAxNDI1NywicGF0aCI6Ii84NTI3Nzk1OS81NzIyNjAxNTgtZGI4NTBhYWMtNmNiZS00MTE3LWFlNGYtMGE3OGZiZGM0NjY2LmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMzA1N1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWVkNWM3NjIxN2MxYTg2Njg3ZjBkMjlkMTFjMGFiOGNkYzY2OTFlZTIzYzIwYjRkNDc5N2JhNWY1ODVmNzYzODYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.VNP-G-LT1N9csQEgWuoVF_ffGxpTsKvERfN6DN6WG9o" width="500"/>

### **Dealing with Non-linier Data**
If a non-linear relationship is detected, the most direct approach is to change one or both variables to achieve linearity. An alternative with data transformation is carried out to create new variables to represent the non-linear part of the relationship (Hair et al., 2014). The variable V3 to V9 forms a right convex curve, so a quadratic transformation is performed on the dependent variable (V9) first. Based on the Linearity Test of Variable V9 to the new transformed V3 data, the p-value (0.024) < significance level (0.05) so that there is still no linear relationship. So the next step is to transform the independent variable (V3) with a quadratic. The result is p-value (0.029) < significance level (0.05) so that there is still no linear relationship either. The linearity visualization of V3 and V9 shows a negative curvilinear relationship. Because it is impossible to force changes in the distribution of dependent and independent variables to follow a straight line, simple non-linear regression analysis can be used for bivariate and multivariate analysis.

___
## 8. CORRELATION
Simple correlation analysis is used to determine whether there is a relationship between independent and dependent variables, what the direction of the relationship is, and how strong the relationship is. The correlation coefficient produces a quantitative measure that describes the strength of the relationship between two variables. A correlation coefficient of -1.00 or +1.00 indicates a perfect correlation. A value close to 0 indicates a weak relationship between variables, a value close to 1 indicates a positive/direct relationship between variables, and a value close to -1 indicates a negative/inverse relationship between variables (Lind, et al., 2014).

There are various methods to determine the correlation coefficient that is differentiated based on the type of observation data. The most commonly used correlation coefficient is the Pearson product moment correlation coefficient which is used for ratio/interval measurement scale data (Jackson, 2015). Delivery speed (V1), Price Level (V2), Price Flexibility (V3), Manufacturer Image (V4), Service (V5), Salesforce Image (V6), & Product Quality (V7) variables against Satisfaction level (V9), where all of these variables are ratio data.

<img src="https://private-user-images.githubusercontent.com/85277959/572260229-22455eab-f489-4be1-8569-648abd8651aa.jpg?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzUwMTQ1ODEsIm5iZiI6MTc3NTAxNDI4MSwicGF0aCI6Ii84NTI3Nzk1OS81NzIyNjAyMjktMjI0NTVlYWItZjQ4OS00YmUxLTg1NjktNjQ4YWJkODY1MWFhLmpwZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA0MDElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwNDAxVDAzMzEyMVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTMxMzVhYTQxMWQ0NzRhMTVkYWVjZjE0MDUxMTA0NmQzZDVjZjhjYWMyOGM3ZTQ2YjUzNGZhNjllYjFkMDIwYTEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.oX_guyAGiWCal0i2sr_hsQslN_3eZyYJxIkVDobXe6o" width="1000"/>

Another correlation coefficient method is Kendall's tau-b correlation coefficient. This method is used to determine the non-parametric relationship between two ordinal-scale variables/one of the ordinal-scale data while the other data is continuous data, ratio and interval data (Ma, Y. 2012) or non-continuous data, such as nominal data whose use is changed as ranking data so that it becomes ordinal-scale. An example of this correlation is the Size of Firm variable (V10) which is ordinal data with Satisfaction Level (V9) which is ratio data. The non-parametric correlation coefficient V10 with V9 produces a moderate relationship strength (-0.408) with a negative relationship direction. This indicates that the larger the company, the smaller the purchase satisfaction.

___
## 9. CONCLUSION
- To maintain the statical power of intact sample data, data deletion needs to be avoided. Missing values ​​cannot be ignored if the observed variables are related to each other. Missing values ​​also cannot be ignored if the cause of the missing value is due to imperfections in filling out the questionnaire. Handling missing values ​​can be done by looking at how large the average percentage of the total missing values ​​is in the variables and cases. A small percentage of missing values ​​can be handled by imputing values ​​based on the characteristics of the type and distribution of normality of the data. Substitution with the mean value is done for normally distributed quantitative data, substitution with the median value is done for non-normally distributed quantitative data, and substitution with the mode value is done for qualitative data.

- Outliers handling is done to ensure the validity of statistical results. Outliers in univariate analysis can be detected by boxplot visualization, outliers in bivariate analysis can be detected using studentized residual scatterplot visualization, and outliers in multivariate analysis can be detected using the Mahalanobis D² method for all independent metric variables. All cases that are outliers are summarized as candidates for which cases to be deleted, namely cases that have a large average total missing value.

- Normality Test can be done by analyzing histogram visualization, skewness value, and kurtosis value, as well as Kolmogorov-Smirnov statistical test. To handle data abnormality, it is necessary to transform the data according to its distribution characteristics. The transformed data is then used as a substitute for the original data for further analysis. Optimization of distribution normality improvement can be influenced by sample size, the presence of outliers, or indeed the basic data distribution is indeed not normal, so that any transformation will not change its basic properties. In this case, further analysis still uses the original data.

- Homoscedasticity Test can be done with Levene Test to test the equality of variance between groups of nonmetric variables against metric variables. Heteroscedasticity of data can be caused by the abnormality of one of the variables. To overcome heteroscedasticity, data transformation is carried out with the same approach as handling abnormality.

- Data transformation can be done as an effort to recover non-linear data. However, if the data transformation effort fails to make the data linear, then the statistical analysis that can be used is non-linear regression analysis so that non-linear relationships can be modeled more accurately.
Non-linear relationships can show a strong correlation at the Pearson Correlation r value. However, Pearson's r is less precise in interpreting the strength of the relationship between variables. Other methods can be used to obtain more accurate curvilinear correlation results.

___
## REFERENCE
> Hair Jr., J.F., Black, W.C., Babin, B.J., dan Anderson, R.E. (2014). Multivariate Data Analysis. Edisi 7. Amerika: Pearson Education.

> Hendrawati, T. (2015). Kajian Metode Imputasi Dalam Menangani Missing Data. Proceedings of the 2015 UMS National Seminar on 	Mathematics and Mathematics Education, pp. 637-642.

> Jackson, S. L. (2015). Research Methods: A Modular Approach, 3rd Edition. America: Cengage Learning.

> Jamaluddin & Tommeng, L. (2018). Pengaruh Teknologi Informasi terhadap Kualitas Layanan di UPT Perpustakaan Universitas 	Hasanuddin. Jurnal Pustakawan, 25(4), pp. 11-23.

> Lind, D. A., Marchal, W. G., dan Wathen, S. A. (2014). Teknik-teknik Statistika dalam Bisnis dan Ekonomi. Edisi 15 Buku 2. Jakarta: 	Salemba Empat.

> Ma, Y. (2012). On Interface fo Kendall’s Τ Within a Longitudinal Data Setting. Journal of Applied Statistics, 39, pp. 2441-2445.



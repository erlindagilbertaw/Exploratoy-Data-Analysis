# Exploratory Data Analysis:<br> Data Examination and Assumption Testing on A Dataset

<table style="text-align:left;">
<tr>
<td style="vertical-align: top; padding-right: 20px;">
  <img src="https://github.com/user-attachments/assets/67489ce5-8e1c-4ec6-96d9-125b2d3ea78b" alt="Foto Erlinda" width="150" style="border:none;"/>
</td>

<td style="vertical-align: top;">

  <h2 style="margin:0; text-align:left; font-size:30px;">
    Authors:
  </h2>

  <h2 style="margin:0; text-align:left; font-size:30px;">
    Ir. Erlinda Gilberta Wibawa, S.T., M.T.
  </h2>

  <p style="margin:0; text-align:left; font-size:23px;">
    <a href="https://www.instagram.com/erlinda_gilberta/?hl=en" target="_blank">
      @erlinda_gilberta
    </a>
  </p>

  <h4 style="margin-top:5px; text-align:left; font-size:23px;">
    <em>
      Lecturer in Logistics Engineering,<br>
      Universitas Katolik Santo Agustinus Hippo,<br>
      West Kalimantan, Indonesia
    </em>
  </h4>

</td>
</tr>
</table>

<table style="text-align:left;">
<tr>
<td style="vertical-align: top; padding-right: 20px;">
  <img src="https://github.com/user-attachments/assets/6cde8ceb-f001-4cc4-b998-fed4bf727863" 
       alt="Foto Yosephine Suharyanti" width="150" style="border:none;"/>
</td>

<td style="vertical-align: top;">

  <h2 style="margin:0; text-align:left; font-size:30px;">
    Dr. Ir. Yosephine Suharyanti, S.T., M.T.
  </h2>

  <h4 style="margin-top:5px; text-align:left; font-size:23px;">
    <em>
      Lecturer in Industrial Engineering,<br>
      Universitas Atma Jaya Yogyakarta,<br>
      Yogyakarta, Indonesia
    </em>
  </h4>

</td>
</tr>
</table>

Data is a very valuable asset in making various decisions. However, raw data collected from various sources often cannot be used directly. This can be caused by various constraints that often arise in the data collection process. If used directly without adjusting the feasibility and requirements of certain statistical analysis methods, the data has the potential to produce misleading or inaccurate interpretations. Therefore, a systematic initial process is needed to explore the structure and characteristics of the data before further analysis is carried out. This aims to ensure that the data is in a condition that is suitable for valid and accountable analysis. One approach that is commonly used is Exploratory Data Analysis (EDA).

EDA is the initial stage in data analysis that aims to understand patterns, detect anomalies, and test assumptions through statistical techniques and visualization. In this study, data examination and assumption testing were carried out to identify missing values ​​and outliers from the raw dataset so that it is worthy of further analysis. Without the right examination process, statistical analysis can produce errors and produce invalid interpretations. Furthermore, assumption testing is carried out to ensure that the data meets certain requirements determined by a statistical analysis method. Ignoring assumption testing can lead to errors in decision making and interpretation of results. Data examination and assumption testing are important foundations in statistical data analysis which aim to increase the validity and reliability of analysis results.

This study aims to analyze the importance of data examination and assumption testing in preparing datasets to be statistically feasible. This study is expected to improve the quality of data analysis, so that data-based decision making becomes more accurate and valid.

<img src="https://github.com/user-attachments/assets/5fb18790-1c38-4f29-8bca-4191046e0d16" alt="Image1" width="1000"/>

___
## 1. DATA
This study uses the [*HBAT_MISSING*](https://github.com/erlindagilbertaw/EDA_DataExamination_AssumptionTesting.github.io/blob/main/HBAT_Missing.xlsx) dataset that adopts information from the HATCO Dataset Documentation. The dataset consists of 70 respondents on 14 separate variables. This dataset is used to illustrate the implementation of data examination techniques and assumption tests. 

<img src="https://github.com/user-attachments/assets/b59126dc-5c19-48d3-a88b-08dc757edece" alt="Table1" width="1000"/>

___
## 2. INITIAL NORMALITY TEST
Data examination begins by conducting a Normality Test to determine the normality of quantitative variables. The normality test is carried out using the Kolmogorov-Smirnov method. The Kolmogorov-Smirnov test calculates the level of significance of the difference from the normal distribution. A significance value > significance level indicates that the variable data is normally distributed. Variables V1 to V4 and V6 to V9 have a p-value > alpha, indicating that the variables are normally distributed. In this quantitative data variable, only V5 is not normally distributed (p-value 0.043 < alpha 0.05).

<img src="https://github.com/user-attachments/assets/5f51ca64-a9d8-4761-adcf-22a4a3e87fd8" alt="Table2" width="500"/>

___
## 3. MISSING VALUES
In this case, it is assumed that missing values ​​cannot be ignored because they are known to originate from errors in completing the entire questionnaire.

<img src="https://github.com/user-attachments/assets/d5d1ec9b-3c1b-4f59-b28b-8eb06a036876" alt="Image2" width="500"/>

### **Handling Missing Values**
Missing data can be handled by deleting or filling with a value. If the missing data is relatively small compared to the total data, then deleting incomplete data is one reasonable approach. Variables with at least 15% missing data are candidates for deletion, but higher levels of missing data (20% - 30%) can often be corrected (Hair et al., 2014). As stated by Hair et al., (2014), deletion of missing data is only done if the probability of Missing at Random (MAR) or Missing Completely at Random (MCAR) of the response is independent of the observed/missing data values. If the variables influence each other, then deletion is not the right choice.

<img src="https://github.com/user-attachments/assets/2fd71cb1-866b-477f-ad68-286b0b0df033" alt="Table3" width="500"/>

The number of missing data can be reviewed based on variables and cases. It is known that the percentage of missing values ​​for each variable in the dataset is far below 15%, the largest is V1 (7.78%), so all are maintained. While the percentage of missing values ​​in cases is quite a lot above 15%. Therefore, so that the sample size is not reduced in order to maintain statistical power, imputation is carried out to replace missing values ​​in cases with possible values ​​based on the information obtained in the dataset (Hendrawati, 2015). One method of imputing missing values ​​is to calculate the mean/median/mode value as a substitute for the emptiness/error of the observation value. Replacement of missing values ​​in normally distributed metric data (V1, V2, V3, V4, V6, V7, V8, and V9) is done with the mean value, non-normally distributed metric data (V5) is done with the median value, and nonmetric data (V10 - V14) is done with the mode value.

___
## 4. NORMALITY TEST
Normality Test can be known from the statistical values ​​for the skewness and kurtosis values. If one of the calculated z values ​​exceeds the specified critical value, then the distribution characteristics are not normal. The critical value comes from the z distribution, based on the specified significance level. The most commonly used critical values ​​are ± 2.58 for a significance level of 0.01 and ± 1.96 for a significance level of 0.05. It can be seen from the 9 quantitative variables, only variables V4 and V9 are normal, the other variables (V1, V2, V3, V5, V6, V7, and V8) show deviations from normality in the Normality Test as a whole.

<img src="https://github.com/user-attachments/assets/1d7afe7c-078d-4936-9ce4-4e329d52da1c" alt="Table4" width="1000"/>

### **Dealing with Non-normal Data**

Hair et al., (2014) explained that data transformation provides the primary means of correcting for abnormality. Trial error data transformation is done by applying all possible transformations and then selecting the most appropriate transformed variable (Hair et al., 2014). The results of the data transformation will replace the original data from the previous step (handling outliers).
- In V6, there is no transformation that can improve normality, so this variable must be used in its original form.
- In V3, V5, V7, and V8, it can change to increase sharply to a more acceptable level of significance.
- In V1 and V2 there is only a small change in the increase in significance. This can be caused by the number of outliers retained in V1 and V2, thus affecting the distribution of the variables.

<img src="https://github.com/user-attachments/assets/a5dde9c6-e7db-4c8f-a761-c8d9038bae9d" alt="Image3" width="1000"/>

___
## 5. OUTLIERS
Outliers are unusual observations that are far from other observations. Outliers are usually treated as abnormal values ​​that can affect the overall observation because of their extreme values ​​that are very high (upper outliers) or low (lower outliers).

### 5.1. Outliers Detection for Univariate Analysis
<img src="https://github.com/user-attachments/assets/8a003f01-e969-4312-bddc-e25378da8020" alt="Image4" width="1000"/>

### 5.2. Outliers Detection for Bivariate Analysis

#### 5.2.1. Metric Data V1 – V7 against V9
<img src="https://github.com/user-attachments/assets/a9645b25-6a69-498a-afa1-1e83e33b5daf" alt="Image5" width="1000"/>

#### 5.2.2. Nonmetric Data V10 – V14 against V9
<img src="https://github.com/user-attachments/assets/aafc1417-30bb-430a-a94f-8d8f8eceba1e" alt="Image6" width="1000"/>

### 5.3. Outliers Detection for Multivariate Analysis
Outliers detection in multivariate analysis is performed on all independent metric variables (Hair, et al., 2014), namely V1, V2, V3, V4, V5, V6, and V7. Outliers detection in multivariate analysis is performed using Mahalanobis D² measurements. The results of the Mahalanobis D² distance are then used to search for the Chi-square probability with the numeric expression of probability transformation in SPSS "1-CDF.CHISQ(MAH_1,7)". The number 7 indicates the degree of freedom that corresponds to the number of variables examined (in this case 7 independent variables). Multivariate outliers will appear if the value of the new probability variable is <0.001 (Statistics Solutions, 2020).

<img src="https://github.com/user-attachments/assets/f6d07a7f-984b-46ce-ac17-e841d03246ae" alt="Image7" width="1000"/>

### **Dealing with Outliers**
From 22 cases that have outliers, a decision was made on which cases to delete and which to keep. The decision to keep was made based on the number of cases that appeared more than 1 in the detection of univariate outliers & bivariate outliers. So there were 9 cases that were deleted and 13 cases were kept. 

<img src="https://github.com/user-attachments/assets/d0aaa892-21b2-4f88-a99e-5ab8ebeaa50a" alt="Table5" width="1000"/>

___
## 6. HOMOSKEDASTISITAS TEST
Homoscedasticity Test is conducted with Levene Test on the variance mean data whether the variance of a metric variable is the same in a number of groups. In Levene Test, the variance of metric variables is compared across levels of nonmetric variables. Homoscedasticity Test is suitable for the preparation of analysis of variance (ANOVA) or multivariate analysis of variance where nonmetric variables are independent variables. Homoscedasticity Test is also suitable for discriminant analysis where nonmetric variables are dependent measures (Hair, et al., 2014). Levene Test results show that out of 9 metric variables, only V5 shows a heteroscedasticity pattern (p-value <alpha 0.05) in more than one nonmetric variable (V10 and V14). In addition, none of the nonmetric variables have more than one problematic metric variable.

<img src="https://github.com/user-attachments/assets/cfb2116b-3f07-432b-8735-f6f0b26af9ae" alt="Table6"  width="1000"/>

### **Dealing with Heteroscedasticity Data**
Heteroscedastic variables can be corrected through data transformations similar to those used in the normality test stage. Most heteroscedasticity is the result of non-normality of one of the variables, and conversely, treating non-normality also corrects unequal variance dispersion. So curing heteroscedasticity will also address the normality issue.

Normal data is not necessarily homogeneous and vice versa. In this case, the variable V5 in the non-normality handling step is normal, but when tested for homogeneity, V5 is heterogeneous with respect to the category variables V10 and V14. To overcome this, the data transformation steps as in the normality handling step are carried out again to overcome the heteroscedasticity problem for V5. After being transformed with a square root, heteroscedastic conditions occur in the nonmetric variables V10, V12, and V14. Levene Test is then re-conducted with adjustment of significance level. Heterogeneous nonmetric variables (V10, V12, and V14) are 0.01, while V11 and V13 use significance level of 0.05. Small significance level in V10, V12, and V14 will increase accuracy to reduce the level of testing error.

<img src="https://github.com/user-attachments/assets/ae7726e4-6c39-4a57-a1ed-204fc248a34f" alt="Table7" width="1000"/>

___
## 7. LINEARITY TEST
Linearity Test is used in bivariate and multivariate analysis to determine whether two or more variables have a significant linear relationship or not. Linearity Test is intended to show that the average obtained from the sample data group lies in straight lines (Jamaluddin & Tommeng, 2018). Linearity test can be done by comparing the significant value (p-value) of Linearity and p-value Deviation from Linearity with the level of significance (alpha). So there are 3 conditions for data linearity assessment criteria. P-value Linearity < alpha and p-value Deviation > alpha indicate a linear relationship. P-value Linearity < alpha and p-value Deviation < alpha indicate a non-linear relationship. P-value Linearity > alpha and p-value Deviation < or > alpha indicate a relationship cannot be concluded. Bivariate analysis in this case, namely V9 ​​is influenced by V1, V2, V3, V4, V5, V6, & V7. The Linearity Test results show that only V3 is non-linear to V9.

<img src="https://github.com/user-attachments/assets/eb4fc52f-72f0-4229-9078-176f6e7b734c" alt="Table8" width="1000"/>

<img src="https://github.com/user-attachments/assets/575f3119-d743-445c-ba18-bd4e9888d409" alt="Image8" width="500"/>

### **Dealing with Non-linier Data**
If a non-linear relationship is detected, the most direct approach is to change one or both variables to achieve linearity. An alternative with data transformation is carried out to create new variables to represent the non-linear part of the relationship (Hair et al., 2014). 

<img src="https://github.com/user-attachments/assets/5e7b2cc2-5775-48f1-bd12-0775fbd798c8" alt="Image10" width="500"/>

The variable V3 to V9 forms a right convex curve, so a quadratic transformation is performed on the dependent variable (V9) first. Based on the Linearity Test of Variable V9 to the new transformed V3 data, the p-value (0.024) < significance level (0.05) so that there is still no linear relationship. So the next step is to transform the independent variable (V3) with a quadratic. The result is p-value (0.029) < significance level (0.05) so that there is still no linear relationship either. The linearity visualization of V3 and V9 shows a negative curvilinear relationship. Because it is impossible to force changes in the distribution of dependent and independent variables to follow a straight line, a Simple Non-linear Regression analysis can be used for bivariate and a Multiple Non-linear Regression analysis can be used for multivariate analysis.

___
## 8. CORRELATION
Simple correlation analysis is used to determine whether there is a relationship between independent and dependent variables, what the direction of the relationship is, and how strong the relationship is. The correlation coefficient produces a quantitative measure that describes the strength of the relationship between two variables. A correlation coefficient of -1.00 or +1.00 indicates a perfect correlation. A value close to 0 indicates a weak relationship between variables, a value close to 1 indicates a positive/direct relationship between variables, and a value close to -1 indicates a negative/inverse relationship between variables (Lind, et al., 2014).

There are various methods to determine the correlation coefficient that is differentiated based on the type of observation data. The most commonly used correlation coefficient is the Pearson Product Moment Correlation coefficient which is used for ratio/interval measurement scale data (Jackson, 2015). Delivery speed (V1), Price Level (V2), Price Flexibility (V3), Manufacturer Image (V4), Service (V5), Salesforce Image (V6), & Product Quality (V7) variables against Satisfaction level (V9), where all of these variables are ratio data.

<img src="https://github.com/user-attachments/assets/217a9576-1fdd-4afc-b349-58d2d0e8954e" alt="Image9" width="1000"/>

Another correlation coefficient method is Kendall's tau-b Correlation coefficient. This method is used to determine the non-parametric relationship between two ordinal-scale variables/one of the ordinal-scale data while the other data is continuous data, ratio and interval data (Ma, Y. 2012) or non-continuous data, such as nominal data whose use is changed as ranking data so that it becomes ordinal-scale. An example of this correlation is the Size of Firm variable (V10) which is ordinal data with Satisfaction Level (V9) which is ratio data. The non-parametric correlation coefficient V10 with V9 produces a moderate relationship strength (-0.49) with a negative relationship direction. This indicates that the larger the company, the smaller the purchase satisfaction.

___
## 9. CONCLUSION
- To maintain the statical power of intact sample data, data deletion needs to be avoided. Missing values ​​cannot be ignored if the observed variables are related to each other. Missing values ​​also cannot be ignored if the cause of the missing value is due to imperfections in filling out the questionnaire. Handling missing values ​​can be done by looking at how large the average percentage of the total missing values ​​is in the variables and cases. A small percentage of missing values ​​can be handled by imputing values ​​based on the characteristics of the type and distribution of normality of the data. Substitution with the mean value is done for normally distributed quantitative data, substitution with the median value is done for non-normally distributed quantitative data, and substitution with the mode value is done for qualitative data.

- Outliers handling is done to ensure the validity of statistical results. Outliers in univariate analysis can be detected by boxplot visualization, outliers in bivariate analysis can be detected using studentized residual scatterplot visualization, and outliers in multivariate analysis can be detected using the Mahalanobis D² method for all independent metric variables. All cases that are outliers are summarized as candidates for which cases to be deleted, namely cases that have a large average total missing value.

- Normality Test can be done by analyzing histogram visualization, skewness value, and kurtosis value, as well as Kolmogorov-Smirnov statistical test. To handle data abnormality, it is necessary to transform the data according to its distribution characteristics. The transformed data is then used as a substitute for the original data for further analysis. Optimization of distribution normality improvement can be influenced by sample size, the presence of outliers, or indeed the basic data distribution is indeed not normal, so that any transformation will not change its basic properties. In this case, further analysis still uses the original data.

- Homoscedasticity Test can be done with Levene Test to test the equality of variance between groups of nonmetric variables against metric variables. Heteroscedasticity of data can be caused by the abnormality of one of the variables. To overcome heteroscedasticity, data transformation is carried out with the same approach as handling abnormality.

- Data transformation can be done as an effort to recover non-linear data. However, if the data transformation effort fails to make the data linear, then the statistical analysis that can be used is non-linear regression analysis so that non-linear relationships can be modeled more accurately.
Non-linear relationships can show a strong correlation at the Pearson Correlation r value. However, Pearson's r is less precise in interpreting the strength of the relationship between variables. Other methods can be used to obtain more accurate curvilinear correlation results.

___
## REFERENCES
> Hair Jr., J.F., Black, W.C., Babin, B.J., dan Anderson, R.E. (2014). Multivariate Data Analysis. Edisi 7. Amerika: Pearson Education.

> Hendrawati, T. (2015). Kajian Metode Imputasi Dalam Menangani Missing Data. Proceedings of the 2015 UMS National Seminar on 	Mathematics and Mathematics Education, pp. 637-642.

> Jackson, S. L. (2015). Research Methods: A Modular Approach, 3rd Edition. America: Cengage Learning.

> Jamaluddin & Tommeng, L. (2018). Pengaruh Teknologi Informasi terhadap Kualitas Layanan di UPT Perpustakaan Universitas 	Hasanuddin. Jurnal Pustakawan, 25(4), pp. 11-23.

> Lind, D. A., Marchal, W. G., dan Wathen, S. A. (2014). Teknik-teknik Statistika dalam Bisnis dan Ekonomi. Edisi 15 Buku 2. Jakarta: 	Salemba Empat.

> Ma, Y. (2012). On Interface fo Kendall’s Τ Within a Longitudinal Data Setting. Journal of Applied Statistics, 39, pp. 2441-2445.

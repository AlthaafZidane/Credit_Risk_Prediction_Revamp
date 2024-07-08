This readme file was generated on **2024-06-29** by **Althaaf Athaayaa Daffa Qushayyizidane**

# GENERAL INFORMATION

Credit Risk Predictions:

### **Author/Principal Investigator Information**<br>

Name : Althaaf Athaayaa Daffa Qushayyizidane<br>
Institution : ID/X Partners<br>
Email : althaafzidane@gmail.com<br>

**Date of data collection**: `2023-12-23`

**Geographic location of data collection**: `Indonesia`
<br>

### **DATA & FILE OVERVIEW**

File List: -

Relationship between files, if important: -

Additional related data collected that was not included in the current data package: -

Are there multiple versions of the dataset?
If yes, name of file(s) that was updated: -<br>
Why was the file updated?
When was the file updated?

### **METHODOLOGICAL INFORMATION**

**Description of methods used for collection/generation of data**:<br>

> Data dikumpulkan dari dataset pinjaman yang tersedia secara publik, yang mencakup informasi kredit pelanggan, termasuk status pinjaman, jumlah pinjaman, dan informasi demografis.

**Methods for processing the data**: <br>

1. **Data Cleaning**: Penghapusan nilai yang hilang dan duplikat, serta pembersihan data dari karakter khusus.
2. **Encoding**: Variabel kategorikal diencoding menggunakan LabelEncoder.
3. **Define Target variable**: Menentukan target/label untuk pemodelan.
4. **Feature Engineering**: Melakukan standardization, membuat fitur baru(jika diperlukan).
5. **Feature Selection**: Menggunakan model Random Forest untuk mendapatkan fitur yang paling penting.<br>

**Instrument- or software-specific information needed to interpret the data**: <br>

1. Numpy: 1.26.4
2. Pandas: 2.1.4
3. Seaborn: 0.13.2
4. Scipy: 1.11.4
5. Matplotlib: 3.8.0
6. Sklearn: 1.2.1
7. Imblearn: 0.9.1
8. Gdown: 4.7.3
9. Mlxtend: 0.23.1
10. Xgboost: 2.0.3
11. Lightgbm: 4.3.0
12. Shap: 0.45.0

**Standards and calibration information, if appropriate**: -

**Environmental/experimental conditions**:<br>

> Data dianalisis dalam lingkungan Jupyter Notebook menggunakan Python di sistem operasi Windows 11 Home Single Language.

**Describe any quality-assurance procedures performed on the data**:<br>

> Dilakukan pengecekan dan validasi terhadap nilai yang hilang dan data duplikat. Semua fitur yang dipilih untuk model dievaluasi menggunakan metrik kinerja seperti ROC-AUC, dan dilakukan validasi silang untuk memastikan konsistensi model.

People involved with sample collection, processing, analysis and/or submission:<br>

1. Althaaf Athaayaa Daffa Qushayyizidane
   <br>

### **DATA-SPECIFIC INFORMATION FOR**:

`loan_data_2007_2014.csv`

Number of variables: `75`

Number of cases/rows: `466285`

Variable List: <br>
|Columns|Description|
|:-:|:-:|
|`Unnamed: 0`||
|`id`|A unique LC assigned ID for the loan listing.|
|`member_id`|A unique LC assigned Id for the borrower member.|
|`loan_amnt`|The listed amount of the loan applied for by the borrower.|
|`funded_amnt`|The total amount committed to that loan at that point in time.|
|`funded_amnt_inv`|The total amount promised for the loan at that time.|
|`term`|The number of payments on the loan. Values are in months and can be either 36 or 60.|
|`int_rate`|Interest Rate on the loan.|
|`installment`|The monthly payment owed by the borrower if the loan originates.|
|`grade`|LC assigned loan grade.|
|`sub_grade`|LC assigned loan subgrade|
|`emp_title`|The job title supplied by the Borrower when applying for the loan.|
|`emp_length`|Employment length in years. Possible values are between 0 and 10 where 0 means less than one year and 10 means ten or more years.|
|`home_ownership`|The home ownership status provided by the borrower during registration. Our values are: RENT, OWN, MORTGAGE, OTHER.|
|`annual_inc`|The self-reported annual income provided by the borrower during registration.|
|`verification_status`|Whether the status has been verified.|
|`issue_d`|The month which the loan was funded.|
|`loan_status`|Current status of the loan.|
|`pymnt_plan`|Payment Plan.|
|`url`|URL for the LC page with listing data.|
|`desc`|Loan description provided by the borrower.|
|`purpose`|A category provided by the borrower for the loan request. |
|`title`|The loan title provided by the borrower.|
|`zip_code`|The first 3 numbers of the zip code provided by the borrower in the loan application.|
|`addr_state`|The state provided by the borrower in the loan application|
|`dti`|A ratio calculated using the borrower’s total monthly debt payments on the total debt obligations, excluding mortgage and the requested LC loan, divided by the borrower’s self-reported monthly income.|
|`delinq_2yrs`|The number of 30+ days past-due incidences of delinquency in the borrower's credit file for the past 2 years.|
|`earliest_cr_line`|The date the borrower's earliest reported credit line was opened.|
|`inq_last_6mths`|The number of inquiries in past 6 months (excluding auto and mortgage inquiries)|
|`mths_since_last_delinq`|The number of months since the borrower's last delinquency.|
|`mths_since_last_record`|The number of months since the last public record.|
|`open_acc`|The number of open credit lines in the borrower's credit file.|
|`pub_rec`|Number of derogatory public records.|
|`revol_bal`|Total credit revolving balance.|
|`revol_util`|Revolving line utilization rate, or the amount of credit the borrower is using relative to all available revolving credit.|
|`total_acc`|The total number of credit lines currently in the borrower's credit file|
|`initial_list_status`|The initial listing status of the loan. Possible values are – W, F.|
|`out_prncp`|Remaining outstanding principal for total amount funded.|
|`out_prncp_inv`|Remaining outstanding principal for portion of total amount funded by investors.|
|`total_pymnt`|Payments received to date for total amount funded.|
|`total_pymnt_inv`|Payments received to date for portion of total amount funded by investors.|
|`total_rec_prncp`|Principal received to date.|
|`total_rec_int`|Interest received to date|
|`total_rec_late_fee`|Late fees received to date.|
|`recoveries`|Indicates if a payment plan has been put in place for the loan.|
|`collection_recovery_fee`|Recovery cost when receiving a termination notice.|
|`last_pymnt_d`|Last month payment was received.|
|`last_pymnt_amnt`|Last total payment amount received.|
|`next_pymnt_d`|Next scheduled payment date.|
|`last_credit_pull_d`|When is the last day LC checks credit history|
|`collections_12_mths_ex_med`|Number of collections in 12 months excluding medical collections.|
|`mths_since_last_major_derog`|Months since most recent 90-day or worse rating.|
|`policy_code`|publicly available policy_code=1, new products not publicly available policy_code=2|
|`application_type`|Indicates whether the loan is an individual application or a joint application with two co-borrowers.|
|`annual_inc_joint`|The combined self-reported annual income provided by the co-borrowers during registration.|
|`dti_joint`|A ratio calculated using the co-borrowers' total monthly payments on the total debt obligations, excluding mortgages and the requested LC loan, divided by the co-borrowers' combined self-reported monthly income.|
|`verification_status_joint`|Indicates if the co-borrowers' joint income was verified by LC, not verified, or if the income source was verified.|
|`acc_now_delinq`|The number of accounts on which the borrower is now delinquent.|
|`tot_coll_amt`|Total collection amounts ever owed.|
|`tot_cur_bal`|Total current balance of all accounts.|
|`open_acc_6m`|Number of open trades in last 6 months|
|`open_il_6m`|Number of currently active installment trades.|
|`open_il_12m`|Number of installment accounts opened in past 12 months.|
|`open_il_24m`|Number of installment accounts opened in past 24 months.|
|`mths_since_rcnt_il`|Months since most recent installment accounts opened.|
|`total_bal_il`|Total current balance of all installment accounts.|
|`il_util`|Ratio of total current balance to high credit/credit limit on all install acct.|
|`open_rv_12m`|Number of revolving trades opened in past 12 months.|
|`open_rv_24m`|Number of installment accounts opened in past 24 months.|
|`max_bal_bc`|Maximum current balance owed on all revolving accounts.|
|`all_util`|Balance to credit limit on all trades|
|`total_rev_hi_lim`|Total revolving high credit/credit limit|
|`inq_fi`|Number of personal finance inquiries.|
|`total_cu_tl`|Number of finance trades.|
|`inq_last_12m`|Number of credit inquiries in past 12 months|

Missing data codes: <br>

```
# Fill missing values with a placeholder (e.g., -999)
X.fillna(-999, inplace=True)
```

```
threshold = 0.7

def check_missing_values(df_preprocess):
    missing_value = df_preprocess.isnull().sum() / len(df_preprocess)
    return missing_value

missing_value = check_missing_values(df_preprocess)

def drop_missing_value(df_preprocess) :
    columns_to_drop = missing_value[missing_value > threshold].index
    drop_missing_values = df_preprocess.drop(columns=columns_to_drop, inplace=True)

drop_missing_value(df_preprocess)

def fill_missing_value(df_preprocess) :
    for col in df_preprocess.columns:
        if df_preprocess[col].dtypes == 'object' :
            df_preprocess[col].fillna(df_preprocess[col].mode()[0], inplace=True)
        else:
            df_preprocess[col].fillna(df_preprocess[col].median(), inplace=True)

fill_missing_value(df_preprocess)
```

Specialized formats or other abbreviations used:

- np: Numpy
- pd: Pandas
- sns: Seaborn
- plt: matplotlib
- df: DataFrame
- AUC: Area Under Curve
- lg: Logistic Regression
- knn: KNeighbors
- dt: Decision Tree
- rf: Random Forest
- xgb: XGBoost
- lgb: LightGBM
- grd: Gradient Boost

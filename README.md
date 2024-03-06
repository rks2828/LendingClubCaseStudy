# Lending Club Case Study
> Lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labeled as 'charged-off' are the 'defaulters'. The company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables that are strong indicators of default.  
> This case study involves performing exploratory data analysis on the loan records that were shared in the form of CSV. The company can utilize this knowledge for its portfolio and risk assessment.


## Table of Contents
* [General Information](#general-information)
* [Technologies Used](#technologies-used)
* [Exploratory Data Analysis](#exploratory-data-analysis)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Performing EDA on the shared loan csv will provide the driving factors that can be utilized for the risk assessment for the new applicants.
- borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 
  If one can identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.
- **Dataset used**: loan.csv

## Technologies Used
- Python 3.12.2
- Jupyter Notebook
- python libraries - numpy, pandas, matplotlib, seaborn

## Exploratory Data Analysis
Below are the EDA steps performed, 
- **Data Sourcing**
  - The private data was sourced by importing a CSV file using pandas library. 
- **Data Cleaning**
  - **Fix rows and columns:** 
    Merge columns for creating unique identifiers if needed: E.g. Merge State, City into Full address
		Split columns for more data: Split address to get State and City to analyse each separately
		Add column names: Add column names if missing
		Rename columns consistently: Abbreviations, encoded columns
		Delete columns: Delete unnecessary columns
		Align misaligned columns: Dataset may have shifted columns

  - **Fix missing values:**
    Set values as missing values
		Adding is good, exaggerating is bad
		Delete rows, columns
		Fill partial missing values using business judgement

  - **Standardise values:**
    Standardise units: Ensure all observations under a variable have a common and consistent unit, e.g. convert lbs to kgs, miles/hr to km/hr, etc.
		Scale values if required:  Make sure the observations under a variable have a common scale
		Standardise precision for better presentation of data, e.g. 4.5312341 kgs to 4.53 kgs.
		Remove outliers: Remove high and low values that would disproportionately affect the results of your analysis.

  - **Fix invalid values:**
    Encode unicode properly
		Convert incorrect data types
		Correct values that go beyond range
		Correct values not in the list
		Correct wrong structure
		Validate internal rules
  - **Filter data:**
    Deduplicate data: Remove identical rows, remove rows where some columns are identical
		Filter rows: Filter by segment, filter by date period to get only the rows relevant to the analysis
		Filter columns: Pick columns relevant to the analysis
		Aggregate data: Group by required keys, aggregate the rest

- **Univariate Analysis**
    
- **Segmented Univariate Analysis**

- **Bivariate Analysis**
    
- **Python libraries used** - pandas, matplotlib, seaborn
  
## Conclusions
- Univariate Analysis
  - 80% of the loans are in fully paid status and almost 15% are charged off.   
- Segmented Univariate Analysis
  - Borrowers with higher Grades have a high chance of default.
  - The borrower with a higher term of the loan has a high chance of defaulting.
  - The borrower with the purpose of "Small Business" has a high chance of defaulting.
- Bivariate Analysis
  - The borrower who has a high revolving utilization rate has a high chance of defaulting.
  - The borrower making late monthly credit installment payments has a high chance of defaulting.
  - The borrower with a higher DTI-Debt to Income ratio has a high chance of defaulting.
  - The borrower with a higher number of public record bankruptcies has a high chance of defaulting.
  - The borrower who has made a higher number of loan inquiries has a high chance of defaulting.
  


## Acknowledgements
**Contributors**
- Swarnali Sen
- Rajesh Kumar Singh


## Contact
Created by [@rks2828, @swarnalisen] - feel free to contact us!

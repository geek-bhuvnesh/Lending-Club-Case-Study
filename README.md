# Lending Club Case Study

**Lending Club is US based peer-to-peer consumer finance company founded in 2007.
Lending Club specialises in lending various types of loans to urban customers.
LendingClub matches borrowers with investors willing to fund their loans.**

> When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

- If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company.
- If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company.

## Table of Contents

- [Problem Statement](#problem-statement)
- [General Info](#general-information)
- [Conclusions](#conclusions)
- [Technologies Used](#technologies-used)
- [Acknowledgements](#acknowledgements)

## Problem Statement

### Business Understanding

When a person applies for a loan, there are two types of decisions that could be taken by the company:

**Loan accepted**: If the company approves the loan, there are 3 possible scenarios described below:

- Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

- Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

- Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan

**Loan rejected**: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)

### Business Objectives

This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface.

Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'.

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default. The company can utilise this knowledge for its portfolio and risk assessment.

To develop your understanding of the domain, you are advised to independently research a little about risk analytics (understanding the types of variables and their significance should be enough).

## General Information

- Steps for EDA :
<ol>
    <li>Data Understanding</li>
    <li>Data Cleaning</li>
    <li>Univariate Analysis</li>
    <li>Bivariate Analysis</li>
    <li>Multivariate Analysis</li>
    <li>Conclusion</li>
</ol>
- Data Set : Loan Lending Club loans

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusion: 

<div class="alert alert-block alert-danger">
    <span style='font-family:Georgia'>
        <b>Key determinants influencing the likelihood of borrower default: </b> <br><br>
        <b>Continuous Variable: </b>
        <ul>
            <li>Loan amount greater than 15000 dollars have higher default rate</li>
            <li>Funded amount greater than 15000 dollars have higher default rate</li>
            <li>Funded amount invested greater than 15000 dollars have higher default rate</li>
            <li>As Interest rate increases the default rate increases steeply</li>
            <li>As the annual income increase the default rate decreases</li>
            <li>As dti increase the default rate increases</li>
            <li>Higher Incomes along with good grades usually leads to less defaulting</li>
            <li>Grades and Sub grades by and large depict creditworthiness of a borrower</li>
        </ul>
        <b>Categorical Variable: </b>
        <ul>
            <li>60 months term have a higher default rate than 36 months term</li>
            <li>As the Grade decreases (A B C D E F G) default rate increases</li>
            <li>As the Subgrade decreases (A1 A2 B1 B2.....) default rate increases</li>
            <li>The percentage of loans defaulted is higher for verified borrowers</li>
            <li>Small business borrowers have high default rate</li>
            <li>The percentage of defaulted loans is very high for the state of NE and high for NV and SD</li>
        </ul>
    </span>
</div>
<div class="alert alert-block alert-warning">
    <span style='font-family:Georgia'>
        <b>Some of determinants that may or may not determine whether an applicant will be Defaulter:</b> 
        <ul>
            <li>MONTHS_SINCE_LAST_DELINQ</li>
            <li>STATE</li>
            <li>EMPLOYEE TITLE</li>
            <li>ZIP CODE</li>
        </ul>
    </span>
</div>

## Technologies Used

- Python 3.10.11
- pandas - 2.0.2
- numpy - 1.24.3
- matplotlib - 3.7.1
- seaborn - 0.12.2

## Acknowledgements

- This project was group case study for an online advance course.
- https://www.kaggle.com/
- https://www.geeksforgeeks.org/
- https://seaborn.pydata.org/
- https://pandas.pydata.org/
- https://learn.upgrad.com/

## Contact

Created by [@pragya2611] [@geek-bhuvnesh] feel free to contact us!

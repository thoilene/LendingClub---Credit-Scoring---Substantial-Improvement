# Substantial Improvement in Credit Scoring of Lending Club Loans
Substantial Improvement in Credit Scoring of Lending Club Loans

## Introduction

LendingClub used FICO scores to assess the credit creditworthiness of its clients like many other lenders. According to the online article [LendingClub: FICO's New Model Won't Help](https://www.pymnts.com/consumer-finance/2020/lendingclub-president-fico-model-wont-save-credit-scoring-dinosaur/) - << the president of LendingClub, said that traditional credit scoring — such as through the FICO credit score — misrepresents creditworthiness of individuals >>.

LendingClub is a leading lender in the USA. It publishes quarterly loan data online and thus offers its audience the possibility to evaluate the loans. The current work will show that FICO scores indeed misrepresent creditworthiness of individuals as a lot of loans with good FICO scores get into trouble. Most importanly, this work uses Data Science techniques to develop a substancial improvement in credit scoring of LendingClub loans.  

Let's assume that the last FICO rate range score is used to monitor credit risk and predict the final loan status which is "Fully Paid" for good loan or "Default", "Charged Off","Late (31-120 days)" for bad loan. This work will focus on following main objectives

- Use ML metrics "accuracy" and "f1-score" to show the limitation of the FICO credit scoring model
- Create an ML model which improves the FICO credit scoring model significantly on LendingClub loan data
- Demontrate the truthfulness and reliability of the model

Here are some ML metrics which will be helpfull in this context:

**accuracy = (TP + TN) /(TP+FP+TN+FN)**

**recall = TP/(TP+FN)**

**F1 = 2.0 x accuracy x recall/(accuracy + recall)**

**ROC-Curve: measure of truthfulness and reliability of the model**

- TP: True positives - number of good loans ("Fully Paid") which have been predicted good 
- TN: True negatives - number of bad loans (not "Fully Paid") which have been predicted bad 
- FP: False positives - number of good loans ("Fully Paid") which have been predicted bad
- FN: False negatives - number of bad loans (not "Fully Paid") which have been predicted good

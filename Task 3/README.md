# Task: Build a Credit Risk Model to Predict Probability of Default (PD)

## Task Overview
Here is your task:
The risk manager has collected data on the loan borrowers. The data is in tabular format, with each row providing details of the borrower, including their income, total loans outstanding, and a few other metrics. There is also a column indicating if the borrower has previously defaulted on a loan. You must use this data to build a model that, given details for any loan described above, will predict the probability that the borrower will default (also known as PD: the probability of default). Use the provided data to train a function that will estimate the probability of default for a borrower. Assuming a recovery rate of 10%, this can be used to give the expected loss on a loan.

## Task Instructions
1. **Build a model to estimate the probability of default (PD) for a borrower.**
   - Use the provided data to train the model.
   - The data includes details such as borrower's income, total loans outstanding, and a column indicating if the borrower has previously defaulted on a loan.

2. **Produce a function that takes in the properties of a loan and outputs the expected loss.**
   - The expected loss can be calculated using the formula: `Expected Loss = Probability of Default (PD) * (1 - Recovery Rate) * Exposure at Default (EAD)`, where the Recovery Rate is 10%.

3. **Explore various modeling techniques:**
   - Simple regression
   - Decision tree
   - Advanced machine learning methods

4. **Provide a comparative analysis of the different methods used.**

## Important Notes
- This role often requires the knowledge and utilization of data analysis and machine learning. Python is a useful tool and one that JPMorgan Chase uses a lot in quantitative research since it’s capable of completing complex tasks.
- Moving forward in this program, the example answers are given in Python code. (If Python is not downloaded on your system, you can execute Python code in Jupyter Notebook online for free.)


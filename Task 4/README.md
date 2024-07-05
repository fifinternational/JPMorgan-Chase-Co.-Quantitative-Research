# Task: Create a Rating Map for FICO Scores Using Quantization

## Task Overview
Here is your task:
Charlie wants to make her model work for future data sets, so she needs a general approach to generating the buckets. Given a set number of buckets corresponding to the number of input labels for the model, she would like to find out the boundaries that best summarize the data. You need to create a rating map that maps the FICO score of the borrowers to a rating where a lower rating signifies a better credit score.

## Task Instructions
1. **Understand the process of quantization:**
   - Quantization involves dividing data into buckets and summarizing it.
   - Optimize different properties of the resulting buckets, such as the mean squared error or log-likelihood.

2. **Mean Squared Error:**
   - Approximate all entries in a bucket to one value, minimizing the associated squared error.
   - Minimize the following:
     \[
     \text{MSE} = \sum_{i=1}^{N} (x_i - \hat{x_i})^2
     \]
3. **Log-Likelihood:**
   - Maximize the following log-likelihood function:
     \[
     \text{Log-Likelihood} = \sum_{i=1}^{N} \left( k_i \log(p_i) + (n_i - k_i) \log(1 - p_i) \right)
     \]
   - Where \( b_i \) are the bucket boundaries, \( n_i \) is the number of records in each bucket, \( k_i \) is the number of defaults in each bucket, and \( p_i = \frac{k_i}{n_i} \) is the probability of default in the bucket.
   - This function considers the roughness of discretization and the density of defaults in each bucket.

4. **Dynamic Programming Approach:**
   - Address the problem by splitting it into subproblems and solving incrementally.
   - For example, create five buckets for FICO scores ranging from 0 to 600 and five buckets for FICO scores ranging from 600 to 850.

5. **Create a rating map:**
   - The map should assign a lower rating to better credit scores.
   - Optimize using mean squared error or log-likelihood.

## Important Notes
- This role often requires the knowledge and utilization of data analysis and machine learning. Python is a useful tool and one that JPMorgan Chase uses a lot in quantitative research since it’s capable of completing complex tasks.
- Moving forward in this program, the example answers are given in Python code. (If Python is not downloaded on your system, you can execute Python code in Jupyter Notebook online for free.)


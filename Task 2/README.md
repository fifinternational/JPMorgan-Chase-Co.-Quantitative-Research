# Task: Create a Prototype Pricing Model for Commodity Storage Contract

## Task Overview
Here is your task:
You need to create a prototype pricing model that can go through further validation and testing before being put into production. Eventually, this model may be the basis for fully automated quoting to clients, but for now, the desk will use it with manual oversight to explore options with the client.

## Task Instructions
1. **Write a function that uses the data you created previously to price the contract.**
   - The client may want to choose multiple dates to inject and withdraw a set amount of gas, so your approach should generalize the explanation from before. Consider all the cash flows involved in the product.

2. **Input parameters to be taken into account for pricing:**
   - Injection dates
   - Withdrawal dates
   - The prices at which the commodity can be purchased/sold on those dates
   - The rate at which the gas can be injected/withdrawn
   - The maximum volume that can be stored
   - Storage costs

3. **Write a function that takes these inputs and gives back the value of the contract.**
   - Assume there is no transport delay and that interest rates are zero.
   - Market holidays, weekends, and bank holidays need not be accounted for.

4. **Test your code by selecting a few sample inputs.**

## Important Notes
- This role often requires the knowledge and utilization of data analysis and machine learning. Python is a useful tool and one that JPMorgan Chase uses a lot in quantitative research since it’s capable of completing complex tasks.
- Moving forward in this program, the example answers are given in Python code. (If Python is not downloaded on your system, you can execute Python code in Jupyter Notebook online for free.)


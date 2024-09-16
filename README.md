# Welcome to Infinitech Development!

Hello there,

We are excited for you to start your new job as a senior data analyst here at Infinitech. Your SQL skills made you a great candidate for this role, and will certainly aid you in many of your projects over the coming years. 

## Your First Project 

Your first project will be to clean our corporate employee archive, which contains all the information about the employees here at Infinitech. Unfortunately, the archive has been poorly maintained and is in need of significant refinement. Therefore, we are requesting that you use SQL queries to review the dataset, find anything that doesn't make sense, and then use SQL deletes/updates to correct the issues. 

## The Dataset

The dataset is in dataset.csv and referred to as *employees* from here on.

## Example

You will need to use your own intuition to identify these instances, but we includes the following example to guide you:

#### Identify nonsense
Query: SELECT DISTINCT age FROM employees  
Response: -1, 0, 24, 58, 223

#### Correct nonsense
Mutation: DELETE FROM employees WHERE age < 0 or age > 110

## Testing

Once you believe you have found all of the nonsense, you can run the test in test.py: *python test.py* 

This will provide feedback if there is anything you have missed. We note that this does depend on a proper installation of python. 
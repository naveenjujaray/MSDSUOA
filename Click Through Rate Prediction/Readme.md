# Problem Statement

Most of the websites you visit include ads. The online advertising industry is huge, and players such as Google, Amazon, and Facebook generate billions of dollars by targeting the correct audiences with relevant ads. Most of the decisions about ads are data-driven solutions such as the following: 
* How do you know which ad to use and who to target?
* Many companies advertise products in the same category, so how do you decide whose ad to display?
* Which ad should be placed on which part of the web page?
* Should a particular ad be pushed on a mobile device or remain on a desktop or laptop?

 

These decisions depend on numerous factors, including when the ad is placed, the site it is placed on, the characteristics of the people who will see the ad, the overall demographics, and more.

 

An important exercise marketing companies need to do before making any of the above decisions is a click-through rate (CTR) prediction. The objective is to predict whether the audience will click on an ad or not and thus help the marketing team answer ad placement-related questions.

 

In online advertising, CTR is a very important metric for evaluating ad performance. CTR prediction systems are thus essential and widely used for sponsored search and real-time bidding.

 

Let’s look at the data description for this assignment in the file below. 
[Download](https://cdn.upgrad.com/uploads/production/eacea03d-1c63-41fa-bbdc-fca44b4d4558/Data+Description+-+Sheet1.csv)

The data set for this assignment has 99,999 rows and 27 columns. It can be downloaded from the link below.
[Download](https://cdn.upgrad.com/uploads/production/542c59da-a2e2-409f-a5aa-c08c55920585/data.csv)

As part of this assignment, you are required to predict whether a user will click on an ad or not. A classification method usually designed to solve such problems is best suited here. However, as part of this assignment, you will be required to apply any 3 of the classification methods taught in Course 3 – The introduction to Machine Learning.

 

**Important Points to keep in mind while solving this assignment.** This is explained using the scenario below:

 

Imagine you are a data scientist working for a marketing company. First, you have to draw important conclusions or insights from the data set you’ve been given. For example, the data set might be imbalanced like ours—the percentage of data points with the label ‘False’ is 87%, and the label ‘True’ is 13%. Later, you understand the nature of the data set and the characteristics of the various columns. While understanding the nature of the data set, suppose you realize that the data has some missing values or outliers, so you work on fixing those values. 

 

Let’s say that while analyzing the nature of the data, you realize that some columns need to be one-hot encoded. For example, in the data set for this problem, some columns such as the banner position are represented as integers when they are actually categorical variables, not continuous variables. Representing such categorical variables with integers gives them an order that does not otherwise exist. 

 

For instance, banner position 3 is not 3 times banner position 1. So you need to find a way to communicate only the category of that particular data point using integers and at the same time make sure no other relation or order is communicated. To learn more about one-hot encoding, refer to the link here.

 

After cleaning up the data set, you will then split the data set into train-test data where you will train the model on the train data and use the test data to predict whether the user is likely to click on an ad or not. Then, an important part of your task is to decide which model works the best for a given business scenario. When selecting an appropriate model, also think of model interpretability. Does this application need an interpretable model? Or should you focus on improving the predictability at the cost of model interpretability? 

 

To do that, you can use evaluation metrics such as accuracy, precision, recall, and the area under the ROC curve to decide which method works best. You can compare these metrics for the 3 classification methods of your choice and explain why one method works better than the other methods.

 

You can use techniques like cross-validation, and feature selection to improve the model predictability. 

 

## Let’s go through the recommended steps for your assignment below:
1. Perform missing value and outlier treatment, if needed, in the data set you received.
2. Perform categorical variable treatment:
    - Identify the categorical columns 
    - Use suitable techniques to treat these categorical columns. For instance, as explained earlier, the banner position is a categorical variable. 
3. Perform a train-test split in the data set (the usual split followed in the industry is 70-30 or 80-20).
4. Identify the 3 classification methods you will use in the data set, and explain the reason you chose those 3 methods in the notebook file you will share in the submission process.
5. For all 3 methods, use appropriate evaluation metrics to assess model performance. Also, evaluate the models' basis the cross-validation.
6. Compare which methods work best based on the evaluation metrics mentioned in the previous point.
7. Use model simplification techniques like feature creation and selection, to improve model predictability. 
8. After building the best model possible, explain the risks associated with adopting the model to the business team (You can create a 3-5 slide presentation)
    - Interpret the evaluation metric of choice 
    - Explain the implications of errors made in the prediction by the model.

Note: it is possible that some of the concepts required to solve the assignment are not yet covered, but we request you to keep doing the parts that you know for now, and for the concepts not taught, they will be covered in the upcoming weeks, before the assignment submission.
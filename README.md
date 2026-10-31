# AI_Assignment_Barnes
This repository has the files for the AI assignment due November 2.

PROMPTS

In this file we will be doing analysis on the card_transdata file and looking at credit card fraud. Start by importing pandas, seaborn, matplotlib.pyplot, plotly.express, train_test_split from sklearn.model_selection, StandardScalar from sklearn.preprocessing, KNeighborsClassifier from sklearn.neighbors, and confusion_matrix, classification_report, accuracy_score, precision_score, recall_score, f1_score from sklearn.metrics


Next create a code cell and load in the csv file called card_transdata. Print the head of this data after you load it in.


Now create two new cells one calling shape and the other calling info on the dataset


Create a markdown cell with 'Data Wrangling' inside it and then create a code cell that counts the number of nulls in each column


Create a new cell and create a new dataframe where there are no rows with null values in them. Then print the shape of this new dataset


Call the head funciton on the newly cleaned dataset


Create a new markdown with 'Visualize the Data' inside. Then create a a new code cell and make a vertical count plot ising seaborn. Use the cleaned data and use the 'fraud' as the x axis. Add a title that says 'Fraud Class Distribution' and show the plot


Create a new cell and use seaborn to create a countplot with the cleaned data using 'used_pin_number as the x axis. Add a title 'Used Pin Distributions' and show the plot


Create a new cell and create a seaborn countplot with the cleaned data and repeat_retailer as the x axis. Add the title 'Repeat Retailer Distribution' and show plot


Create a new cell and make a seaborn countplot with 'online_orders' as the x axis. Add the title 'Online Orders' and show plot.


Create a new cell with a seaborn histplot where ratio_to_median_purchase_price is the x axis. Make it with 30 bins and add title 'Ratio to Median Purchase Price Distribution'. Then show plot


Create a new markdown cell that says 'Better Visualizations: Bivariate Visualizations'. Then create a code cell that makes a seaborn countplot with the cleaned data. used_pin_number will be the x axis, fraud will be the hue, and the palette will be green and red. Add a title 'Transactions with PIN vs Fraudulent Transactions', xlabel 'Used PIN', ylabel 'Count', and a legend titled 'Fraud' with labels 'Non-Fraudulent' and 'Fraudulent'


Create a new cell and create a new dataframe that is grouped by used_pin_number and contains fraud value counts unstacked and multiplied by 100. Normalize should also be true. Create a stacked bar plot with fig size (5,3) from this new dataframe. It should have colors green and red. Add title 'Percentage of Fraudulent Transactions with PIN Usage', xlabel Used Pin, ylabel Percentage, adn a legend with same lables as last chart. 


Create a new cell and set plt figure to (5,3). Then make a seaborn countplot from the cleaned data with 'used_chip' as the x axis, 'fraud' as the hue, and green and red as the palette. Add a title 'Transactions with Chip vs Fraudulent Transactions', xlabel 'Used Chip', ylabel 'Count', and legend with title 'Fraud' and labels 'Non-Fraudulent' and 'Fraudulent'. Then create a new dataframe from the cleaned data that is grouped by 'used_chip' and contains value counts for 'Fraud'. unstack it and multiply by 100. Normalize should be set to true. Then create a bar plot from this new dataframe with stacked being true, color being green and red, and figure size (5,3). Add the title 'Percentage of Fraudulent Transactions with Chip Usage', xlabel 'Used Chip', ylablel 'Percentage', and a legend like the one in the previous chart. show both plots.


Create a new cell and set figsize to (5,3). Create a countplot with the cleaned data where online order is the x axis, fraud is the hue, and palette is red green. Set the title to 'Transactions with Online Order vs Fraudulent Transactions', the xlabel to Online Order, and the ylabel to Count. Use the same legend that has been used in previous charts. Then create a new dataframe from the cleaned data that is grouped by 'online_order' and contains value counts of 'fraud', set normalize to true and unstack followed by multiplying by 100. With this dataframe create a bar plot with size (10,6). Stacked should be true and color is green and red. Add the title 'Percentage of Fraudulent Transactions with Online Order', xlabel Online Order, ylabel Percentage, and the same legend as previous charts. Show both plots.


Create a new cell and set figsize to (10,6). Create a scatter plot from the cleaned data with x being 'distance_from_last_transaction' and y being 'ratio_to_median_purchase_price'. Hue should be fraud with colors green and red. Set title to 'Fraudulent vs Non-Fraudulent Transactions: Distance from Last Transaction vs Ratio to Median Purchase Price', xlabel to 'Distance from Last Transaction', and ylabel 'Ratio to Median Purchase Price'.




2. I used the built in copilot in VS code. 

5.  I found AI to be very useful in for creating code, expically when needing basic plots and charts. It is nice to be able to tell an AI to create a chart with certain variables and it quickly creates the chart. However, I did not find AI to be useful when making or changing small details. For example, specifying labels and figure size is something that is much easier to do by hand and not through a chat bot, especially when wanting specific sizes or labels.

One example of verification I ran into was with the simple functions in the beginning of the assignment. The chat bot printed the calling of the functions a couple times, resulting in something much different than what was desired. These simple functions to access descriptive stats and shape of the data are things that are best done by hand and not through a chat bot. I definitley see why it is important to know what you want and know how to do it before off loading it to an AI. After charts were made I was able to look through the code and make an assessment on it because we have already learned the how to make these charts. That makes verifying the code and having the AI make chnages to the code much easier. 

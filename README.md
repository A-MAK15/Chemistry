# Wine Classification
This repository consists of the methods followed to determine if a specific wine belongs to wine 1, 2, or 3
based on the certain ingredients that are utilized. Two algorithms are utilized to construct this classification 
and the results are compared. I explored the dataset by checking the first 5 rows of the dataset and the last 5 
rows as well just to check the structure of the dataset. I also checked the length of the data frame to see if it
matches to the number of rows in the csv file that contained the dataset. I also checked for the duplicates and the 
results all returned false. For basic statistics, I described the data frame so that I can see the mean and standard 
deviation of the ingredients of these wines. My approach to understanding this data was to get the averages of these 
attributes (ingredients) so that I can be able to easily see which ingredients had the most effect in a particular 
wine type. Before I got these averages, I grouped all the different wine types together as their own dataset, and then
I proceeded to describe each data frame then I got my results (mean and std). That’s only when I constructed my visuals
(bar graph) using these averages as my data of interest.

## Features
The first step I took was to check for null values in the data frame for all columns and the results came back as non-null
for all columns. After I had visualized the averages of these attributes, I saw that Proline (one of the attributes) is
dominant in comparison to other attributes, therefore I had to standardize the attributes so that they can all be within the 
same range.  For the multi-layer perceptron algorithm, I split the data into validation (0.25), testing (0.25), and training (0.50)
dataset. For the Random Forest, I split the data into training (0.50) and testing (0.50).

## Results
I chose the MLP and Random Forest classification algorithm and I trained and tested each model on the training dataset.
The models were evaluated, the MLP had an accuracy of 0.970 and the rest of the classification report can be seen in the
output of the code. The confusion matrix has been visualized and the ROC curve has been constructed as well. In the ROC 
curve, as the False Positive Rate increases the True Positive Rate remained constant for some time but eventually started
to increase slightly for both the MLP and Random Forest.

The random forest algorithm is the model that has performed the best in comparison to the MLP algorithm due to the fact that
I had increased the number of nodes in the hidden layer to 20 nodes which made the algorithm reach convergence in a few 
iterations than the MLP.

## Requirements
To run the project, ensure you have the following installed:

- **Python 3.8+**
- **Libraries**
  - **pandas**
  - **numpy**
  - **matplotlib**
  - **seaborn**
  - **scikit-learn**
    
## Future work
- Develop a web application for easy interaction and understanding

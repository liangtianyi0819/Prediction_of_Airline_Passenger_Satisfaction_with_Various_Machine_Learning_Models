# Machine Learning Classification: Predicting Airline Passenger Satisfaction

Project creator: [Tianyi Liang](https://www.linkedin.com/in/tianyi-liang-at-bu/)

This repository contains a Machine Learning model that predicts airline passenger satisfaction based on a range of features including the quality of services, flight characteristics, and personal features of the passengers.

## Table of Contents

1. [Dataset](#dataset)
2. [Requirements](#requirements)
3. [Methodology](#methodology)
4. [Results](#results)
5. [Conclusion](#conclusion)
6. [Insights](#insights)

## Dataset <a name="dataset"></a>

The project uses the dataset "Airline Passenger Satisfaction Score Classification" from Kaggle, which includes the following features:

* Gender: Gender of the passengers (Female, Male)
* Customer Type: The customer type (Loyal customer, disloyal customer)
* Age: The actual age of the passengers
* Type of Travel: Purpose of the flight of the passengers (Personal Travel, Business Travel)
* Class: Travel class in the plane of the passengers (Business, Eco, Eco Plus)
* Flight Distance: The flight distance of this journey
* Inflight Wi-Fi service: Satisfaction level of the inflight wifi service (0:Not Applicable;1-5)
* Departure/Arrival time convenient: Satisfaction level of Departure/Arrival time convenient
* Ease of Online booking: Satisfaction level of online booking
* Gate location: Satisfaction level of Gate location
* Food and drink: Satisfaction level of Food and drink
* Online boarding: Satisfaction level of online boarding
* Seat comfort: Satisfaction level of Seat comfort
* Inflight entertainment: Satisfaction level of inflight entertainment
* On-board service: Satisfaction level of On-board service
* Leg room service: Satisfaction level of Leg room service
* Baggage handling: Satisfaction level of baggage handling
* Check-in service: Satisfaction level of Check-in service
* Inflight service: Satisfaction level of inflight service
* Cleanliness: Satisfaction level of Cleanliness
* Departure Delay in Minutes: Minutes delayed when departure
* Arrival Delay in Minutes: Minutes delayed when Arrival
* Satisfaction: Airline satisfaction level(Satisfaction, neutral or dissatisfaction)

## Requirements <a name="requirements"></a>

This project uses Python along with several additional libraries. These are:

* Pandas for data processing
* Scikit-Learn for machine learning models
* Seaborn and Matplotlib for plotting graphs
* Numpy for basic operations

## Methodology <a name="methodology"></a>

1. Data reading and preprocessing.
2. Data visualization.
3. Data splitting into train and test sets.
4. Model training and evaluation with various classifiers, including:
   * K-Nearest Neighbors Classifier
   * Logistic Regression Classifier
   * Polynomial Regression Classifier
   * Naive Bayes Classifier
   * Decision Tree Classifier
5. Model comparison based on accuracy.

## Results <a name="results"></a>

The accuracy of each model depends on the parameters used. Here are some representative results:

* K-Nearest Neighbors Classifier: Best accuracy of 65.7% at k=12.
* Logistic Regression Classifier: Best accuracy of 76.13% at C=301.
* Polynomial Regression Classifier: Best accuracy of 92.58% at degree=2.
* Naive Bayes Classifier: Accuracy of 85.0%.
* Decision Tree Classifier: Accuracy ranged from 89% to 94%.

Please note that these results can vary depending on the random state during the train-test split and other factors. For more details on how these models were trained and evaluated, please refer to the code in the Jupyter Notebook file in this repository.

## Conclusion <a name="conclusion"></a>

This project showcased the applicability and effectiveness of various machine learning classifiers in predicting airline passenger satisfaction. It revealed that the accuracy of predicting passenger satisfaction greatly depends on the classification algorithm used. Among the classifiers tested, the Polynomial Regression Classifier showed the most promising results with the highest accuracy of 92.58% at degree=2, followed by the Decision Tree Classifier which had an accuracy range of 89% to 94%.

The project also underlines the importance of data preprocessing and visualization in understanding and manipulating the data for optimal results. Through visualization, we were able to understand the distribution and correlation of variables, thereby informing our choices of classifiers and parameters.

## Insights <a name="insights"></a>

Through the results of the project, we understand that passenger satisfaction in the airline industry can be influenced by a variety of factors, which are reflected in our feature set. Each feature contributes uniquely to the model’s performance, and it's worth noting that different models might weigh these features differently when making predictions. 

The high accuracy of the Polynomial Regression Classifier and Decision Tree Classifier suggests that these models might be better at capturing the complexity and patterns inherent in the satisfaction data, compared to the other models tested. This implies that customer satisfaction could be a function of intricate relationships between the features, and not solely reliant on individual factors. 

Future work could explore further feature engineering, the use of more sophisticated models, or the application of ensemble methods to improve prediction accuracy. Moreover, this project underscores the potential value of machine learning applications within the customer service domain, particularly for data-driven decision making and predictive analytics. It offers insights that can be leveraged by airlines to enhance customer satisfaction and tailor their services according to customer preferences and needs.

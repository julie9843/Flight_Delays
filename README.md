# Predicting flight delays 

Flight delays are inevitbable.. Or are they? 

Flight delay is an important subject to tackle for air transportation all over the world. There are various reasons for why a flight can get delayed including weather conditions, mechanical problems, and bird strikes! Due to the large number of reasons for a delay, the data we are faced with is massive, which 

According to the Bureau of Transportation Statistics of the United States, over 20% of US flights were delayed during 2018. 

Knowing the status of the flight is crucial as it plays a role in both the profits and loss of the corresponding airline. Accurately predicting delay times can increase profit and customer satisfaction. 

In this project, I applied various machine learning algorithms to predict if a flight will or will not be delayed according to the data we are given. 


## Data Exploration 
By utilizing tableau, I was able to generate simple and interactive plots that would help me better understand the data I was given. 

The first thing that came to mind when I thought of flight delays was whether the departure airport was busy or not. 
<img width="1270" alt="Screen Shot 2021-06-22 at 2 34 24 PM" src="https://user-images.githubusercontent.com/77126366/123002603-f24a1b80-d366-11eb-8d0d-a7411e885611.png">
Figure 1. Busiest airports and the corresponding number of flights 

Chicago, Atlanta and New York landed the Top 3 busiest airports in terms of the total number of flights they had. 



Another factor that can play in flight delays can be the corresponding airline carrier that is responsible for each of the flights. 
<img width="1217" alt="Screen Shot 2021-06-22 at 2 36 11 PM" src="https://user-images.githubusercontent.com/77126366/123002829-33dac680-d367-11eb-8766-e28bb3f58332.png">
Figure 2. Percentage of flight delays by each airline carrier 

Based off the plots, the top 3 airline carriers with the most delays are: 
1. Commut Air
2. Trans States Airlines
3. JetBlue



I also thought the seasonality of each flight mattered. So I looked into whether arrival delay varies per month. 
<img width="1203" alt="Screen Shot 2021-06-22 at 2 42 34 PM" src="https://user-images.githubusercontent.com/77126366/123003464-15c19600-d368-11eb-866f-48f7b8ce61a9.png">
Figure 3. Month vs number of arrival delays 

We can see that there is a clear spike in the number of arrival delays during the summer months - when people are most likely to go on vacation. 



Combining all the exploratory data analysis I have gathered, I've created an interactive plot that can easily visualize which airports have the most number of flights, most number of arrival delays, as well as its reason for the delay. 

<img width="902" alt="Screen Shot 2021-06-22 at 2 33 28 PM" src="https://user-images.githubusercontent.com/77126366/123002477-d2b2f300-d366-11eb-9363-671ee00ec1fa.png">
Figure 4. Interactive plot of airports


## Modelling 
This will be a binary classification problem to tackle. "0" will correspond to a flight being on time, and "1" will be a flight that is delayed. 

The models that I've used for binary classification are the following: 
1. Random Forest 
2. AdaBoost
3. XGBoost 
4. Naive Bayes 


Further, I wanted to see if I could predict how long the delay would be with regression models. 

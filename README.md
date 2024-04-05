# Twitter_Airline_Sentiment-Analysis

<img align="center" src="https://media.sproutsocial.com/uploads/2020/09/Benefits-of-Twitter-v03.svg"/>

## Description
Twitter is one of the most powerful social media platforms if not the most powerful one
</br>
Big companies from all over the world give huge attention to knowing the opinions of the customers in different fields so they can know what they love, hate or even what is not important to them so the companies can learn from their mistakes and improve their services 
</br>
This data contains 14640 tweet Sentiments about US airlines('Virgin America', 'United', 'Southwest', 'Delta', 'US Airways', 'American') with dates 
</br>
Data was scraped from February of 2015 (2015-02-16) to(2015-02-24) 9 days range
</br>
## Data Analysis
the objective was to analyze these tweets and know the reasons behind them such as (late flights, customer service, etc)
</br>
### Negative Tweets
The most negative reasons were issues with customer service and late flights 
![image](https://user-images.githubusercontent.com/94745919/234127521-69e5c18f-8241-451c-bf52-31816c9c5eb4.png)
</br>
The number of total tweets about every airline was:
</br>
* United:            3822
* US Airways:        2913
* American:          2759
* Southwest:         2420
* Delta:             2222
* Virgin America:     504

![image](https://user-images.githubusercontent.com/94745919/234128501-002de867-b0da-4bcd-baff-b326aeda1304.png)
* United airline has the most negative sentiment (over 2500)
* Virgin America has the highest neutral & positive percentages of all of them

![image](https://user-images.githubusercontent.com/94745919/234134808-9e50f46b-0ed8-49a5-8aa7-b2612c7b8018.png)

* over 65% of the tweets about American, United, and US Airways are negative and they all combined took around 73% of the negative tweets
* Other airlines share only the rest of the 27%
* from the first look and according to the percentages Virgin is the best Airline and US Airways Airline is the worst

Number of Sentiments in each Day:
![image](https://user-images.githubusercontent.com/94745919/234131383-17137125-2228-4854-bf80-2f8902188f3c.png)
</br>
Flights on 2015-02-22 & 2015-02-23 have the most airline sentiment and most negative ones
</br>
Reasons for negative sentimental tweets for each airline
![image](https://user-images.githubusercontent.com/94745919/234135343-c60f9605-f8ab-40a9-987e-c4c44a3a16bf.png)
the main problem and complaints it the customer service except whose major problem is late flights more than customer service and comes in second place late flights and damaged luggage is the least negative reason to complain
</br>
Let's see on which days each airline gets negative and its reasons
![image](https://user-images.githubusercontent.com/94745919/234135542-c9cf8719-66ae-4504-adb5-90380ade9734.png)
</br>
this plot shows that the American airline negative tweets started only from day 22-02-2015 and before that, they didn't have any problems ('according to the negative tweets') so it's a new thing that may be a temporary problem mostly caused by the Customer service and fixing this problem should make things back to normal
</br>
United and US Airlines are consistently getting negative tweets so it is an old problem and it's caused a lot of things mostly(Customer service, late fights) so they should fix these two first
</br>
Delta and Virgin America are the least likely to get negative tweets on the last day(24-02-2015) and it seems they fixed their problems, especially Delta whose negative tweets are significantly reduced over time
</br>
The most common words the negative tweets have:
</br>
![image](https://user-images.githubusercontent.com/94745919/234135767-ac147efb-036f-47dd-b158-1095e5d81170.png)
</br>
some of the words have a double meaning like plane, flight, customer service, etc but they are in negative tweets so we will take them the negative way
</br>
we can see that flight is the most frequent word but it doesn't mean anything (because its airlines' tweets a flight word is most likely to be in a tweet whether it is positive or negative)but it may represent bad flight in general
</br>
we can see also that the late flights whether delayed or canceled
</br>
and also there is a plane and seat problems and maybe bag and luggage damage or lose
## Positive Tweets Analysis
The majority of the tweets were negative but there were also positive tweets let's see its reasons
The most common words the negative tweets have:
</br>
![image](https://user-images.githubusercontent.com/94745919/234135945-c48a8b0c-3591-49cc-8a63-ab540668d9e3.png)
</br>
## Modeling
This process is about building a classifier that classifies the positive and negative tweets so the company can keep track of its work more easily
</br>
cleaning the tweets is the first step before modeling so the model can give a good accuracy 
</br>
First is removing the words and symbols that won't be useful in the classification using nltk
</br>
Then using SVC to classify the cleaned tweets
</br>
![image](https://user-images.githubusercontent.com/94745919/234137758-c9166300-49c9-4a58-87ad-2ab745c9a7f0.png)
</br>
**Accuracy Score is: 0.9241164241164241**

    |precision  |  recall | f1-score  | support|

    |negative   |    0.93 |     0.98   |   0.95 |    2323|
    |positive   |    0.88 |     0.71   |   0.79 |     563|

    |accuracy   |                      |   0.92 |    2886|
    |macro avg  |     0.90 |     0.84  |   0.87 |    2886|
    |weighted avg |   0.92 |     0.92  |   0.92 |    2886|

</br>
</br>
Data link=https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment

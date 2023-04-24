# Twitter_Airline_Sentiment-Analysis
![image](https://user-images.githubusercontent.com/94745919/234124700-504283f1-e501-48da-ba0b-5a4b877f2a45.png)
## Description
Tweeter is one of the most powerful social media platforms if not the most powerful one
</br>
Big companys from all over the world give it a huge attention to know the opinions of the customers in different fileds so they can know what they love,hate or even what is not important to them so the companys can learn form there mistakes and improve there services 
</br>
This data contains 14640 tweet Sentiments about US airlines('Virgin America', 'United', 'Southwest', 'Delta', 'US Airways','American') with dates 
</br>
Data was scraped from February of 2015 (2015-02-16) to(2015-02-24) 9 days range
</br>
## Data Analysis
the objective was to analysis these tweets and know the reasons behind them such as (late flight,customer serves,etc)
</br>
### Negative Tweets
The most negative reasons was issues about the customer service and late flights 
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
* United airline have the most negative sentiment (over 2500)
* Virgin America is the highest neutral & positive percentage of all of them

![image](https://user-images.githubusercontent.com/94745919/234134808-9e50f46b-0ed8-49a5-8aa7-b2612c7b8018.png)

* over 65% of the tweets about American, United and Us airways are negative and they all combined took around 73% of the negative tweets
* others airline share only the rest of the 27%
* from first look and according to the percentages Virgin is the best Airline and US Airways Airline is the worest

Number of Sentiment in each day:
![image](https://user-images.githubusercontent.com/94745919/234131383-17137125-2228-4854-bf80-2f8902188f3c.png)
</br>
Flights on 2015-02-22 & 2015-02-23 have the most airline sentiment and most negative ones
</br>
Reasons for negative sentimental tweets for each airline
![image](https://user-images.githubusercontent.com/94745919/234135343-c60f9605-f8ab-40a9-987e-c4c44a3a16bf.png)
the main problem and complain it the customer serveice except who's major problem is late flights more than customer serveice and come in the second place late flights and damage luggage is the least negativereason to be complained
</br>
lets see in which days each airline get negativereason and its reasons
![image](https://user-images.githubusercontent.com/94745919/234135542-c9cf8719-66ae-4504-adb5-90380ade9734.png)
</br>
this plot shows that the American airline negative tweets starts only from day 22-02-2015 and before that they didn't have any proplem('according the negative tweets') so its a new thing may be temporary problem mostly caused by the Customer serveies and fixing this problem should make things back to normal
</br>
United and US Airlines are consistently getting negative tweets so its an old proplem and it's cause alot of things mostly(Customer serveies,late fights) so they should fixs these two first
</br>
Delta and Virgin Amarica are the least to get negative tweets on the last day(24-02-2015) and it seems they fixed there problems especially Delta which its negative tweets are significantly redused over time
</br>
Most common words the negative tweets have:
</br>
![image](https://user-images.githubusercontent.com/94745919/234135767-ac147efb-036f-47dd-b158-1095e5d81170.png)
</br>
some of the words have double meaning but like plane,flight,customer servive,etc but the are in negative tweets so we will take them the negative way
</br>
we can see that flight is the most freq word but if dosen't mean anything (because is airlines tweets so the most likely to have flight in the tweets)but it may represent bad fligt in genral
</br>
we can see also that the late flights whether was delayed or canceled
</br>
and also there is a plane and seats problems and may be bag and luggage damage or lose
## Postive Tweets Analysis
The majorty of the tweets were negative but there where also postive tweets lets see it's reasons
Most common words the negative tweets have:
</br>
![image](https://user-images.githubusercontent.com/94745919/234135945-c48a8b0c-3591-49cc-8a63-ab540668d9e3.png)
</br>
## Modeling
This process is about bulind a classifier that classifies the postive and negative tweets so the company can keep track of its work more easly
</br>
cleaning the tweets is the first step in before modeling so the model can give a good accuracy 
</br>
Frist is removing the words and symbols that wont be useful in the classification using nltk
</br>
Then using SVC to classify the cleaned tweets
</br>
![image](https://user-images.githubusercontent.com/94745919/234137758-c9166300-49c9-4a58-87ad-2ab745c9a7f0.png)
</br>
**Accuracy Score is: 0.9241164241164241**

    |precision  |  recall | f1-score  | support|

    |negative   |    0.93 |     0.98   |   0.95 |     2323|
    |positive   |    0.88 |     0.71   |   0.79 |     563|

    |accuracy   |                      |   0.92 |    2886|
    |macro avg  |     0.90 |     0.84  |   0.87 |    2886|
    |weighted avg |   0.92 |     0.92  |   0.92 |    2886|

</br>
</br>
Data link=https://www.kaggle.com/datasets/crowdflower/twitter-airline-sentiment

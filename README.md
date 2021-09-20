( Predicting Market Volatility and building short-term trading strategies using data from Reddit's WallStreetBets. )

**Short Description:**
The aim of this project is to use data from posts made on the sub-reddit 'WallStreetBets' to make a prediction on stock prices and market volatility. Various features were extracted from these posts and a learning model was trained to predict if specific stocks rose or fell in the given timeframe.

**Content:**
1. Project Approach
2. What does the DATA tell us?
3. Our PREDICTION models
4. PERFORMANCE evaluate
5. CONCLUSION & NEXT STEP

**Data Collection:**
As per project requirement, the data from the news portals or social media sites which has
lot of stock enthusiast, Customers, Investors, Companies and so on is needed. So, the data
from Reddit’s WallStreetBets can be used. For this project, two different datasets will be
used.
a. SPX file which contains lot of ‘High’, ‘Low’, ‘Close’, ‘Open’, ‘Volume’, so we’ll trim it
out as per the Kaggle file named SP500. Hence from this file we’ll get four columns:
i. Open
ii. Close
iii. High
iv. Low
v. Volume
vi. Date
![alt text](https://github.com/bidhyapokharel/Predict-Market-Volatility/blob/master/Documentation-Report/sent.png)
b. JSON file that contains the body of WSB post. Since, this file is very large we’ll take out
only
i. Body
ii. Date
iii. Score
We’ll also create the target variable using open and close value. Where our condition will
be, if yesterday’s closing price is smaller than today’s closing price then our value will be 1
similiarly vice versa.

**Data Cleaning:**

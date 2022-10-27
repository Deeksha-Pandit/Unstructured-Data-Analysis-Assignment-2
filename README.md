# Unstructured-Data-Analysis-Assignment-2

Unstructured Data Analytics (Fall 2022)
Assignment #2
Note: While this assignment is about politics and the upcoming midterm elections, upon doing this assignment you will obviously see how the overall approach could be applied to a business setting where we analyze what attributes people associate with two competing products or brands, how they feel about such attributes (sentiments), and how the sentiments vary by geography. 

A.	Collect 4-6k tweets on the any senate race in a battleground state (may I suggest John Fetterman and Dr. Mehmet Oz in Pennsylvania). It is preferable to use general hashtags and search keywords (like PA Senate race 2022) rather than “Fetterman” or “Oz” because of the probability of Fetterman or Oz being close to 1 in the latter cases.  Let the occurrences of Fetterman or Oz come naturally in a subset of the tweets you collect. 

B.	Find FOUR key issues mentioned by the public in the tweets – e.g., character, inflation, healthcare, crime, abortion, etc. (these are examples only, use wordfrequency.py to find out). Replace words if necessary. 

C.	
D.	Perform lift and sentiment analysis on each candidate and issue:

	Lift	Sentiment Score (if lift > 1)
Issue 1 & Fetterman	?	?
Issue 2 & John Fetterman	?	?
Issue 3 & John Fetterman	?	?
Issue 4 & John Fetterman	?	?
Issue 1 & Mehmet Oz	?	?
Issue 2 & Mehmet Oz	?	?
Issue 3 & Mehmet Oz	?	?
Issue 4 & Mehmet Oz	?	?

E.	Show the attributes and candidates on an MDS plot (Using mds.py script). 

F.	Use the location data collected in step A to find out lifts and sentiments regarding the candidates in large versus small cities/towns in Pennsylvania. 
G.	What advice would you give to each of the two candidates based on your analyses in C, D and E above?

Guidelines for parts A, B, C, and D – Please read carefully before running the scripts.
1.	Before you collect tweets, find suitable hashtags and keywords (go to Twitter and also search on Google to find out which hashtags and keywords are popular in describing the PA senate race). Keep in mind that there is some trial and error involved in finding suitable keywords for the Twitter search. As a last resort, you can do two searches, one with Fetterman and one with Oz, but first you should try to find more general keywords about the PA senate race. 
2.	Twitter doesn’t like to give more than 3000 tweets in a single search. In fact if you ask for more than 3000, you may get an error. My suggestion is to do multiple searches, each for 3000 tweets, spaced at least by 12 hours (otherwise Twitter will simply send more duplicate tweets). 
3.	Once you have the required tweets, check for duplicate tweets and eliminate them (in Excel you can search for duplicate rows and eliminate them – Google it if you are not familiar with it. If Twitter gives too many duplicates, try searching again after a day or so.  Remember, retweets (RT) are NOT duplicates. A row of data is a duplicate if it completely matches another row. 
4.	You may have to do replacements – e.g., replace Mehmet or other variations by Oz, etc. 
5.	Run the lifts between the 4 issues (like immigration, crime, etc.) and 2 candidates as in the Edmunds assignment. 
6.	For sentiment analysis with issues and candidates (need to do this for candidates & attributes where the lift > 1), you need to write a script to extract windows of words around a keyword. 
Guidelines for E
1.	For location analysis, get a list of PA city and town names from Google. Replace the 5 biggest cities by population (e.g., Pittsburgh, Philadelphia, etc.) with big_city and the rest with small_town. 
2.	Once the replacements are done, merge the location and the text columns into one with the concatenate command in Excel (Google it if not familiar). 
3.	Perform a lift analysis as follows:
	John Fetterman	Mehmet Oz
Big_city PA	Lift?	Lift?
Small_town PA	Lift?	Lift?
Create a matrix as follows from the sentiment scores:
	John Fetterman	Mehmet Oz
Big_city PA	Sentiment score?	Sentiment score?
Small_town PA	Sentiment score?	Sentiment score?

You may find this article relevant to this assignment: https://medium.com/swlh/the-pulse-of-the-nation-a-twitter-analysis-of-the-2020-u-s-presidential-election-15f9afa86ec7

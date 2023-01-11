# Amazon-DataScience-Books-Analysis

Analyzed 1000 DataScience Books on Amazon

# Import Libraries: 
1) Pandas
2)Numpy
3)Plotly
4) Matplotlib.pyplot

Load Dataset.
![image](https://user-images.githubusercontent.com/77182591/204875759-1b54be8f-7720-4314-87e4-c6e3a75638c7.png)

# Exploratory Analysis 
Based on dataset I was curious on do prices of books vary according to reviews written by customers on page. So I plot the graph between average reviews and price. 
![image](https://user-images.githubusercontent.com/77182591/204876080-830f4b5c-8b4d-47d4-b958-dc92d8f354e5.png)

After seeing this I was sure that it pretty much doesn't vary with the reviews given. 

One obvious question arises in mind that do the price also vary on the size of book i.e. length of book?
![image](https://user-images.githubusercontent.com/77182591/204876893-14456558-f704-416a-8623-90e4cea5065f.png)
After seeing the graph it is clear that it does vary with the length of book and the relation is almost linear. 

If someone wanted to start reading about Data Science he/she should start from learning basic python. 
So based on average reviews and no. of reviews I categorized the data to give out the books which contained the word python.
![image](https://user-images.githubusercontent.com/77182591/204877317-1c28408f-5812-44ad-8209-1fea8558944c.png)
The answer came out to be Python-Crash-Course-2nd-Edition

Then should learn about basic Machine Learning. Hence figured out the best ML book.
![image](https://user-images.githubusercontent.com/77182591/204878229-b64f744f-1c94-4742-ba20-6b0a26463b37.png)

## Scrapping Book Reviews

Then started scrapping Amazon Book Reviews. For this I took the website link of a book from amazon along with its review page.Then with this link as an example I created a new dataframe which stored all the previous data alon with the product link and review link as new columns.
![image](https://user-images.githubusercontent.com/77182591/205228692-b49081cc-bb58-4ab7-a961-ef37fd2c7396.png)

For Scrapping the data from the webpage I adapted Code from Jeff James( https://gist.github.com/jrjames83/4653d488801be6f0683b91eda8eeb627)
The above code gave me the data frame with all the books reviews and ratings given to them. 
![image](https://user-images.githubusercontent.com/77182591/205229049-bbdb515d-f196-487d-b787-e81497c1f97c.png)

Then I categorized the reviews according to the title of book and  joined them into a single row.
![image](https://user-images.githubusercontent.com/77182591/205229254-b815d819-be90-4091-bc29-b96ec21929ca.png)

With the help of bert-extract-Summarizer the model Summarized each review row for the given book and presented with a brief summary of it.
![image](https://user-images.githubusercontent.com/77182591/205229433-acb44873-529b-449c-954b-c8614395b2d0.png)
![image](https://user-images.githubusercontent.com/77182591/205229458-e26096bd-2c95-4b51-b393-eaaf3a5cd41c.png)


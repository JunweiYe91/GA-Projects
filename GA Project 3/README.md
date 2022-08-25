# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 3: Ames Housing Data and Kaggle Challenge

### Project Objectives:

You are a data scientist in a well known cosmetic company. The company has an online store and discussion forums for all the product categories. The department in charge of the website and forum has complained that customers are posting their feedbacks and discussions for Makeup and Perfumes in the wrong forums. Due to this, you colleagues have to manually comb through the discussion forums to identify posts that have been posted in the wrong forum. They found this time consuming and have turned to the data science department to look for a better solution.

You have been tasked by your direct supervisor to create a classification model to identify whether posts should be classified in the Makeup or Perfumes column. At the same time, use the analysis to identify useful insights that could be used by the marketing department for their marketing efforts.

---

### Data used:

As the forums were newly created, there isn't sufficient data for us to perform analysis on. As such, we have extract posts from the Makeup and Perfume subreddits to form our dataset.

Information found in the datasets include the title and selftext of the posts. Please refer to the data dictionary for more infomation on the columns extracted.

---

### Data Dictionary:

<br>**Dataset name: `perfumes_df`**
<br>This dataset contains subreddit posts extracted from the "Perfumes" subreddit. 

| Feature | Type | Dataset | Description |
|:--|:-:|:-:|:--|
|subreddit|string|perfumes_df|The subreddit the posts is extracted from. Provides information on the topic of interest.|
|title|string|perfumes_df|Title of the posts found in the subreddit.|
|selftext|string|perfumes_df|Body of the posts found in the subreddit. Usually gives more insights on the posts.|
|title_and_selftext|string|perfumes_df|Combindation of the title and selftext column.|

<br>**Dataset name: `makeup_df`**
<br>This dataset contains subreddit posts extracted from the "Perfumes" subreddit. 

| Feature | Type | Dataset | Description |
|:--|:-:|:-:|:--|
|subreddit|string|makeup_df|The subreddit the posts is extracted from. Provides information on the topic of interest.|
|title|string|makeup_df|Title of the posts found in the subreddit.|
|selftext|string|makeup_df|Body of the posts found in the subreddit. Usually gives more insights on the posts.|
|title_and_selftext|string|makeup_df|Combindation of the title and selftext column.|

<br>**Dataset name: `combined_df`**
<br>This dataset contains subreddit posts extracted from the "Perfumes" subreddit. 

| Feature | Type | Dataset | Description |
|:--|:-:|:-:|:--|
|subreddit|string|combined_df|The subreddit the posts is extracted from. Provides information on the topic of interest.|
|title|string|combined_df|Title of the posts found in the subreddit.|
|selftext|string|combined_df|Body of the posts found in the subreddit. Usually gives more insights on the posts.|
|title_and_selftext|string|combined_df|Combindation of the title and selftext column.|

---

### Key takeaways from the project:
1. The "(TF-IDF) - Naive Bayes Multinomial model is our best performing model with a train score of 0.9522 and a test score of 0.9152.

2. Perfume brands make up most of the top phrases in the Perfume subreddit whereas makeup products made up most of the top phrases in the makeup subreddit.

3. Some of the most mentioned perfume brands are Tom Ford, Victoria Secret and Black Opium.

4. Some of the most mentioned makeup products are Setting Spray, Setting Powder and Eyeshadow Palette.

5. Features that consumers look out for in perfumes are whether the perfumes are long lasting and whether they are appealing to the opposite sex.

6. Features that consumers look out for in makeup are whether the makeup are suitable for their skin.

---

### Limitations and Future Enhancements
1. Words and phrases found and identified were restricted to what were discussed in the subreddit. There could be other topics that were discussed elsewhere. We would suggest scrapping other forums (for example, the forums or comments found on other sites) in addition to the reddit data that we have collected. This could give us a more complete picture on the topics that are most commonly discussed on the forums.

2. The topics discussed on the company's forums might be different from those in the subreddit. We would suggest repeating the analysis when the company website forums have garned enough posts.

3. Analysis is done based on 1 word, 2 words and 3 words phrases. The words do not give us insights on whether the discussions are positive or negative in nature. We would suggest conducting sentiment analysis on the data collected as well.

---

### Recommendations:
Our recommendations are as per below:
1. We would recommend running marketing campaigns on the perfume brands such as Tom Ford, Victoria Secret and Black Opium as these are the most commonly discussed brands. We have taken a look at some of the posts that contain these phrases and it seems like these brands are often recommended by other consumers.
2. When running marketing campaigns for makeup, we would suggest focusing on makeup products instead of brands, because it seems like makeup is less brand sensitive as compared to perfume. We would suggest focusing on the products that are suitable for all kinds of skins.


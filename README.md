# Text Data Analysis - Youtube Case Study
  ![Downpic cc-2012624483](https://github.com/user-attachments/assets/07062909-7ea8-4462-b38f-e03ce48fe33f)

### Project Overview
- This project aims to deliver meaningful findings about how YouTube data is distributed among different categories, dependent on viewer response such as likes, dislikes, emojis and comments.
- I have also performed sentiment analysis using comments to see which words are mostly used in both the negative and positive sense by the viewers.
- Last, but not the least, I have analyzed comments to see how punctuation is effecting useful metrics i-e likes and dislikes.

### Data Source
- Firstly, the data is collected from Youtube, in the form of a csv file named "UScomments.csv", containing columns like comment, likes, replies and more than 50 k rows of data.
- Additional data is also collected, including various csv files, and each contains data with respect to various metrics based on a specific region like Canada, Russia, USA etc.

### Working Tools (Libraries and Packages)
- Python and Pandas - Data Manipulation and Reshaping
- Matplotlib, Seaborn and Plotly - Data Visualization
- Textblob and Wordcloud - Sentiment Analysis
- Emoji - Emoji Analysis

### Data Preprocessing
1. Datatype transformation
2. Data Reshaping
3. Adding new columns for Analysis

### Data Analysis
The following analysis were performed in this project:
1. Wordcloud Representation of Sentiments (Both positive and Negative)
   - Code for positive wordcloud:
     ```
     plt.figure(figsize=(10, 10))
     positive_wordcloud = WordCloud(height=1000, width=1000, stopwords=set(STOPWORDS)).generate(total_postive_comments)
     plt.imshow(positive_wordcloud)
     plt.show()
     ```
   - Code for positive wordcloud:
     ```
     plt.figure(figsize=(10, 10))
     negative_wordcloud = WordCloud(height=1000, width=1000, stopwords=set(STOPWORDS)).generate(total_negative_comments)
     plt.imshow(negative_wordcloud)
     plt.show()
     ```
2. Analyzing the Trending Tags and Views of Youtube
   ```
   plt.figure(figsize=(10, 10))
   tags_wordcloud = WordCloud(height=1000, width=1000, stopwords=set(STOPWORDS)).generate(tags)
   plt.imshow(tags_wordcloud)
   plt.show()
   ```
   - Analyzing the relationship between 'views' VS 'likes':
     
     ![f4b581fe-800d-418f-bec5-39a2da11409f](https://github.com/user-attachments/assets/01baf386-c431-48cd-9c0f-2ff2616e8e57)


   - Analyzing the relationship between 'views' VS 'dislikes':
    
     ![f4b581fe-800d-418f-bec5-39a2da11409f](https://github.com/user-attachments/assets/29b37332-9149-40ef-90e9-d5cc9af15fd0)

3. Perfroming Emoji's Analysis
   
   ![newplot](https://github.com/user-attachments/assets/0ef20399-8f76-4f37-b8aa-4756b918c309)
   
5. Analysing the most liked category of Youtube
6. Analyzing whether audience is engaged or not !
   - Analyzing like rate among different categories
   - Analyzing dislike rate among different categories
   - Analyzing comment rate among different categories
   - Visualizing the relationship between views and likes, views and dislikes

     ![ae3598fe-5efa-43c4-962a-1acb23886438](https://github.com/user-attachments/assets/b4c8666c-cb51-4aed-90bb-32f151e70583)

7. Analyzing trending videos !
8. Do Punctuations have an impact on views, likes, dislikes?

### Results
The results are summarized as follows:
1. The most positive sentiments of viewers are beautiful, awesome, best, perfect, love, amazing etc.
2. The most negative sentiments of viewers are terrible, worst, boring, horrible, awful etc.
3. The most popular trending tags are music video, star wars, makeup tutorial, dude perfect, talk show, movie trailer etc.
4. Likes are very strong correlated with views and may appear to a great predictor for any ML model. The dislikes are not strongly correlated with views.
5. The most common emojis used by viewers are 😂, 😍, ❤, 🔥, 😭, 👏, 😘, 👍, 💖, 💕.
6. The 3 most liked categories of YouTube are Music, Entertainment and Comedy.
7. Almost all the viewers are engaged in the top categories of YouTube in terms of likes and comments.
8. The 3 top trending YouTube channels are The Late Show with Stephen Colbert, WWE and Late Night with Seth Meyers.
9. Videos with comments having less punctuations have more chances of getting higher views than those having many punctuations.

### Recommendations
After going through this anlysis, if someone wants to build their youtube channel, they can easily account for the peculiarities they need to account for before establishing the channel like:
- They can observe how punctuations and emojis are going to affect their viewership.
- Which type of videos and channel are trending and which category of videos they should start to make
- How to engage their audience in a better way
- How to avoid the negative sentiment of viewers

### Limitations
I have only performed analysis based on past data. But there may be chance that YouTube trend has changed over time. Also, this analysis does not include predictive analytics for future results. But, after going through this analysis, somebody can easily perform predictions using ML techniques to see how well this data is going to perform in future.
     
     



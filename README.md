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


     
     



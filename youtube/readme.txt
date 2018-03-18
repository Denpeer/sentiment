see https://www.kaggle.com/datasnaek/youtube/data

Plan
====

Data collected from the (up to) 200 listed trending YouTube videos every day in the US and the UK.

Description
===========

The dataset includes data gathered from videos on YouTube that are contained within the trending category each day.

There are two kinds of data files, one includes comments and one includes video statistics. They are linked by the unique video_id field.



The headers in the video file are:

 - video_id (Common id field to both comment and video csv files)
 - title
 - channel_title
 - category_id (Can be looked up using the included JSON files, but varies per region so use the appropriate JSON file for the CSV file's country)
 - tags (Separated by | character, [none] is displayed if there are no tags)
 - views
 - likes
 - dislikes
 - thumbnail_link
 - date (Formatted like so: [day].[month])



The headers in the comments file are:

 - video_id (Common id field to both comment and video csv files)
 - comment_text
 - likes
 - replies

Extra info: The YouTube API is not effective at formatting comments by relevance, although it claims to do so. As a result, the most relevant comments do not align with the top comments at all, they aren't even sorted by likes or replies.

Inspiration
===========

Possible uses for this dataset could include:

 - Sentiment analysis in a variety of forms
 - Categorising YouTube videos based on their comments and statistics.
 - Training ML algorithms to generate their own YouTube comments.
 - Analysing what factors affect how popular a YouTube video will be.

Although there are likely many more possibilities, including analysis of changes over time etc.

# Topic-Modelling-on-Jeopardy-Questions

The goal of this report is to analyze the topics of the game show Jeopardy!, specifically by the year, rounds, and values. An unsupervised learning method called Latent Dirichlet Allocation was used to simulate the topics in the dataset. The dataset consists of questions from 1984 - 2012 for a variety of topics and values. For this analysis, only the Jeopardy!, Double Jeopardy!, and Final Jeopardy! rounds were used for comparison.

Data preprocessing was done to extract text from the questions. Punctuations, links, and HTML encoded characters were removed. Stopwords were removed using the Sci-kit Learn package. Lastly, all the text was converted to lowercase.

For analysis, the main workflow is illustrated below:

1. Clean text
2. TF-IDF to vectorize data
3. LDA model with 5 topics chosen
4. Find top 10 words per each topic
5. For each question, find the highest probability that a question belongs to a topic; assign that question to topic
6. Visualize words in topic and distribution of questions in each topic

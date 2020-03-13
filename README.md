# News briefer
 Building news briefer using NLP, word vectors

Building a news briefer involves identifying important sentances/words and putting them forward as summarization. 
In this notebook, I played with TimesOfIndia RSS feed to get news article text and created a brief summary of 4/5 sentences for each article. 

Below is the basic data flow:
1. Get RSS feed for a topic. RSS feed contains news headline, link and published-date. 
2. Fetch the link HTML which contains the actual news article. 
3. Using BeautifulSoup library, extract news text from it. 
4. Perform basic text pre-processing such as cleanup/normalization
5. Generate sentence vectors using GloVe algorithm.
6. Rank the sentences using pagerank algorithm. 
7. Take top N sentences which forms the summary of the news article.

# The Impact of Reddit Users on Financial Market Dynamics (BBBY Shares Case Study)

## Project goals 
 - analyze the effect of Reddit users on Bed Bath and Beyond Inc. (BBBY) stock price dynamics and investigate the mechanisms by which committed individuals initiate cascading behaviors in financial markets and social networks.
The paper replicates the research methodology conducted in the article titled ["From Reddit to Wall Street: The role of committed minorities in financial collective action"](https://arxiv.org/pdf/2107.07361.pdf), authored by Lorenzo Lucchini, Luca Maria Aiello, Laura Alessandretti, Gianmarco De Francisci Morales, Michele Starnini, and Andrea Baronchelli in 2021. 

## Project questions:
- Quantify commitment of individual Reddit users of r/wallstreetbets (WSB) subreddit;
- Compare commitment dynamics with BBBY stock shares daily returns;
- Compare Google trend data with BBBY stock shares daily returns
- Investigate the growth of the social identity of WSB participants;
- Conduct sentiment analysis of r/wallstreetbets (WSB) subreddit submissions; 
- Study the dynamics of social interactions between committed individuals and other WSB users.

## Data
- The activity on the subreddit r/wallstreetbets gained by [Academic Torrents](https://academictorrents.com/details/c398a571976c78d346c325bd75c47b82edf6124e))
- The price of Bed Bath and Beyond Inc. shares, ticker BBBY (parsed from Yahoo Finance).
- Google search data and news search interst gained by [Google Trends](https://trends.google.de/trends/)

In overall number of posts: 16 997 
Number of comments: 650 353

## Time period: 
All the data available until December 31, 2022
Analyzed period: from August 1, 2022 up to September 15, 2022 (period of highest activity, 85% of all submitted posts) 

## Quantifying commitment
### Quantifying commitment: number of posts
Peaks in the number of posts on the subreddit align with periods of the highest changes in daily returns and price dynamics. The graph depicting post activity also highlights the two most pronounced periods of post activity.

![map](https://github.com/elenaputilova/reddit_data_analysis/blob/main/images/1.png)

### Comparison to Google search dynamics
The comparison of stock daily returns with Google Trends and Google News search reveals that the increase in public attention to the company (as indicated by the search term ’Bed Bath and Beyond’) does not closely follow the peaks in stock price changes.

![map](https://github.com/elenaputilova/reddit_data_analysis/blob/main/images/2.png)

### Composition of commitment events by flair
”Flairs” refer to descriptive ’tags’ attached to posted threads. To measure financial commitment, three types of flairs were identified in posts: ”profit,” ”loss” (indicating gains or losses exceeding a minimum threshold of $2,500 USD), and ”YOLO” (indicating investment positions at risk with a minimum value of $10,000 USD).
Temporal distribution of commitment events during the selected time period shows that ”profit” posts are the most prevalent in the commitment landscape. Spikes in commitment events occur following significant changes in stock price.
![map](https://github.com/elenaputilova/reddit_data_analysis/blob/main/images/6.png)

## Group identity
Expressions of identity emerged concomitantly with the rise in commitment and abruptly began to decline and deviate after August 17. 

![map](https://github.com/elenaputilova/reddit_data_analysis/blob/main/images/7.png)

## Sentiment analysis of the posts and comments 
Before August 17, the increase in the number of positive posts follows the rise in stock prices. However, after the stock price plummeted, the dynamics of post sentiment deviated from the price dynamics, which also proves a restricted impact of positive sentiment of Reedit posts on market influence during downward movements.

![map](https://github.com/elenaputilova/reddit_data_analysis/blob/main/images/9.png) 

## Network evolution
Nodes represent WSB users, colored according to whether they posted a commitment submission (red) or not (gray). The size of nodes is inversely proportional to their k-shell, meaning that nodes belonging to the core are larger than peripheral nodes. A link exists between two nodes if one of the two replied to the other at least once.
Over time the network appeared sparser, with fewer nodes showing their financial commitment, primarily in the periphery. While it remained more concentrated in the core, the commitment activity spread more towards the periphery.
![map](https://github.com/elenaputilova/reddit_data_analysis/blob/main/images/11.png)

## Network metrics dynamics
Reciprocity -  measures the likelihood of mutual connections between nodes in a directed network.  
Heterogeneity - the degree of variation in the connections that each node maintains.   
Average degree - quantifies, on average, how many connections each node has within the network.   
The diversity and average connections in the network grow, but mutual connections decrease as the network continues to grow before September 17. This characteristic becomes the opposite as the intensity of the discussion declines on WSB.
![map](https://github.com/elenaputilova/reddit_data_analysis/blob/main/images/12.png)

---
**Links to the datasets used in the project**: 
- Academic Torrents with full Reddit dataset: https://academictorrents.com/details/c398a571976c78d346c325bd75c47b82edf6124e 
- JSON with filtered posts https://drive.google.com/file/d/1-Jz3VBoD209_MvcMbfFCd_pD0YE4dXyJ/view?usp=share_link
- JSON with filtered comments https://drive.google.com/file/d/1rXuwMwDiVPR9Hh2fWgj_nzqvmvgTQnl-/view?usp=share_link
- CSV with BBBY shares prices parced from Yahoo finances https://drive.google.com/file/d/15Oq7pPsquZ-R2uQG-IXPlzieE28gFQIq/view?usp=share_link 
- CSV with 'BBBY' search from Google Trends data https://drive.google.com/file/d/1YPJ2jom3aBnL-vECG1QlSmFkm6Dq531t/view?usp=share_link 
- CSV with 'Bed Bath and Beyond' search from Google Trends data  https://drive.google.com/file/d/13WDpGVLWct8kSTHKYlMYIb1k8wYkVsLm/view?usp=share_link
- CSV with news search data https://drive.google.com/file/d/1KZL3_zcpSzwvtPB1lIQnStcnqOr99vZp/view?usp=share_link 

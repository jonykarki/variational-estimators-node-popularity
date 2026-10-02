# Variational Estimators for Node Popularity Models

This repository contains the datasets and data-source information used in the real-world network analyses in:

**Variational Estimators for Node Popularity Models**  
Jony Karki, Dongzhou Huang, and Yunpeng Zhao

## Datasets

### MovieLens 100K

The MovieLens 100K dataset contains 100,000 ratings from 943 users on 1,682 movies. In the paper, the ratings are converted to a binary user-movie adjacency matrix indicating whether each user rated each movie.

**Source:** [GroupLens MovieLens 100K](https://grouplens.org/datasets/movielens/100k/)

The original MovieLens files are not redistributed in this repository in accordance with the GroupLens dataset usage terms.

### Political Blogs

The Political Blogs network records hyperlinks between political blogs during the 2004 U.S. presidential election. We use the largest connected component and treat the network as undirected, resulting in a network with 1,222 nodes and 16,714 edges.

**Data file:** [`data/polblog_data.rda`](data/polblog_data.rda)

**Source:** [M. E. J. Newman — Network Data](https://public.websites.umich.edu/~mejn/netdata/)

**Reference:**  
Adamic, L. A. and Glance, N. (2005). *The Political Blogosphere and the 2004 U.S. Election: Divided They Blog.*

### DBLP

The DBLP network is based on the heterogeneous bibliographic network constructed from DBLP data. Following the preprocessing used in previous work, we consider the database and information-retrieval research areas. The resulting network contains 2,203 nodes and 1,148,044 edges.

**Data file:** [`data/dblp.rds`](data/dblp.rds)

The processed dataset used in our analysis is based on the data accompanying Sengupta and Chen (2018).

**Source:** [Sengupta and Chen — PABM data and code](http://www.apps.stat.vt.edu/sengupta/software_data/PABM/codes_and_data.zip)

**Reference:**  
Sengupta, S. and Chen, Y. (2018). *A Block Model for Node Popularity in Networks with Community Structure.* Journal of the Royal Statistical Society: Series B, 80(2), 365–386.

### British MPs Twitter Network

The British MPs dataset contains Twitter interactions between Members of Parliament and party labels. We use the retweet network, restrict attention to Conservative and Labour MPs, treat the network as undirected, and extract the largest connected component. The resulting network contains 329 nodes and 5,720 edges.

**Data files:**
- [`data/politicsuk-retweets.mtx`](data/politicsuk-retweets.mtx) — retweet network
- [`data/BritishMPcomm.txt`](data/BritishMPcomm.txt) — political-party labels

The processed data used in our analysis are based on the data accompanying Sengupta and Chen (2018).

**Source:** [Sengupta and Chen — PABM data and code](http://www.apps.stat.vt.edu/sengupta/software_data/PABM/codes_and_data.zip)

**Original reference:**  
Greene, D. and Cunningham, P. (2013). *Producing a Unified Graph Representation from Multiple Social Network Views.* Proceedings of the 5th Annual ACM Web Science Conference.
# Website-Ranking-using-Keyword-Extraction-PageRank
Done as a part of course project (group of 2) for CS 257.

## Software and Version
- Python: 3.10.8
- MongoDB: 6.0 
- MongoShell: 1.8.0
- MongoDB Compass: 1.36.4  
The remaining packages and their versions are mentioned in the requirements.txt.

## Setting up MongoDB instance
1. Install MongoDB on your machine using this documentation.
2. Create a Database (‘dbsp’) and two collections (‘article’ and ‘content’) in the MongoDB instance.
3. Create the following indexes using the given commands:

```
- db.article.createIndex({title:"text"})
- db.article.createIndex({article_id:1})
- db.content.createIndex({article_id:1})
- db.content.createIndex({keywords_dict:"text"})
```

## Generating Dataset
1. Download the .ipynb file submitted.
2. Specify the URL to be scraped under the “Retrieval of Pages through Web Scraping” module. 
3. Run all the blocks in the notebook sequentially. 
4. Under the “Inserting the webpages data to DB” heading, mention the IP address and port at which the MongoDB instance is hosted (for example:  'mongodb://127.0.0.1:27017/').
5. Execute the code blocks under the “Page Rank” section.
6. “Visualization” section is only for representation purposes. 

We have also used MongoDB Compass for easier understanding of the Query Execution Plan.

## Task Description
* Developing a framework to scrape websites
* * Extracting data from the website and segregating into columns
* Developing DB schema
* Writing framework for Data Processing
* Designing TF-IDF algorithm
* Updating the DB collections with scraped data
* Analyzing Indexing requirements & configurations
* Determining outbound/inbound links & graph representation
* Developing Page Ranking Algorithm on news articles
* Result Analysis and Optimization
* Report & PPT drafting

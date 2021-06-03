Part A: Text-based industry classification
Cluster the business sections extracted in assignment 3 into 50 clusters (using the cosine similarity) to group firms with similar business descriptions together.

Submit your code and the final output csv file, with CIK, conformed end of period, and the cluster number for each business section file.

Note: it is likely you will need to tokenize/word count each business section file before reading the next one. (If you try to read all business sections before doing any further processing you will probably run out of memory).

Part B: Sentiment
Use the VADER (Valence Aware Dictionary and sEntiment Reasoner) sentiment package to rate the sentiment of the files with text/reviews extracted for one of the two websites you crawled in assignments 1 and 2. Make sure to remove stop words, punctuation and remove words starting with a digit. (So no need to include the code that scraped the website, just read the scraped text from disk.)
Recent uploads: 

HL-1: ended w/ writing filtered files into personal directory;
HL-2: ended w/ initial clustering attempts with in-class codes; 

To-do list: 

Cluster the business sections (/blue/acg7849/share/BS) using Doc2Vec (50 clusters) in two ways:

(DONE - allfiles)  Using a counter as the ‘tag’ (as in 5.1.5)

(  )  Using a counter as the ‘tag’, and the industry code as an additional tag (yield TaggedDocument(words=file_tokens, tags=[i, SIC]) where SIC is a string holding the tag (for example ‘1740’)

(  )  Extract the 4-digit SIC industry code from the annual report header (STANDARD INDUSTRIAL CLASSIFICATION).

Evaluate whether adding the industry code as an additional tag improves the clustering with using standard deviation. (Firms that are more similar, should have similar performance. Therefore, a better clustering would result in lower standard deviations for each cluster, relative to a worse clustering).

(DONE)  filings for the year 2019 only, and BS files that are longer than 1000 characters. 

(  )  Calculate the standard deviation of performance for each cluster. 2 standard deviations for each cluster (one for each approach, with the extra SIC tag vs not adding the extra SIC tag). 

(  )  Use a t-test to test for a difference between the two sets of 50 standard deviations.

(The performance of each firm is provided on Canvas files, folder assignment 5, file performance.csv. This file has the CIK, year and performance.)
(Not all BS files are included in performance.csv. You should still include such firms in the clustering, but not in the calculation of the standard deviation. (So these firms will not influence the evaluation which method is better).)

Expected final output: csv for 50 clusters +2 kinds of SDofP for each. Then a conclusion on whether adding SIC makes clustering better.

DONE = no further changes needed;  TEST = tested on small scale of data

# TDSA Paper Details

The papers defined in the TSV file are for those for the task of Target Dependent Sentiment Analysis (TDSA), also known as Apsect Based Sentiment Analysis (ABSA). TDSA is the task of predicting the sentiment of a target with respect to the text it is within, whereby the target is always in the text and never latent. An example of a TDSA sample is shown below:

Bob said that "**Github** is a great platform for releasing code and is much better than **GitLab**.

This sample has two targets which are in bold (Github and GitLab) which have two different sentiments (positive and negative) in this example. The task for TDSA would be given a target and the text it appears in predict the sentiment towards it for instance given the sample above and the target **Github** the correct prediction would be positive. 

The papers in the TSV file also contains papers that perform Targeted Sentiment Anlysis (TSA) ([Mitchell et al. 2013](https://www.aclweb.org/anthology/D13-1171.pdf)) which is the task of extracting the targets and then predicting the sentiment for those extracted targets. Thus in comparison to TDSA it performs the extraction of targets as an extra step before TDSA. These papers were included in the TSV as they perform TDSA even if it is in a joint manner with the extraction of targets. 

The list of papers in the TSV are not up-to-date, they are all papers that perform the task of TDSA or TSA and have been published after **2013 and before 2019** at the following conferences/workshop 1. ACL, 2. EACL, 3. NAACL, 4. EMNLP, 5. CONLL, 6. COLING, 7. AAAI, 8. TACL, 9. WASSA (workshop). In total there are **31** papers. 

Contains one TSV file with the following headers:
1. Paper -- Title of the paper.
2. Paper URL -- URL to the paper.
3. Dataset -- Name of the dataset(s) used in the paper.
4. External Data -- If any other data was used, this included any data that may have been used to train custom word embeddings, but does not include any data that was used to train pre-trained embeddings taken from another paper e.g. does not include the data used to train the GloVe embeddings if GloVe embeddings were used.
5. Twitter -- If any of the dataset(s) used came from Twitter.
6. Non-Twitter -- If any of the dataset(s) used came from Twitter.
7. Code URL -- URL to the code. This can be either a URL or NA if no code is available. The code URL here is always the offical codebase and not a reproduction from another researcher.
8. Code URL in paper -- If there is a code URL (if not then the value is NA) whether that URL was found in the paper (Yes) or if the URL had to be found through searching for it on the internet (No). Searching for it on the internet mainly involoved googling the authors name or the paper name and looking for either the code on the authors website or looking for a Github link. 
9. Tokeniser from paper -- Name of the tokeniser that was used (if not specified in the paper this is NA).
10. Tokeniser from code -- If the tokeniser was not specifed in the paper and the codebase could be found then the codebased is searched to find the tokeniser used (if not found then NA or if found in the paper NA).
11. Embeddings -- All coulmns from 11 onwards specify the embeddings used in the paper, there is more than one columns as some papers used more than one embedding or tested more than one embedding, thus each column only contains one embedding name. All papers use at least one embedding, the most embeddings used is 4 thus in that case there is an embedding name in column 14.

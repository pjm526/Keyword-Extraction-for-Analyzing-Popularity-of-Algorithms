# Keyword-Extraction-for-Analyzing-Popularity-of-Algorithms

In research and news articles, keywords form an important component since they provide a concise
representation of the article’s content. Keywords play a crucial role in locating the article from
information retrieval systems, bibliographic databases and for search engine optimization. Keywords
also help to categorize the article into the relevant subject or domains.
Conventional approaches of extracting keywords involve manual assignment of keywords based on
the article content and the authors’ judgment. This involves a lot of time and effort and also may not
be accurate in terms of selecting the appropriate keywords. With the emergence of Natural Language
Processing (NLP), keyword extraction has evolved into being effective as well as efficient.

In this project, we’ll be using SparkML on a collection of research papers to extract keywords in order to deduce popularity of Algorithms used.

## Data
In this project, we will be extracting keywords from a dataset that contains about 7939 research papers.
The dataset is from *Kaggle - (NIPS Paper)2. Neural Information Processing Systems (NIPS)* is one
of the top machine learning conferences in the world. This dataset includes the title and abstracts and
paper text for all NIPS papers to date (ranging from the first 1987 conference to the 2016 conference).

## Technologies Used
1. MongoDB
2. Spark
3. SparkML

### Python Libraries
1. Natural Language Processing Toolkit(NLTK)
2. NumPy
3. Matplotlib
4. WordCloud

## Models Used
1. N-grams
2. TF-IDF
3. LDA

## Result
The results of our analysis are shown in figure 7. The output contain a list of tri-grams which are
actually relevant. When observed, we found a few generic tri-grams and hence filtered the list on the
word “Algorithm”. This gave us a much accurate list of all the algorithms used in the papers with
their counts. In order to explicitly see how much a particular algorithm is used, we made a list of all
62 algorithms used till date and filtered out these algorithms. The plot below gives us an idea about
the most researched algorithm and the least researched ones. The biggest challenge faced during the
research was to clean the data in order to make it ready to feed it to the ML Algorithm. We also tried
to test the LDA model and clustered the papers but providing labels to the clusters was challenging.
![algorithmsgraph (1)](https://user-images.githubusercontent.com/43018908/63992069-211f3f80-cab8-11e9-8cc9-8f3c8dbecff0.png)

## Conclusions
In this way we conclude that Support Vector Machine, Recurrent Neural Networks, Stochastic
gradient descent, Principal component analysis are the most researched ones till 2017. However we
can see that Convolution Neural Network is comparatively researched less. Hence there is a scope of
more research in this domain which might help to exploit the usage of these algorithms in efficient
manner. In the future we look forward to extending this approach to classify papers based on the
Algorithms used and also Dynamic Classification for Search Engines.

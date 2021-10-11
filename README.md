# MLimplementations


This will be a guide to implementing ML algorithms as can be used for the course CBDM at ITU. The models include:
1. Clustering (kMeans)
1. Classification (kNN)
1. Network analysis (iGraph)
1. Natural language processing (spaCy)
	1. for LDA see https://www.kaggle.com/thebrownviking20/topic-modelling-with-spacy-and-scikit-learn/data. But replace parser with: 

def lemmatizer(doc):
    return [token.lemma_ for token in doc]

def spacy_tokenizer(setence):
    doc = nlp(setence)
    tokens = lemmatizer(doc)
    tokens = [ word for word in tokens if word not in stopwords and word not in punctuations ]
    tokens = " ".join([i for i in tokens])
    return tokens


Additionally we look at how to use pandas to clean/preprocess data.

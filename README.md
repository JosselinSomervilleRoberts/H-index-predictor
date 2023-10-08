# INF554 data challenge

Visit: https://josselinsomervilleroberts.github.io/ to find a description of the project.

This folder contains the 2 notebooks we used to make submission to the **INF554 Kaggle Competition**.

## Requirements
In order to run these notebooks, you will need 
- numpy
- matplotlib
- nltk
- sklearn
- pandas
- tqdm
- re
- networkx
- pickle
- ast
- stellargraph
- tensorflow
- keras
- gensim 



To use these notebook, you need to change the different paths to the ones on your environment and download the datasets from the INF554 Kaggle Competition.
.
To use the Word2Vec model and compute the features, you will need to download the pretrained model from [lexvec](https://github.com/alexandres/lexvec)
 ## Training and Testing 
 
 You'll need to run the co_author graph analysis notebook first in order to create the features from the graph given in this challenge.
 This consists in a **Node2Vec** model and outputs vectors associated with each authors that represent them in the graph. The more connected two authors are, the closer their associated vectors.
 

 The second notebook will then take these features into account and mix them with features deducted from the abstracts. In order to infer these features, we used **TF-IDF** and **Word2Vec** models.
 
 
 Then these concatenated features go into a feed forward neural network that trains on the train-set and outputs the predicted h-index for the test-set.
 
 

# Geographic Entity Recognizer on Biomedical Abstracts

This repository contains part of the source code for a Geographic Entity Recognizer model on Biomedical Abstracts with the aid of Embeddings, Metadata, and Linked Data. It focuses on three main aspects: data preprocessing, feature engineering, and model training, for reproducibility of experiments.

## 1. Data Preprocessing
This section involves scanning geographic names from the raw abstracts of PubMed 2018 using spaCy and Stanza, and generating the initial silver standard data. Some files are too large to be directly uploaded to GitHub. Please refer to the comments in the code for download instructions.

- Abstract data: Navigate to [this link](http://abel.lis.illinois.edu/data/) and search for `abstracts2018.tsv.gz`.

Note: The provided code demonstrates an example with 1 million data points, which takes several hours to run. To generate the complete dataset, you will need to modify the code to run on the full dataset.

## 2. Feature Engineering
This section focuses on generating metadata, linked data, and other related features. Golden standard data is provided as a sample for testing. Silver standard data can be generated using the code from the data preprocessing section, or by downloading pre-generated features from the links below. Some files are too large to be directly uploaded to GitHub. Please refer to the comments in the code for download instructions.

- MeSH data: Navigate to [this link](http://abel.lis.illinois.edu/data/) and search for `mesh2018.tsv.gz`.
- Citation information: Navigate to [this link](http://abel.lis.illinois.edu/data/PubMed-citation-2018/) and search for `PPUB.tsv.gz`.
- MapAffil data: Navigate to [this link](http://abel.lis.illinois.edu/data/) and search for `MapAffilTempo2018.tsv.gz`.
- MapAffil dictionary: [MapAffil dictionary](https://drive.google.com/file/d/1PMfMJnbkNX03KijSsWcraM3R8wmqma5s/view?usp=sharing)

## 3. Model Training
This section covers the final model training using the silver standard data as the training set and the gold standard data as the test set, incorporating embedding features. It is recommended to upload the training script to Google Colab for execution. The training set is too large to be directly uploaded. Please refer to the comments in the code for download instructions.

- Training data: [training data](https://drive.google.com/file/d/14qRCzfshrPlUHfiqOpYZiLJx4tCFdVhj/view?usp=sharing)

For any questions, please contact [xjiang36@Illinois.edu](mailto:xjiang36@Illinois.edu).

# gcn
GitHub Project README
This repository contains a Python script that generates two files, .content and .cites, based on document-document edges. The script utilizes the scikit-learn library for text processing and similarity calculations.

Description
The purpose of this script is to create two files that can be used for document analysis and graph-based computations. Here's an overview of the files and their generation process:

.content file: This file contains document information in a tab-separated format. Each line represents a document and includes the document ID, a sequence of word IDs, and a label. The word IDs are obtained from a provided vocabulary file. Out-of-vocabulary words are excluded. The content file is created based on the provided dataset files.

.cites file: This file represents document-document edges based on a similarity threshold. It contains pairs of document IDs that have a similarity above the specified threshold. The similarity between documents is calculated using the cosine similarity measure. The threshold can be adjusted according to your requirements. By default, a threshold of 0.7 is used.

Prerequisites
Before running the script, ensure that you have the following:

Python 3.x installed
Required Python libraries: numpy, scikit-learn, and pandas
Usage
Follow these steps to use the script:

Clone or download this repository to your local machine.

Place your dataset files in the specified data_dir directory. The dataset files required are:

sr_sentences.txt: Contains the comments or sentences to be processed.
sr_labels.txt: Contains the corresponding labels for the comments or sentences.
sr_vocabulary.txt: Contains the vocabulary of words to be used for encoding.
Modify the paths in the script (comments_file, labels_file, vocabulary_file, and data_dir) to match the locations of your dataset files.

Adjust the similarity threshold (threshold) if necessary.

Run the script using a Python interpreter.

After the script finishes executing, you will find the generated .content and .cites files in the data_dir directory.

Note
It is important to ensure that the dataset files are in the correct format and that the vocabulary file matches the words in the dataset.

The script uses the TfidfVectorizer from scikit-learn to calculate document similarities based on the TF-IDF representation of the comments. You can explore other vectorization techniques or adjust the vectorizer parameters as per your requirements.

The provided code is a basic implementation. You can modify and extend it according to your specific needs.

License
This project is licensed under the MIT License. Feel free to modify and use it according to your requirements.

Acknowledgments
The script is inspired by various techniques and libraries available for text analysis and graph computations.
The scikit-learn library was used for text processing and similarity calculations.
Please feel free to contribute to this project by submitting issues or pull requests.

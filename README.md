# Sentence Toxicity Classifier

This project aims to build a Sentence Toxicity Classifier that can determine the toxicity level of sentences. We started by using the Kaggle dataset "Jigsaw Toxic Comment Classification Challenge," which not only served as a valuable reference for other submissions but also provided a solid foundation for our work.

### Algorithm Selection

Initially, we implemented Multinomial Naive Bayes as a straightforward entry point to machine learning. Simplicity was key at this stage. However, after testing it on different datasets, we realized that the accuracy was suboptimal. This prompted us to explore more complex algorithms.

### Transition to LSTM RNN

Our choice for a more sophisticated approach led us to the LSTM RNN (Long Short-Term Memory Recurrent Neural Network) model. Simultaneously, we decided to work with the full dataset, which included various toxicity-related labels such as hate speech, threats, and severe toxicity.

### Data Optimization

In the initial stages of the project, we worked with a dataset that included both toxic and non-toxic comments. However, to enhance production speed without compromising the model's accuracy, we made a strategic decision to remove all non-toxic comments from our dataset.

This adjustment did not have a negative impact on the model's performance, as toxicity detection primarily relies on understanding and identifying toxic language. Therefore, focusing solely on the toxic comments proved to be a more efficient approach, allowing us to streamline our workflow and improve overall project efficiency.


### GloVe Embeddings

We initially attempted to streamline the word embedding process by using pre-trained GloVe embeddings. Unfortunately, this approach yielded low accuracy, possibly due to complications arising from tokenization.

### Vectorization Approach

After some research and experimentation, we discovered that a vectorization-only approach was more effective. This change in processing words significantly improved the model's accuracy.

### Overcoming Challenges

Throughout the project, we encountered various challenges, including issues with input compatibility, difficulties graphing validation and loss metrics, and several minor bugs. However, through persistence and problem-solving, we overcame these obstacles.

### Usage

When inputting custom sentences, and the classifier provides the toxicity level results. This project represents our journey from a basic machine learning approach to a more advanced and accurate model for assessing sentence toxicity.

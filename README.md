## Introduction

Within the realm of Natural Language Processing (NLP), I undertook a project centered around text classification. The primary objective was to construct a robust and versatile model capable of discerning tweets that pertained to genuine disasters from those that did not.

The project comprised a systematic exploration of four distinct model architectures, each designed to address the unique challenges associated with text classification:

1. A foundational model was established, featuring essential components such as vectorization and embedding layers, complemented by a hidden feed-forward layer.

2. Building upon this foundation, a more intricate model was created. It incorporated vectorization and embedding layers, along with a global max-pooling layer. This addition enhanced the system's ability to efficiently extract vital information from textual data.

3. The project also involved the implementation of a Bidirectional Long Short-Term Memory (LSTM) model, exploring various directional merge modes. This approach allowed the model to capture complex linguistic dependencies and temporal patterns in the tweets.

4. In keeping with the latest advances in the field, a pre-trained transformer model called 'DIstilBERT' was introduced. This model harnessed the power of transfer learning to enhance the system's ability to understand and interpret nuanced language.

By conducting a thorough and systematic analysis of these models, I aimed to determine the most effective approach for this particular text classification challenge.


## Data Description

The datasets provided for this project, comprising 'train.csv' and 'test.csv,' encompass five key columns, each holding vital information:

1. `id`: A unique identifier assigned to each tweet, ensuring data integrity and traceability.

2. `keyword`: This column captures specific keywords or phrases extracted from the tweets, although it may be left blank in some instances.

3. `location`: Offers insights into the geographical origin of the tweet, when available; however, it may also contain blank entries.

4. `text`: The 'text' column constitutes the heart of the dataset, containing the actual textual content of each tweet, essential for the model to make accurate classifications.

5. `target`: Denoted by binary values, 'target' serves as the target variable for this classification task. A value of '1' signifies that the tweet pertains to a real disaster, while a value of '0' indicates that it does not.


## Conclusion

In this project, I undertook the development of a series of deep learning text classification models using TensorFlow, with the objective of predicting whether a given tweet indicated a disaster or not, using a real-world tweets dataset.

The model-building process was marked by a progression from a basic, shallow neural network to more advanced Transformer-based models. The performance of each model variant is summarized as follows:

1. **Shallow Neural Network:** Demonstrated a train and test set accuracy of approximately **58%**.

2. **Multi-layer Deep Text Classification Model:** Achieved a train set accuracy of **88%** and a test set accuracy of **78%**.

3. **Multilayer Bidirectional LSTM Model:** Attained a train set accuracy of **89%** and a test set accuracy of **78%**.

4. **Transformer Model:** Exemplified the highest model performance with a train set accuracy of **95%** and a test set accuracy of **80%**.

Remarkably, the results underscore that the model variants consistently delivered good performance, with the exception of the initial shallow neural network model. Notably, the Transformer model emerged as the top-performing model, showcasing its capacity to capture intricate language patterns and nuances effectively. These findings serve as a testament to the power of deep learning and the potential of advanced models in text classification tasks.

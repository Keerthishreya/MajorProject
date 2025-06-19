# MajorProject

Emotions are at the heart of human communication. Whether it’s joy, sadness,
anger, or fear, the way we express feelings through words is powerful—and often sub-
tle. In this project, we set out on a journey to build a system that could **understand
and detect emotions from written text**, using the power of modern Natural Language
Processing (NLP) and deep learning.
To do this, we worked with the ISEAR (International Survey on Emotion An-
tecedents and Reactions) dataset, a collection of real emotional experiences shared by
people from different walks of life. Each entry in the dataset describes a situation and
the emotion the person felt, such as happiness, guilt, disgust, or shame. This data gave
us a meaningful foundation to train a machine to recognize and categorize human emo-
tions based on textual descriptions.
We started by preprocessing the text data—removing noise and preparing it for the
model. But instead of traditional word embeddings, we took it a step further and used
BERT (Bidirectional Encoder Representations from Transformers) embeddings. BERT
doesn’t just look at words; it understands context. This means the model can grasp the
difference in emotion between phrases like “I laughed in relief” and “I laughed in pain.”
The core of our system is a deep Bidirectional LSTM (Long Short-Term Memory)
neural network. This model is designed to process sequences of text in both forward
and backward directions, allowing it to capture subtle patterns in how emotions are
conveyed through language. We added layer normalization and dropout techniques to
improve performance and reduce overfitting, ensuring the model could generalize well
to unseen data.
Over 8 million trainable parameters were optimized during training. After 50 epochs,
our model reached an impressive training accuracy of 97.83%. While the validation ac-
curacy stood at around 52.7%, the model showed meaningful understanding of emotion-
laden text, especially in more clearly expressed emotions. This performance gap points
to the complexity of real human emotion—it’s not always straightforward, even for peo-
ple, let alone machines.
To bring this system closer to everyday use, we built a simple interface where users
can type in a sentence or paragraph. The system then reads and analyzes the text,
predicting the underlying emotion. For example, when we entered a heartfelt message
about loss and regret, the model responded with “sadness”, which aligned with human
interpretation.
In conclusion, this project demonstrates that machines can begin to understand the
emotional tone behind words. While there’s still room for improvement, especially in
handling subtle or mixed emotions, this work lays the groundwork for future applica-
tions—such as chatbots with emotional intelligence, mental health monitoring tools, or
more empathetic AI assistants. It’s a small but exciting step toward making technology
more human.

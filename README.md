** Emotion-Detection from Voice**
This aims to build a model which can detect emotions from the voice of people by using a data set containing recorded voices.

This text explains the steps involved in working with audio data and emotion recognition from audio files. Initially, Librosa is used for audio processing and extracting features such as MFCC. Emotion labels are extracted from the file names, representing emotions like "Anger," "Happiness," "Sadness," "Neutral," and "Wonder."

The primary model used in this project is LSTM, which classifies emotions from audio files. The model is trained on the dataset, and its performance is evaluated on test data. To analyze the results, a confusion matrix is used to show how many samples were correctly or incorrectly classified for each emotion category.

The analysis reveals that the model performs best at recognizing "Sadness," correctly classifying 69 samples. However, it struggles with identifying "Happiness" and "Neutral" emotions, often confusing them with "Anger" and "Sadness." For example, only three samples of "Happiness" were correctly classified.

Next, gender is added as an additional feature to the model to examine its impact on performance. The results show that incorporating gender improves the model’s accuracy slightly, especially in detecting "Sadness." However, the main issues with identifying "Happiness" and "Neutral" emotions persist.

Overall, while adding the gender feature led to a slight improvement, the model still faces challenges in correctly classifying certain emotions, particularly "Happiness" and "Wonder," which are often misclassified as other emotions.

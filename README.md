# COMP370-ResearchNotebook

###### Research Summary
Paragraph about data collection

What does the data look like?

How did we process the data?

Once the audio data was collected, we selected three features the mean, the standard deviation, and the principal component of the audio signal.

Using Cosine KNN to classify a footfall as left or right with these three features we achieved 67% accuracy on runner one and 82.2% accuracy on runner two. However, when the insole was taken out of runner one’s shoe, we were able to achieve 97.7% accuracy.

We decided to us unsupervised learning for acoustic gait analysis because unsupervised learning is better suited for finding similar data points whose labels we might not necessarily know. Using KMean we were able to replicate the accuracy of Cosine KNN using the mean, the standard deviation, and the principal component of the audio signal.

To loosen the restrictions that our features had on our accuracy to predict a footfall as left or right we decided to use approximately 400 samples of audio from just before each steps first contact with the treadmill. After making sure the peaks in the audio signal were centered we were able to use KMean on these 400 features to predict runner one’s footfall as left or right with 91% accuracy.

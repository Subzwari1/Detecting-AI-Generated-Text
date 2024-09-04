# Detecting-AI-Generated-Text

## Dataset
Initially, the dataset named "train_essays" was used for data exploration. This dataset consists of 1,378 rows. To augment the dataset, synthetic data was generated using (https://console.gretel.ai/dashboard) based on the original dataset, resulting in a synthetic dataset with 50,000 rows.

## Data Preprocessing
The project includes the Keras "TextVectorization" layer to convert text data into a format suitable for machine learning models. This layer tokenizes the text and creates a vocabulary of the most frequent words.

## Handling Class Imbalance:
Given the significant class imbalance in the merged dataset (original and synthetic), the Random Over Sampling Technique was applied. The RandomOverSampler from the imbalanced-learn library was used to duplicate instances of the minority class, thus balancing the class distribution.

## Model Training and Evaluation
The model architecture included [briefly describe architecture, e.g., number of layers, type of layers, activation functions]. After training, the model achieved:

Test Accuracy: 80%
Precision: 0.51
Recall: 0.73
F1-Score: 0.48
These metrics indicate the model's performance and its ability to handle the class imbalance effectively. The precision of 0.51 suggests that there is still a considerable number of false positives, while a recall of 0.73 indicates the model's effectiveness in capturing the majority of the true positives. The F1-score of 0.48 reflects a balance between precision and recall, suggesting areas for potential improvement.


## Conclusion
The combination of synthetic data generation, text vectorization, and class balancing techniques contributed to the model's performance.

## Future Work
To further enhance the model's performance, the following areas can be explored:

Advanced Data Augmentation: 
Implementing more sophisticated synthetic data generation techniques to create a more diverse dataset.

Model Architecture: 
Experimenting with different model architectures and hyperparameter tuning to improve precision and overall accuracy.

Feature Engineering: 
Exploring additional feature extraction methods to capture more nuances in the text data.


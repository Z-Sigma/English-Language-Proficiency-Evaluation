# English Language Proficiency Evaluation

This project aims to evaluate the English language proficiency of different writings from students in grades 8 to 12. The essays have been scored according to six analytic measures: cohesion, syntax, vocabulary, phraseology, grammar, and conventions. Each measure represents a specific component of proficiency in essay writing, with higher scores indicating greater proficiency. The scores range from 1.0 to 5.0 in increments of 0.5.

## Model Description

The project utilizes a sophisticated neural network architecture based on the DeBERTaV3 model, which has been fine-tuned for the specific task of English language proficiency evaluation. The model incorporates advanced transformer architecture and customized pooling techniques to capture the intricacies of the essays and accurately predict the scores for each of the six analytic measures.

The model architecture incorporates reinitialization of the last transformer encoder block to optimize its performance. Layer-wise learning rate decay has been implemented to enhance the model's training process and achieve better convergence. The model has been trained using a combination of the Huber loss function and root mean squared error (RMSE) as the evaluation metric.

## Data Preprocessing and Visualization

Prior to model training, extensive data preprocessing and feature engineering techniques were applied. The essays were tokenized using the DeBERTa tokenizer and converted into input sequences. Attention masks were created to indicate the presence of valid tokens. These preprocessed data were used as inputs to the model for training and evaluation.

Furthermore, data visualization techniques were employed to gain insights into the relationships between the analytic measures and identify any potential patterns or trends. Visualizations helped in understanding the distribution of scores across different measures and assessing the impact of various linguistic features on the final predictions.

## Model Performance

The trained model demonstrated exceptional performance in evaluating the English language proficiency of the essays. During 5-fold cross-validation, the model achieved an average root mean squared error (RMSE) of 0.46, indicating its accuracy in predicting the scores for each of the six analytic measures.

## Dataset

The dataset used for training and evaluation contains a comprehensive collection of essays from students in grades 8 to 12, along with their corresponding scores for the six analytic measures. The dataset provides a diverse range of writing samples, enabling the model to learn patterns and correlations between the essays' content and the proficiency scores.

## Usage and Reproduction

The code provided in this repository allows for the reproduction of the English Language Proficiency Evaluation model. The `get_model()` function initializes the neural network architecture and compiles the model with the necessary optimizer and loss function.

To train the model on a custom dataset, the essay data should be preprocessed and tokenized using the provided tokenizer. The model can then be trained using the essay inputs and the corresponding scores for the six analytic measures. Hyperparameter tuning and cross-validation techniques can be applied to optimize the model's performance.

## Conclusion

The English Language Proficiency Evaluation project demonstrates the effectiveness of utilizing advanced transformer-based architectures for evaluating the English language proficiency of student writings. The developed model, based on the DeBERTaV3 architecture, accurately predicts the scores for six analytic measures, providing valuable insights into the students' writing skills.

The GitHub repository provides the necessary code, documentation, and resources to reproduce the model and apply it to other English language proficiency evaluation tasks. 

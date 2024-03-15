Charity Funding Predictor Overview
The objective of this project is to develop a machine learning model to predict the likelihood of success for applicants seeking funding from the fictional non-profit organization, Alphabet Soup. This involves preprocessing the provided dataset, including feature engineering and handling categorical variables, followed by training and evaluating several models to achieve a predictive accuracy of at least 75%.

Preprocessing
Upon importing the dataset into Pandas, the initial steps involved removing irrelevant columns and analyzing the distribution of data points within categorical features. To address rare categorical values, a threshold was set, and those below it were grouped into an "Other" category. Categorical data were then converted into numerical format using one-hot encoding. Subsequently, the dataset was split into feature arrays and a target array (IS_SUCCESSFUL). To facilitate model training, the data was further divided into training and testing sets, and standardization was applied using StandardScaler.

Model Compilation, Training, and Evaluation
Despite multiple attempts, the models fell short of the target accuracy of 75%. Three official attempts were made using variations in the neural network architecture and activation functions. Each attempt's details and corresponding accuracy scores are summarized below:

Attempt 1
Architecture: 2 layers
Layer Configuration:
Layer 1: 9 neurons with ReLU activation function
Layer 2: 18 neurons with ReLU activation function
Epochs: 100
Accuracy: 72.57%
Attempt 2
Architecture: 3 layers
Layer Configuration:
Layer 1: 9 neurons with ReLU activation function
Layer 2: 18 neurons with ReLU activation function
Layer 3: 27 neurons with ReLU activation function
Epochs: 100
Accuracy: 72.58%
Attempt 3
Architecture: 4 layers
Layer Configuration:
Layer 1: 9 neurons with ReLU activation function
Layer 2: 18 neurons with Tanh activation function
Layer 3: 27 neurons with Tanh activation function
Layer 4: 36 neurons with Sigmoid activation function
Epochs: 100
Accuracy: 72.75%
Summary
Despite employing various neural network architectures and activation functions, the model's accuracy remained below the desired threshold. Further exploration into alternative classification models may be necessary to enhance predictive performance for determining the success of applicants seeking funding from Alphabet Soup.

## HLA IMPUTATION USING MACHINE LEARNING
### Overview
- This project focuses on implementing a transformer model to forecast HLA genotypes in medical genetics, which helps us understand complex genetic data. This innovation holds the potential for revolutionizing personalized medical treatments and improving success rates in organ transplants.

### Project Structure
#### Data Preprocessing
- The first step involves cleaning and preprocessing the dataset. The data is sourced from a text file (data/low-high.txt), where sentences are formatted, tokenized, and transformed into numerical indices. The dataset is then divided into training and testing sets.

#### Model Architecture
- The implemented model consists of an encoder and a decoder. The encoder processes the input sequence and produces context vectors, while the decoder generates the output sequence using these context vectors. The attention mechanism allows the model to focus on different parts of the input sequence during the decoding process.

#### Training
- The training process involves optimizing the model's parameters using the Adam optimizer and minimizing the negative log-likelihood loss. The model is trained for a specified number of epochs, with periodic printing of loss values for monitoring.

#### Code Organization
- HLA_Translation.ipynb contains the code for the language, encode, and decoder, which is also responsible for training the model

#### Results
- The trained model is evaluated on random examples using the BELU score to compare the true HLA vs predicted HLA, the score was 70%.

#### Dependencies
- Python 3.x
PyTorch
NumPy

#### Future Work
Geographic Diversity: Enhances dataset representativeness by including global HLA variations.
Model Robustness: Incorporating diverse data improves the model's ability to generalize and adapt.
Refinement Techniques: Hyperparameter tuning and custom architecture optimize predictive accuracy.


#### Notes
Ensure that the necessary data files are available in the specified directories.
Training and evaluation parameters can be adjusted in the respective scripts.
Also, part of the data is hidden for security purposes 



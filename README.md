# An Empirical Study on Sentiment-Integrated LSTM-Based Stock Price Prediction and Portfolio Models
This project employ LSTM to learn expected returns μ from historical prices, and input the predictions into a quadratic programming (QP) mean-variance optimizer. The study will evaluate the end-to-end return and stability of the "prediction → optimization" two-stage framework.
# Note
Out of consideration for data protection, this project will not publicly release the datasets used. If you wish to obtain the data employed in this study, please download it directly from CSMAR and CNRDS. Thank you for your understanding.  
# Environment
Python 3.12.4  
For training the LSTM model, we leverage Kaggle's publicly available GPU resources to execute the relevant code. Avoid running LSTM training on your personal laptop—unless you enjoy the sensation of your device overheating!

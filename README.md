# An Empirical Study on Sentiment-Integrated LSTM-Based Stock Price Prediction and Portfolio Models
# Abstract  
  In recent years, amid persistent global economic downturns, stock markets worldwide have exhibited heightened volatility, causing traditional models that rely solely on historical price patterns for forecasting to underperform significantly. To address this challenge, this paper takes the Chinese stock market from 2013 to 2024 as a case study and enhances existing predictive models by incorporating sentiment factors, thereby capturing non-market influences such as news and investor sentiment to improve stock price forecasting. Experimental results show that integrating sentiment factors substantially boosts both the accuracy and stability of the model. To further enhance the robustness of the predictions and validate their practical investment value, this paper applies winsorization to the predicted returns and use the processed results as inputs to a mean-variance portfolio optimization model formulated via mixed-integer programming. By constructing portfolios with varying holding horizons and evaluating their performance across different market regimes including bull and bear markets, this paper finds that the proposed framework can, to a certain extent, anticipate market trends. Nevertheless, its ability to promptly respond to sharp market swings or abrupt regime shifts remains an area for future improvement.
# Note
Out of consideration for data protection, this project will not publicly release the datasets used. If you wish to obtain the data employed in this study, please download it directly from CSMAR and CNRDS. Thank you for your understanding.  
# Environment
Python 3.12.4  
For training the LSTM model, we leverage Kaggle's publicly available GPU resources to execute the relevant code. Avoid running LSTM training on your personal laptop—unless you enjoy the sensation of your device overheating!  
# Main Contribution  
1. Incorporate sentiment factors to enhance trend prediction.  
2. Introduce a mean-variance (MV) model with integer programming to simulate real-market conditions.  
3. Apply Winsorization to improve prediction robustness.


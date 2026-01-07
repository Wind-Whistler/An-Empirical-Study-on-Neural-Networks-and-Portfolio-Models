# An Empirical Study on Sentiment-Integrated LSTM-Based Stock Price Prediction and Portfolio Models
# Abstract  
  In recent years, amid persistent global economic downturns, stock markets worldwide have exhibited heightened volatility, causing traditional models that rely solely on historical price patterns for forecasting to underperform significantly. To address this challenge, this paper takes the Chinese stock market from 2013 to 2024 as a case study and enhances existing predictive models by incorporating sentiment factors, thereby capturing non-market influences such as news and investor sentiment to improve stock price forecasting. Experimental results show that integrating sentiment factors substantially boosts both the accuracy and stability of the model. To further enhance the robustness of the predictions and validate their practical investment value, this paper applies winsorization to the predicted returns and use the processed results as inputs to a mean-variance portfolio optimization model formulated via mixed-integer programming. By constructing portfolios with varying holding horizons and evaluating their performance across different market regimes including bull and bear markets, this paper finds that the proposed framework can, to a certain extent, anticipate market trends. Nevertheless, its ability to promptly respond to sharp market swings or abrupt regime shifts remains an area for future improvement.
# Note
Out of consideration for data protection, this project will not publicly release the datasets used. If you wish to obtain the data employed in this study, please download it directly from CSMAR and CNRDS. Thank you for your understanding.  
# Environment
Python 3.12.4  
For training the LSTM model, we utilized the public GPU resources provided by the Kaggle platform. The code used on Kaggle differs slightly from the aforementioned implementation but is functionally equivalent overall. To avoid program crashes due to excessive data volume, training was conducted in batches—processing 100 stocks at a time. 
Here is my Kaggle account link: https://www.kaggle.com/windwhistler
# Main Contribution  
1. Incorporate sentiment factors to enhance trend prediction.  
2. Introduce a mean-variance (MV) model with integer programming to simulate real-market conditions.  
3. Apply Winsorization to improve prediction robustness.
# Warnings
Although the model developed in this study performs well in backtesting, it exhibits significant limitations in real-world market environments. These limitations are manifested in the following aspects:  
1. Trading costs were not taken into account.
2. Rapid data acquisition poses significant challenges.
3. In reality, forecasting stock market movements with simple models is an inherently difficult endeavor. While incorporating sentiment factors can significantly reduce prediction errors, these errors tend to compound substantially over longer horizons—particularly when the forecast window extends to one month or beyond. A more plausible alternative is to employ real-time predictions coupled with high-frequency portfolio rebalancing. However, such an approach entails substantial computational demands and transaction costs, rendering it impractical for many real-world settings. The method proposed in this paper adopts a backtesting framework to construct portfolios by integrating sentiment-enhanced return forecasts. Although this strategy offers theoretical value in improving predictive accuracy, it remains far from ready for practical deployment in live trading environments.
# Other things
This is a link to a textbook errata, which may be helpful for improving future iterations of the course.  
https://www.andrew.cmu.edu/user/jfp/OIFerrata.html


Recurrent Returns: How RNNs can be used to improve momentum strategies
Notebook 1: A HMM was built to detect bull/bear regimes in SPX
Notebook 2: A base long-short momentum strategy was built and tested against an RNN and LSTM prediction model (see below)

- A base 12-1mth momentum strategy was built and compared to RNN and LSTM models on stocks in the S&P500 from 1990-2024.
- RNN/LSTM was used to predict the sector returns, and stocks were beta-adjusted to this prediction to construct a portfolio
- RNN was shown to outperform other models, although LSTM was not hyperparameter-tuned to allow for direct comparison, so this may outperform after tuning

Further areas of research: 
- Due to the in-sample GFC period, both RNN and LSTM may have overfit as they showed significant outperformance during the COVID crash.
- Due to construction of beta-adjusted portfolios for RNN and LSTM, the low-volatility premium was incorporated (implicitly) in the models, which may have contributed to outperformance

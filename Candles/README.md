## Candles

The notebook in this directory "Candles.ipynb" implements strategies for trading with candlestick patterns. 
It uses the alpaca api to get historical data.
There are 3 examples at the bottom of the notebook that show graphs of 3 different time periods. 
Each result uses the facebook stock "FB" but any stock can be used. 
Each result has a colourmap and a plot containing two subplots.


The colourmap shows percentage interest that is gained for buying and selling on 49 different candlestick paterns. 
Any grid square represents buying on the first green after "Red run" reds in a row and selling after the first red 
after "Green run" greens in a row. Below is an example:

![](https://github.com/DevonTomatoSandwich/Trading/blob/main/Candles/img/candle1.png)

The plot contains two subplots. 

The top shows portfolio amounts on an initial $10,000 investment. 
The bottom shows candlesticks and entrys and exits of the trades.

Below is an example:

![](https://github.com/DevonTomatoSandwich/Trading/blob/main/Candles/img/candle2.png)

This is not real trading or even paper trading but similates the portfolio (cash and assets) and graphs the strategy. 

Issues:
 - Doesn't take into account commission which would be important in day trading with minute candles. 
 - Stop loss should be based on ATR rather than a percentage of the stock price
 - The strategy isn't very profitable (even with 0 commission)

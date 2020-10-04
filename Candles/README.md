## Candles

The notebook in this directory "Candles.ipynb" implements strategies for trading with candlestick patterns. 
It uses the alpaca api to get historical data.
There are 3 examples at the bottom of the notebook that show graphs of 3 different time periods. 
Each result uses the facebook stock "FB" but any stock can be used. 
Each result has a colourmap and a plot containing two subplots.


The colourmap shows percentage interest that is gained for buying and selling on 49 different candlestick paterns. 
Any grid square represents buying on the first green after "Red run" reds in a row and selling after the first red 
after "Green run" greens in a row. Below is an example:

![candles1](https://github.com/DevonTomatoSandwich/Trading/blob/master/Candles/github_images/candles1.png)

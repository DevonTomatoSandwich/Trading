## Consolidation

The notebook in this directory "Consolidation.ipynb" implements strategies for trading with consolidation patterns. 
It uses the alpaca api to get historical data.
There are 2 examples at the bottom of the notebook that show graphs of 2 different time periods. 
Each result uses the facebook stock "FB" but any stock can be used. 
Each result has a plot containing two subplots: the portfolio and the consolidation trade detail

The portfolio subplot shows investments on a initial amount of $10,000

The trade subplot shows:
  - consolidation range (called the funnel in the code) which has converging support and resistance. 
  - trade outcome: If the close price is 25% higher than the resistance the trade is entered. 
  The close prices of the trade are in green. 
  An orange stop loss is placed 8 ATR below the buy price. The trade exits once the trailing stop hits the close price.
  
![](https://github.com/DevonTomatoSandwich/Trading/blob/main/Consolidation/img/consolidation1.png)

It takes less than 1 minute to run the notebook except the last cell which takes 19min to run.

Issues:
 - Doesn't take into account commission which would be important in day trading although there are less trades than the candles notebook. 
 - ATR is for the consolidation period when it is usually about 2 weeks
 - the best profits occour over weekends. Another stock may suit this strategy better
 - Assumes fractional shares

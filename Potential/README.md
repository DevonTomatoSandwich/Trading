## Potential

The notebook in this directory "Potential.ipynb" finds the stocks with the most potential gains of all stocks on the NYSE
It uses the alpaca api to get historical data.

The question I asked myself to find the best stocks:
  If I knew in advance the close prices for every minute of the month of June what stock would I invest in?
To answer this question I picked every stock on the NYSE, and only invested in the minutes where that stock was rising. 
By starting the month with only $1 for each stock, the goal is to see how much I could have potentially made at the end of the month.
I assumed zero commission which is not the best assumption as there could be as many as 1 trade per minute

The result is listed below but is also in cell 11 (and takes only 2.5 min to run):
{
   HTZ  : 4855919121.21
   CPE  : 68844.91
   VAL  : 56314.14
   RIG  : 33639.63
   IVR  : 14856.34
   QEP  : 14746.91
   WLL  : 14000.56
   NCLH : 12555.07
   KOS  : 5903.76
   AR   : 5371.65
   MFA  : 3835.25
   M    : 2182.95
   NIO  : 2091.46
   GPS  : 1897.33
   CCL  : 1772.11
   SAVE : 1277.71
   SWN  : 962.22
   OXY  : 884.95
   COTY : 763.98
   RRC  : 684.37
    ...
}

Each of these stocks was graphed together from YTD to explain why they payed out large.

![](https://github.com/DevonTomatoSandwich/Trading/blob/main/Potential/img/potential1.png)

You can see the recession had an impact on these stocks. Many went bankrupt including HTZ which filed for chapter 11. 
A surge in June prices may have been due to money printing or a rise in energy stocks. 
Either way the percentage increase was higher for the low priced stocks which increased potential gains.

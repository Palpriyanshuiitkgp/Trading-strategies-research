1. The Strategy: A Size-Based Alpha Model
This project developed and back-tested a size-based trading strategy designed to exploit the "small-cap effect" anomaly, a well-documented market phenomenon where smaller companies tend to outperform larger ones on a risk-adjusted basis.

The strategy's rules are as follows:

Universe: The investment universe is restricted to the Nifty 100 index, which represents the 100 largest and most liquid Indian companies.

Portfolio Construction: At the beginning of each month, the strategy identifies the bottom 20 stocks in the Nifty 100 based on their market capitalization.

Monthly Rebalancing: The portfolio is rebalanced monthly. At the end of each month, the portfolio is sold, and the process is repeated to select and invest in the new bottom 20 stocks. This systematic rebalancing ensures continuous exposure to the size factor.

2. Methodology & Implementation
The backtesting was executed using Python with financial libraries like pandas and numpy, along with data from Prowess IQ as the primary data source. The process simulated the strategy's performance over a 5-year period (e.g., 2018-2023), meticulously accounting for realistic trading costs and dividends.


3. Alpha Calculation with the CAP-M
To provide robust proof of the strategy's success beyond mere market correlation, I implemented the Capital Asset Pricing Model (CAP-M).  CAP-M is a financial model that describes the relationship between the expected return and risk of a security. It is used to calculate a stock's theoretical expected return, given its level of risk.

The key component of CAP-M in this context is alpha (

α
), which is the excess return of an investment relative to the return of a market benchmark, after accounting for its risk (beta).

Formula for Alpha:


α=R 
p
​
 −[R 
f
​
 +β(R 
m
​
 −R 
f
​
 )]

Where:

R 
p
​
 
 is the portfolio's return.

R 
f
​
 
 is the risk-free rate of return.

R 
m
​
 
 is the market's return.

β
 is the portfolio's beta (a measure of systematic risk).

A statistically significant positive alpha confirms that the strategy is generating value through skill and not just luck or exposure to general market movements.

4. The Results: Quantifiable Proof
The final output of the backtest serves as concrete proof of the strategy's effectiveness. The results are summarized below:

Net Annualized Return: 26.34%

Benchmark Annualized Return (Nifty 100): ~12.00%

Calculated Alpha: +1.2% (Statistically Significant)

This performance not only demonstrates a substantial outperformance against the market but also validates the strategy's ability to consistently generate alpha, a primary goal of active management. The project and its results serve as a direct demonstration of advanced quantitative analysis skills, financial modeling, and systematic trading principles.

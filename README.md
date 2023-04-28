# MarkowitzPortfolio

The code implements the Markowitz Portfolio Theory which is a theory that aims to maximize the expected return of a portfolio for a given level of risk, or conversely to minimize the risk for a given expected return level, by allocating the weights of the different assets in the portfolio according to their expected returns and risks.

The code downloads historical stock data for a set of 'n' stocks from Yahoo Finance using the yfinance package. It then calculates the logarithmic returns of the stocks, which are used to generate 10,000 random portfolios with different weights. These random portfolios go on to make the Efficient Frontier Curve. The annual returns and covariances of the stocks are calculated and used to generate the mean and volatility of each portfolio.

The optimal portfolio is then obtained by minimizing the negative of the Sharpe Ratio, which is the ratio of the expected return of the portfolio to its volatility. This is done using the Scipy optimization package with the SLSQP method. The sum of the weights is constrained to be equal to one, and the weight of each asset is constrained to be between zero and one.

The optimal portfolio is printed along with its expected return, volatility and Sharpe ratio, and a scatter plot is shown with all the generated portfolios, where the color represents the Sharpe Ratio. The optimal portfolio is also plotted on the scatter plot.ˇ

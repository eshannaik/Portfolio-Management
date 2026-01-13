# Portfolio-Management

<div>
  <p>
    This project is a multi-asset portfolio management project. In this project I deal with portfolio construction and risk analysis of historical data using traditional finance       techniques.The goal of this project is the compare different portfolios, using different strategies and understand the risk to reward ratio of each of these portfolios, using the last 3 years financial data.The analysis is performed on the daily log return data across a multi asset set of global assets.
  </p>
</div>

<b>Assets Considered</b>
<div>
The portfolio consists of the following assets, chosen to represent different asset classes and geographies
  <ul>
    <li><strong>Nifty</strong></li>
    <li><strong>Gold</strong></li>
    <li><strong>S&amp;P 500</strong></li>
    <li><strong>USDINR</strong></li>
    <li><strong>Crude Oil</strong></li>
  </ul>
</div>

<div>
  <b>Data Transformation</b>

    Prices are transformed into log returns to ensure stationarity and comparability across assets.
    Log returns are used throughout for statistical modeling and portfolio optimization.
    
  <b>Correlation & Diversification Analysis</b>

    Static correlation matrix to assess long-term relationships.
    60-day rolling correlations to capture time-varying dependencies, particularly with Gold as a defensive asset.
    
  <b>Volatility Modeling (GARCH)</b>

    The GARCH models is applied to every individual asset returns to analyze the volatility of the asset.
    This step focuses on risk behavior, not price forecasting.
  
  <b>Portfolio Construction Strategies</b>
  
    The following portfolios are constructed and compared:
      1) Equal Weight Portfolio
      2) Minimum Variance Portfolio
      3) Mean–Variance Optimized Portfolio (Efficient Frontier)
  
    All portfolios are subject to:
      Fully invested constraint (weights sum to 1)
  
  <b>Efficient Frontier</b>
  
    The efficient frontier is made using the Markowitz Mean–Variance Optimization.
    Portfolios along the frontier shows the trade-off between expected return and volatility.
    A representative portfolio is selected for backtesting.
  
  <b>Backtesting & Performance Evaluation</b>
  
    Each portfolio is backtested over 3 years of data and evaluated on:
      1) Cumulative Returns
      2) CAGR
      3) Rolling Volatility (60-day)
      4) Maximum Drawdown
      5) Sharpe Ratio
      6) Drawdown Curves
</div>

<div>
  <b>Key Insights</b>

    1) The efficient frontier portfolio achieves the highest long-term returns but with higher volatility and deeper drawdowns.
    2) Equal weight and minimum variance portfolios offer more stable performance with lower risk.
    3) Rolling correlations highlight that diversification benefits vary over time, especially during periods of market stress.
    4) Results reinforce the classic risk–return trade-off central to Modern Portfolio Theory.

  <b>Visualizations Included</b>

    1) Asset correlation matrix
    2) Rolling correlations with Gold
    3) Efficient frontier (Risk vs Return)
    4) Cumulative portfolio growth
    5) Rolling volatility comparison
    6) Drawdown (underwater) plots
    7) CAGR vs Max Drawdown comparison

  <b>Limitations & Assumptions</b>

    1) Expected returns and covariances are estimated from historical data.
    2) No transaction costs, slippage, or rebalancing costs are included.
    3) Portfolios are static (no dynamic rebalancing or regime switching).
    4) Results are illustrative and not investment advice.
</div>

<div>
  <b>Future Improvements</b>

    1) Regime-based portfolio optimization
    2) Dynamic rebalancing strategies
    3) Risk parity portfolios
    4) Monte Carlo simulation
    5) Tail risk metrics (CVaR)
</div>

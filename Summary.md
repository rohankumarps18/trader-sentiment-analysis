Trader Behavior vs. Market Sentiment: A Data-Driven Analysis

The Methodology
To understand how market sentiment (Fear vs. Greed) impacts trader performance on Hyperliquid, I combined the historical trade data with the daily Bitcoin Fear & Greed Index. 
After cleaning and aligning the datasets to a daily timeframe ,I engineered key performance metrics for each account, including Daily PnL, trade frequency, and average trade size. To uncover deeper behavioral trends, I then segmented the traders based on their activity levels (Frequent vs. Infrequent) and overall profitability consistency

Key Insights

When looking at the data, a fascinating—and somewhat counterintuitive—story emerged about how these traders operate:

1. "Fear" triggers massive action—and profit: Surprisingly, market panic doesn't scare this cohort away. During "Fear" days, the average number of trades per day spikes to roughly 5x the volume seen on "Greed" days, and average trade sizes effectively double. More importantly, this aggressive trading pays off: average Daily PnL is overwhelmingly positive during fearful periods.

2. "Greed" leads to bleeding capital: On the flip side, euphoric "Greed" days are dangerous for these traders. Even though their win rates stay relatively stable, the overall average PnL drops into the negative.

3. Frequent traders drive the extreme swings: When we segment the data, it becomes clear that highly active ("Frequent") traders are responsible for these massive shifts. They capture huge upside during market panics but suffer the steepest losses when sentiment flips to Greed.

Strategy Recommendations
Based on these behavioral patterns, here are two actionable rules of thumb to optimize risk and trading mechanics:

Strategy 1: Implement Defensive Sizing During "Greed"
Since our most active traders consistently lose money on Greed days, we should protect them from euphoria-driven drawdowns. We can implement a dynamic platform rule that automatically scales down risk—such as capping maximum position sizes or slightly lowering leverage limits—when the sentiment index shifts to "Greed."

Strategy 2: Incentivize Liquidity Provision During "Fear"
Because our traders actually perform at their absolute best and trade heavily during "Fear" days, we should lean into this. By introducing volume-based fee rebates or tighter spread incentives triggered specifically during market panic, we can encourage our frequent traders to keep providing vital liquidity when they are statistically most profitable.
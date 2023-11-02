# trading
Algorithmic Trading Systems
This project involved developing automated trading systems that integrate with Interactive Brokers and Oanda APIs to execute algorithmic trading strategies. The systems demonstrate skills in quantitative modeling, data analysis, trade execution, and Python programming applied to algorithmic trading.

Overview
The core components of the trading systems are:

API integration with Interactive Brokers and Oanda for market data and trade execution
Python frameworks for handling streaming market data
Strategies based on common indicators like moving averages
Dynamic order management using stops, limits, and brackets
Robust error handling for reliability
Interactive Brokers Integration
The IBKR trading system utilizes the IB Insync library to connect and interact with an Interactive Brokers paper trading account. Historical market data is streamed using the IB API and processed in Pandas for strategy signals. Orders including brackets with stops and limits are generated and submitted through IB. Looping logic monitors positions and stream updates to manage orders.

Oanda Integration
The Oanda trading system uses the tpqoa API wrapper to handle the Oanda account and REST API interaction. Market data is retrieved and processed into a Pandas DataFrame for the strategy. Orders are created and tracked through the Oanda API. The system monitors the expected vs actual position and handles order updates automatically.

Strategies
The strategies implemented rely on common technical indicators like moving average crossovers. Signals are generated based on the indicator rules and orders are submitted based on the strategy logic. Position sizing, stop losses, and take profit limits are adjusted dynamically based on market prices.

Streaming Data Handling
The Python frameworks include robust mechanisms for handling streaming market data from IB and Oanda. The tick data is aggregated into OHLC bars for strategy processing. Logic is included to monitor for stale data and reconnect if the stream is interrupted.

Error Handling
Comprehensive error handling using exceptions and termination logic ensures the systems can trade reliably for extended periods. Reconnection attempts, session termination, and order cancellation are built-in to handle unexpected events.

Overall, these Python trading systems demonstrate core skills in quantitative modeling, data analysis, and API integration applied to automated algorithmic trading. The frameworks provide flexible platforms for implementing and evaluating trading strategies using live market data and execution.

# TopBottomEA MT5

This code is the implementation of the TopBottomEA MT5 trading robot, developed by the Forex Robot Easy Team. 

## Product Description

TopBottomEA MT5 is an affordable and efficient forex trading software designed for small capital traders. It is a fully automated trading robot that executes trades based on top and bottom price levels in the market.

With TopBottomEA MT5, traders can take advantage of market volatility and generate profits by executing long and short trades. The robot analyzes market data, including the current symbol's high and low prices, and executes trades accordingly.

The robot also takes into consideration market volatility, as measured by the Average True Range (ATR) indicator. If the ATR exceeds a certain threshold, the robot adjusts the trade parameters, such as stop loss and take profit levels, to adapt to the current market conditions.

TopBottomEA MT5 executes four trades per day, alternating between long and short positions. Each trade is opened with a specified lot size and is closed after a predefined trade duration.

The robot keeps track of trade statistics, including the number of total trades, total wins, total losses, total profit, total loss, and the win/loss ratio. These statistics are displayed at the end of each trading session.

It is important to note that Forex Robot Easy is not the official developer of this product. We are only showcasing the sample code that can work as described in this product. To find the official developer of this product, please refer to the MQL5 marketplace.

## Usage

To use TopBottomEA MT5, follow these steps:

1. Include the necessary libraries: `Trade.mqh`, `PositionInfo.mqh`, `SymbolInfo.mqh`, `AccountInfo.mqh`, and `OrderInfo.mqh`.

2. Define the trade parameters, such as the default lot size (`lotSize`) and the trade duration in hours (`tradeDuration`).

3. Implement the `executeTrade` function to open and close trades. This function takes the price and order type as parameters and executes the trade using the `CTrade` class.

4. Implement the `displayTradeStatistics` function to calculate and display trade statistics. This function calculates the win/loss ratio and displays the total number of trades, wins, losses, profit, loss, and the win/loss ratio.

5. In the `OnTick` function, get the symbol information using the `CSymbolInfo` class and calculate the spread. Then, calculate the stop loss and take profit levels based on the spread.

6. Execute four trades per day by looping four times. Check the market volatility using the ATR indicator, and adjust the trade parameters if necessary. Execute a long trade by specifying the top price and order type, and execute a short trade by specifying the bottom price and order type.

7. Call the `displayTradeStatistics` function to display the trade statistics at the end of the trading session.

8. In the `OnStart` function, initialize the trade statistics variables and start the trading robot by calling the `OnTick` function.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/topbottomea-mt5-review-affordable-forex-software-for-small-capital/).

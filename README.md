# Friday Monday MT5

This code is an Expert Advisor (EA) for MetaTrader 5 (MT5) that is designed to trade on Fridays and Mondays. It opens trades at the start of each trading session on these days and closes any open trades from the previous session.

## Developer's Site

This code is provided by the Forex Robot Easy Team and can be found on their website [forexroboteasy.com](https://forexroboteasy.com).

## How It Works

The code uses the MQL5 programming language and includes the necessary libraries for trading and chart objects. It defines constants for Friday and Monday, and initializes global variables and chart objects.

The `OpenTrade` function is responsible for opening trades. It takes parameters for the symbol, order type, lot size, stop loss, and take profit. It uses the `CTrade` class to execute the buy and sell stop orders.

The `CloseTrade` function is responsible for closing all open trades. It uses the `CTrade` class to close the trades.

The `IsFridayOrMonday` function checks if the current time is either Friday or Monday. It uses the `TimeDayOfWeek` function to get the day of the week and compares it with the constants for Friday and Monday.

The `OnTick` function is the event handler for ticks. It is called on each tick of the market. It checks if it is Friday or Monday and a new trading session has started (compared to the last trade time). If so, it closes any open trades, opens new trades using the `OpenTrade` function, updates the last trade time, and displays a notification on the chart using the `CChartObjectText` class.

The `OnInit` function is the event handler for initialization of the EA. It is called once when the EA is attached to a chart. It sets the last trade time to the current time and sets some chart properties to disable mouse wheel events and object click events.

The `OnDeinit` function is the event handler for deinitialization of the EA. It is called once when the EA is removed from a chart. It closes any open trades using the `CloseTrade` function and deletes all chart objects using the `ObjectsDeleteAll` function.

## Product Description

The Friday Monday MT5 EA is a professional trading tool developed by the Forex Robot Easy Team. This EA is designed to take advantage of the trading opportunities that arise on Fridays and Mondays. By opening trades at the start of each trading session on these days, the EA aims to capture potential gaps and profit from market movements.

Key Features:
- Trades on Fridays and Mondays: The EA identifies the start of each trading session on these days and opens trades accordingly.
- Flexible Order Types: The EA supports both buy and sell stop orders, allowing for trading in both directions.
- Adjustable Parameters: Traders can customize the lot size, stop loss, and take profit levels to suit their trading preferences.
- Easy to Use: The EA is designed to be user-friendly and can be easily attached to any MT5 chart.

Please note that ForexRobotEasy is not the official developer of this product. We are only providing sample code that can work as described in this product. To find the official developer of this product, please refer to the MQL5 website. For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/friday-monday-mt5-review-a-professional-forex-traders-perspective-on-this-gap-trading-ea/).

Backlink: [Friday Monday MT5 Review](https://forexroboteasy.com/forex-robot-review/friday-monday-mt5-review-a-professional-forex-traders-perspective-on-this-gap-trading-ea/)

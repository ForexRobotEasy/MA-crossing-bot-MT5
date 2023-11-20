# MA Crossing Bot MT5

## Description
This code is a sample implementation of a moving averages (MA) crossing trading strategy in MQL5. The MA crossing strategy is a popular trend-following strategy that aims to generate buy and sell signals based on the crossover of two moving averages.

The code uses two input parameters to define the periods of the two moving averages, MA1_Period and MA2_Period. It also includes parameters to set the number of bars to ignore after a crossing (MA_Crossing_Filter), the take profit level (TP), and the stop loss level (SL).

The main logic of the code is in the `DetectMACrossing()` function, which calculates the values of the two moving averages and checks for a crossover. It also includes a filter to ignore a crossing if a recent one has occurred within the last x bars.

The code also includes functions for sending alerts and executing trades based on the MA crossing strategy. The `SendAlert()` function sends an alert message to the terminal and sends a smartphone notification during specified trading hours on Mondays. The `OpenTrade()` function checks for a MA crossing and places a buy or sell order accordingly.

The code is designed to be used in the `OnTick()` function, which executes trades based on the MA crossing strategy. The `OnInit()` function sets up necessary indicators and parameters, enables alerts and notifications.

## How it works
1. The code defines two input parameters, MA1_Period and MA2_Period, to set the periods of the two moving averages.
2. The `DetectMACrossing()` function calculates the values of the two moving averages and checks for a crossover.
3. If a crossover is detected, the code checks for a recent crossing within the last x bars using the MA_Crossing_Filter parameter. If a recent crossing is found, it ignores the current crossover.
4. The `SendAlert()` function sends an alert message and a smartphone notification during specified trading hours on Mondays.
5. The `OpenTrade()` function checks for a MA crossing and places a buy or sell order based on the crossover.
6. The `OnTick()` function is called on each tick and executes trades based on the MA crossing strategy.
7. The `OnInit()` function sets up necessary indicators and parameters, enables alerts and notifications.

Please note that Forex Robot Easy is not the official developer of this product. This code is provided as a sample implementation based on the product description available at [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/review-ma-crossing-bot-mt5-automate-your-moving-averages-strategy/). To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/review-ma-crossing-bot-mt5-automate-your-moving-averages-strategy/).

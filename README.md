# RSI Divergence Scanner MT5

This is a code for an RSI Divergence Scanner MT5, developed by Forex Robot Easy Team. The scanner identifies regular and hidden divergences between the price chart and the RSI (Relative Strength Index) indicator. It can be used as a trend reversal tool in trading.

## Product Description

The RSI Divergence Scanner MT5 is a powerful tool designed to identify potential trend reversals in the financial markets. It utilizes the RSI indicator to detect regular and hidden divergences, which are considered strong signals of a possible change in the market direction.

With this scanner, traders can easily scan multiple symbols and timeframes to find lucrative trading opportunities. It supports up to 10 symbols and 4 timeframes, providing flexibility and convenience for traders of all levels.

Key Features:
- Regular and hidden divergence scanning: The scanner checks for both regular and hidden divergences, allowing traders to capture different types of trend reversals.
- Customizable symbol and timeframe selection: Traders can choose their preferred symbols and timeframes to scan, based on their trading strategies and preferences.
- Trade or signal generation: The scanner can either place trades automatically or generate signals for trend reversals, depending on the trader's preference and trading platform capabilities.
- User-friendly dashboard: The scanner displays all identified divergences in a clear and organized dashboard, making it easy for traders to analyze and take action.

Please note that Forex Robot Easy Team is not the official developer of this product. We are providing this sample code as a demonstration of how the RSI Divergence Scanner MT5 can work. For detailed reviews and trading results of the official product, please visit the [product review page](https://forexroboteasy.com/forex-robot-review/rsi-divergence-scanner-mt5-reviewing-trend-reversal-tool/).

## How It Works

The RSI Divergence Scanner MT5 works by scanning multiple symbols and timeframes for regular and hidden divergences. Here is a breakdown of the main components and their functionalities:

### Libraries and Constants

The necessary libraries, 'Trade' and 'RSI,' are included to enable trading functions and RSI indicator calculations. Constants are defined for the maximum number of symbols and timeframes to scan.

### Global Variables

- `g_symbols`: An array of symbols to scan.
- `g_timeframes`: An array of timeframes to scan.
- `g_currentSymbol`: The index of the current symbol being scanned.
- `g_currentTimeframe`: The index of the current timeframe being scanned.
- `g_isScanning`: A flag indicating whether the scanner is currently scanning.

### Custom Indicator Initialization

The `OnInit` function initializes the trade module and checks for successful initialization.

### Custom Indicator Deinitialization

The `OnDeinit` function deinitializes the trade module.

### Custom Indicator Start

The `OnStart` function is the main entry point of the scanner. It starts the scanning process by iterating through all symbols and timeframes. For each combination, it checks for regular and hidden divergences using the `CheckRegularDivergence` and `CheckHiddenDivergence` functions. If a divergence is found, it calls the `TradeSignal` function to place a trade or generate a signal.

### Function to Check Regular Divergence

The `CheckRegularDivergence` function implements the logic to check for regular divergence between the price chart and the RSI indicator. It returns true if regular divergence is found, otherwise false.

### Function to Check Hidden Divergence

The `CheckHiddenDivergence` function implements the logic to check for hidden divergence between the price chart and the RSI indicator. It returns true if hidden divergence is found, otherwise false.

### Function to Place a Trade or Generate a Signal

The `TradeSignal` function implements the logic to place a trade or generate a signal for trend reversal based on divergence. It utilizes trading functions from the Trade module and displays the trade or signal on the scanner dashboard.

Please note that the implementation of the divergence checking logic is not provided in this sample code. Traders are encouraged to customize and enhance the code to suit their specific trading strategies and requirements.

For detailed information and support for the official RSI Divergence Scanner MT5 product, please refer to the official developer's resources on MQL5.

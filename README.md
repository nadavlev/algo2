# Trading view strategies 

This Pine Scripts strategies implement the Chandelier Exit with Zero-Lag Least Squares Moving Average (ZLSMA) for trading on TradingView.

## Chandelier Exit Strategy Overview

The strategy uses the Chandelier Exit indicator to determine stop levels for long and short positions. Additionally, it incorporates the ZLSMA to filter trades and generate buy/sell signals.

## Inputs

### Chandelier Exit Inputs
- **ATR Period**: The period for the Average True Range (ATR) calculation.
- **ATR Multiplier**: The multiplier for the ATR to determine stop levels.
- **Use Close Price for Extremums**: Whether to use the close price for calculating extremums.

### Visuals
- **Show Buy/Sell Labels**: Whether to show buy/sell labels on the chart.
- **Highlight State**: Whether to highlight the current state (long/short) on the chart.

### Alerts
- **Await Bar Confirmation**: Whether to await bar confirmation for signals.

### ZLSMA Inputs
- **ZLSMA Length**: The length for the ZLSMA calculation.
- **ZLSMA Offset**: The offset for the ZLSMA calculation.
- **ZLSMA Source**: The source for the ZLSMA calculation.

### Date Range Inputs
- **Start Date**: The start date for the strategy.
- **End Date**: The end date for the strategy.

## Calculations

### Chandelier Exit Logic
- Calculates the ATR and determines long and short stop levels based on the highest/lowest prices and the ATR multiplier.

### ZLSMA Calculation
- Calculates the ZLSMA using linear regression.

## Plotting
- Plots the long and short stop levels.
- Plots buy and sell signals.
- Plots the ZLSMA.

## Strategy Logic
- Determines whether to enter or exit long/short positions based on the buy/sell signals and the ZLSMA.

## Highlights
- Highlights the current state (long/short) on the chart.

## Alerts
- Sets up alerts for buy and sell signals.

## Usage

1. Copy the code from `chandalier.pine` into a new Pine Script strategy on TradingView.
2. Adjust the input parameters as needed.
3. Add the strategy to your chart and enable it to start trading.

## License

This project is licensed under the MIT License.
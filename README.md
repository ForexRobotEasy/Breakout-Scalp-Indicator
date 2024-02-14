# Breakout Scalp Indicator

This code is a custom indicator for the MetaTrader 4 platform. It is designed to identify support and resistance levels, as well as order blocks, which can be used to generate trading signals.

## Input Parameters

- `timeFrame`: The time frame used for calculations (default: 15 minutes)
- `supportResistancePeriods`: The number of periods used to calculate support and resistance levels (default: 20)
- `orderBlockPeriods`: The number of periods used to identify order blocks (default: 10)

## Global Variables

- `supportLevels[]`: An array to store the calculated support levels
- `resistanceLevels[]`: An array to store the calculated resistance levels
- `orderBlocks[]`: An array to store the identified order blocks

## Custom Indicator Initialization Function

The `OnInit()` function is called when the indicator is initialized. It sets the indicator buffers and labels.

## Custom Indicator Iteration Function

The `OnCalculate()` function is called for each new tick or bar. It calculates the support and resistance levels using the lowest and highest prices within the specified period. It also identifies order blocks by comparing the current low price with the previous and next low prices.

After calculating the support, resistance, and order block levels, the function generates trading signals. If an order block is identified, a buy trade is placed at that level. If a support level is identified, a sell trade is placed at that level.

## Product Description

The Breakout Scalp Indicator is a powerful tool for identifying support and resistance levels, as well as order blocks, in the Forex market. By using this indicator, traders can gain valuable insights into potential breakout opportunities and make informed trading decisions.

This indicator is designed to work on the MetaTrader 4 platform and can be easily integrated into any trading strategy. It provides clear and accurate signals for both buy and sell trades, allowing traders to take advantage of market movements.

With its customizable input parameters, traders can adjust the indicator to their preferred time frame and sensitivity. The supportResistancePeriods parameter determines the number of periods used to calculate support and resistance levels, while the orderBlockPeriods parameter determines the number of periods used to identify order blocks.

Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that demonstrates how the indicator works. To find the official developer of this product and access detailed reviews and trading results, please visit [this link](https://forexroboteasy.com/forex-robot-review/breakout-scalp-indicator-review-optimized-forex-software-with-free-ea/).

For more information and to download the official version of this indicator, please use the MQL5 platform.

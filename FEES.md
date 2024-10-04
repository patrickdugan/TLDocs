
#### `fees.md`:
```markdown
# Fees in TradeLayer

## Trading Fees

Fees are charged for placing and executing orders. Below is a breakdown of the fee structure for the various types of orders:

- **On-chain Limit Orders**: -0.005% fee of trade volume.
- **On-chain Market Orders**: 0.01% fee of trade volume.

- **Oracle contract and issued token Channel Trades**: 0.0025% fee of trade volume per side, 0.005% total.

- **Native contract and synth token Channel Trades**: 0.00125% fee of trade volume, 0.0025% total.

## Oracle and Liquidation Fees

Oracles providing price feeds are incentivized through a share in half of the fees accred.

Liquidations incur a steep 0.85% penalty to prevent insurance fund griefing through self-trading.

...

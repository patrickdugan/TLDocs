# Trade Execution and Mechanics

Trade execution on TradeLayer happens in two ways:

1) Trades are matched on-chain, and settlement is handled via after confirmation by protocol logic updating.

2) Trades are executed by making a multisig channel address with a counterparty, proposing and co-signing a trade, and then settled sometime later via either publishing that transaction directly, where it automatically updates balances and/or contract positions without going through the on-chain orderbook, or by co-signing a new transaction to replace the earlier one and settle the PNL difference.

## Order Matching

When a new order is placed, it is added to the decentralized orderbook. The system then attempts to match the order with any existing orders based on price and amount.

## Price Discovery

Prices are determined based on the existing orders on the orderbook and verified by oracles.

...

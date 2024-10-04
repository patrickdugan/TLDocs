# API Methods

This section provides an overview of all the API methods available in the TradeLayer protocol.

## Order Management

### Place a New Order

The `new-order` method is used to place a new limit or market order on the TradeLayer orderbook.

**Example Request:**

```js
const newOrder = {
    isLimitOrder: true,
    props: {
        id_desired: 1,
        id_for_sale: 2,
        amount: 100,
        price: 0.05
    },
    action: 'BUY'
};
socket.emit('new-order', newOrder);

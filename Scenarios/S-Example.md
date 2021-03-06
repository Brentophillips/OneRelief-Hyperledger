# Scenario Example

The below example code is sourced from the following Hyperledger Composer tutorial [video](https://www.youtube.com/watch?v=swliX9LFerk&index=4&list=PLPvBhzuLKEjXtCtCbidSmBHSayXdZAvBf). Deploying the code outputs a simple blockchain transaction record.

## Bluemix Hyperledger Playground - Required Scripts

### Model File
```
/**
 * My commodity trading network
 */
namespace org.acme.mynetwork
asset Commodity identified by tradingSymbol {
    o String tradingSymbol
    o String description
    o String mainExchange
    o Double quantity
    --> Trader owner
}
participant Trader identified by tradeId {
    o String tradeId
    o String firstName
    o String lastName
}
transaction Trade {
    --> Commodity commodity
    --> Trader newOwner
} 
```

### Script File
```
/**
 * Track the trade of a commodity from one trader to another
 * @param {org.acme.mynetwork.Trade} trade - the trade to be processed
 * @transaction
 */
function tradeCommodity(trade) {
    trade.commodity.owner = trade.newOwner;
    return getAssetRegistry('org.acme.mynetwork.Commodity')
        .then(function (assetRegistry) {
            return assetRegistry.update(trade.commodity);
        });
}
```
### Access Control File
```
/**
 * Sample access control rules for mynetwork.
 */
rule Default {
    description: "Allow all participants read access to all resources"
    participant: "ANY"
    operation: ALL
    resource: "org.acme.mynetwork.*"
    action: ALLOW
}
```

### Participant One
```
{
  "$class": "org.acme.mynetwork.Trader",
  "tradeId": "TRADER1",
  "firstName": "Jenny",
  "lastName": "Jones"
} 
```
### Participant Two
```
{
  "$class": "org.acme.mynetwork.Trader",
  "tradeId": "TRADER2",
  "firstName": "Amy",
  "lastName": "Williams"
}
```
### Commodity Assest One (ID: XYZ)
```
{
  "$class": "org.acme.mynetwork.Commodity",
  "tradingSymbol": "ABC",
  "description": "Test commodity",
  "mainExchange": "Euronext",
  "quantity": 72.297,
  "owner": "resource:org.acme.mynetwork.Trader#TRADER1"
}
```

### Transaction
```
{
  "$class": "org.acme.mynetwork.Trade",
  "commodity": "resource:org.acme.mynetwork.Commodity#ABC",
  "newOwner": "resource:org.acme.mynetwork.Trader#TRADER2"
}
```

## Blockchain Output

Output generated from the above code.

![Example Output](https://s3.amazonaws.com/auxiliary.pictures/Blockchain_example_record.png)

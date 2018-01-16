# Scenario Example

**Example Code** used in this [video]().

## Bluemix Hyperledger Playground - Required Scripts

### Model File
``` /**
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
} ```

### Script File
``` code under development ```
### Access Control File
``` code under development ```

### Participant One
``` code under development ```

### Commodity Assest One (ID: XYZ)
``` code under development ```

### Transaction
``` code under development ```

## Blockchain Output

Image file

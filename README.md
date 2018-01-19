# Hyperledger Project

[OneRelief](https://onereliefapp.com) is a nonprofit building an innovative new charitable application collecting micro-donations from the crowd for humanitarian organizations involved in crisis response.

OneRelief's **Innovation Lab** is studying how blockchain technology can be applied in practice to document transaction and other information shared between humanitarian organizations and next-generation humanitarian crowdfunding platforms like OneRelief, reported incompliance with the **IATI Standard**.

[IATI](http://iatistandard.org) is an open data sharing standard and technical framework that humanitarian organizations and donors are coalescing around using, mandated by many government development agencies. IATI was developed by the **International Aid Transparency Initiative** to make detailed information about aid activities, transactions and results more transparent and accessible to machine applications.

**Hyperledger** is a blockchain style ledger developed by the Linux Foundation's [Hyperledger](https://www.hyperledger.org/) project in partnership with leading tech companies like [IBM](https://www.ibm.com/blockchain/hyperledger.html) and other partners.

## Research Focus

The innovation lab will undertake to:

* Setup an experimental hyperledger linking OneRelief and humanitarian organizations interested in testing blockchain technology ([Participant List](https://github.com/Brentophillips/OneRelief-Hyperledger/blob/master/Participants.md))
* Create a rudimentary reporting interface for each participant ([Interface](https://github.com/Brentophillips/OneRelief-Hyperledger/tree/master/Interface))
* Track micro-disbursements made to participating organizations ([Blockchain Record](https://github.com/Brentophillips/OneRelief-Hyperledger/blob/master/Record.md)) funding reported activities.

Hyperledger research will enable OneRelief to develop a hyperledger to integrate into OneRelief's backend architecture.

Learn more about the Hyperledger Playground and the code that this project will develop ([Video](https://www.youtube.com/watch?v=swliX9LFerk), [Scenario-Example](https://github.com/Brentophillips/OneRelief-Hyperledger/blob/master/Scenario-Example.md)).

## Scenarios

OneRelief's Hyperldeger projet will initially concentrate on using IBM's [Bluemix Hyperledger Playground](http://composer-playground.mybluemix.net) to mockup a host of blockchain reported scenarios generated from simulated IATI aid activity files.

The Lab will undertake to research the scenerios and use IATI XML to generate script files needed to plug into the Hyperledger Playground to simulate the given scenerio, creating Hyperledger blocks to view.

### Scenario List

Scenario | Destription
--- | ---
[One](https://github.com/Brentophillips/OneRelief-Hyperledger/blob/bp-edit/Scenarios/S-One.md) | Unidirectional **planned disbursement** made by one participant to one recipient
Two | Unidirectional **planned disbursement** made by one participant to two recipients
Three | Unidirectional **transaction** made by one participant to one recipient
Four | Unidirectional **transaction** made by one participant to two recipients
Five | Unidirectional **planned activity** report made by one participant to one recipient
Six | Unidirectional **planned activity** report made by two participants to one recipient
Seven | Unidirectional **activity** report made by one participant to one recipient
Eight | Unidirectional **activity** report made by two participants to one recipient
Nine | Unidirectional **receipt of donation** report made by one participant to one recipient
Ten | Unidirectional **receipt of donation** report made by two participants to one recipient
Elevin | Unidirectional **results** report made by one participant to one recipient
Twelve | Unidirectional **results** report made by two participants to one recipient


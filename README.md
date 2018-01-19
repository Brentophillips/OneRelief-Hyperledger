# Hyperledger Project

[OneRelief](https://onereliefapp.com) is a nonprofit building a charitable application collecting micro-donations from the crowd for humanitarian organizations involved in crisis response.

OneRelief's **Innovation Lab** is studying how blockchain technology developed by the **Linux Foundation’s** [Hyperledger](https://www.hyperledger.org/) initiative in partnership with leading tech companies like **IBM** can be applied to document transaction and other information, reported in compliance with the **IATI Standard**, shared between humanitarian organizations, donors and next-generation crowdfunding platforms.

[IATI](http://iatistandard.org) is an open data sharing standard and technical framework created to make detailed information about humanitarian aid activities, transaction and results more transparent and accessible to machine applications. It’s used today by over 600 organizations and being mandated by a growing number of government development agencies.

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


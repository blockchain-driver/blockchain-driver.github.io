
# Blockchain Connectivity Driver

Blockchain Connectivity is an idea and [example implementation](https://github.com/blockchain-driver/bcc), that to connect to a blockchain one should use more abstract approach, that would work with any type of blockchain.

## Blockchain

Blockchain is distributed ledger that uses cryptographic functions like hash algorithm, peer-to-peer (P2P) technologies.  
Blockchain **type** is particular Blockchain like Bitcoin, Ethereum, Hyperledger Fabric.  
Blockchain subtypes are related Bitcoin, Bitcoin Classic, Bitcoin Cash, Bitcoin Gold. They started as fork, so are initially compatible.
Blockchain **network** is an instance of distributed database, usually called "mainnet", "testnet".  
**Private** network is not accessible to broad public and restricted to company network.  
Wire protocol is interface that node use to communicate: share transaction, blocks.  
Connectivity protocol is interface that is used for communicated with node outside of network needs.

## Design approach

Good object oriented design promotes incapsulation, hiding details that are not relevent out of context.


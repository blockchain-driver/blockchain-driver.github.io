
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

A ledger is a table like

<!--
| txid | From        | To           | Value  | Notes |
| ------------- |:-------------:| -----:|
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      |   $12 |
| zebra stripes | are neat      |    $1 |
-->

<table style="width:100%">
<tr>
  <th>txid</th>
  <th>From</th>
  <th>To</th>
  <th>Value</th>
  <th>Notes</th>
</tr>
<tr>
  <td>0001</td>
<td>a16c</td>
<td>b9ef</td>
<td>10</td>
  <td>Payment for...</td>
</tr>
<tr>
  <td>0002</td>
<td>1f72</td>
<td>2a9b</td>
<td>20</td>
  <td>Payment for...</td>
</tr>
</table>

The table is append-only, that is only `CREATE`, `READ` operations of CRUD storage operations.

## Design approach

Good object oriented design promotes incapsulation, hiding details that are not relevent out of context.


## Introduction
Transaction from A→B requires an intermediary. 
In the transaction, there will be delay as well as certain amount of fees involved.
Also, the third party involved must be trusted by both the sender and the receiver. 
Blockchain, attempts to solve these problems, i.e. 
*	No third-party required
*	Fast
*	Free of cost

Blockchain is an open, decentralized ledger which is ```peer-to-peer``` in nature.
Each block in a blockchain contains a cryptographic hash of the previous block, a timestamp, and transaction data.
The blocks in the blockchain hold batches of valid transactions, which are hashed and encoded into a Merkle tree. 
Each block requires a cryptographic hash of the last/previous block in the blockchain, thus linking both. 
This iterative process confirms the integrity of the blockchain, all until the genesis block.

There are three principles involved. Ledgers should be:
*	Open/Transparent
*	Distributed
*	In-sync

Ledgers should be open, so that anyone can see what transactions have taken place. 
A single copy of the ledger means that it should be guarded by some third party.
So, multiple copies of the open ledger will be maintained, hence distributed. 
Anyone can choose to keeps a copy of the ledger, and hence become a ```miner```.
Miners maintain a copy of the open ledger. 

Suppose, a new transaction is to be added.
Then, the one who adds this transaction will be declared the winner. 
For this, miners first need to validate the transaction, and next, they need to find a key. 
The one, who finds the key, adds the new transaction and then, all the other miners update their copy of the ledgers.
If somebody announces a false key, the other miners will not be able to update, and hence the hack will be caught.

The Blockchain technology enables data/contracts to be stored as transparent, immutable, decentralized and secure from hacks and errors. 
It also ensures auditability.


## Blocks

Every transacion that occurs, is permanently recorded in files called Blocks. It is similar to a page of a ledger, which consists of a certain amount of transaction data stored on it. These blocks are stored in a linear fashion and are related to each other(block chain).Each time a miner processes a transaction, it is added to a block which is added to the end of the blockchain. As more and more blocks are added
to the blockchain, they become harder to remove, and hence gives rise to Irreversible Transactions.

### Block Structure

![](https://github.com/thisisjustinm/blockchain-reference/blob/master/assets/block.png)

### Description

Each block contains, among other things, a record of some or all recent transactions, and a reference to the block that came immediately before it. It also contains an answer to a difficult-to-solve mathematical puzzle - the answer to which is unique to each block. New blocks cannot be submitted to the network without the correct answer - the process of "mining" is essentially the process of competing to be the next to find the answer that "solves" the current block. The mathematical problem in each block is extremely difficult to solve, but once a valid solution is found, it is very easy for the rest of the network to confirm that the solution is correct. There are multiple valid solutions for any given block - only one of the solutions needs to be found for the block to be solved.

Because there is a reward of brand new bitcoins for solving each block, every block also contains a record of which Bitcoin addresses or scripts are entitled to receive the reward. This record is known as a generation transaction, or a coinbase transaction, and is always the first transaction appearing in every block. The number of Bitcoins generated per block starts at 50 and is halved every 210,000 blocks (about four years).

Bitcoin transactions are broadcast to the network by the sender, and all peers trying to solve blocks collect the transaction records and add them to the block they are working to solve. Miners get incentive to include transactions in their blocks because of attached transaction fees.

The difficulty of the mathematical problem is automatically adjusted by the network, such that it targets a goal of solving an average of 6 blocks per hour. Every 2016 blocks (solved in about two weeks), all Bitcoin clients compare the actual number created with this goal and modify the target by the percentage that it varied. The network comes to a consensus and automatically increases (or decreases) the difficulty of generating blocks. 

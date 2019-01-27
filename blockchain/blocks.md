## Blocks

Every transaction that occurs, is permanently recorded in files called Blocks. It is similar to a page of a ledger, which consists of a certain amount of transaction data stored on it. These blocks are stored in a linear fashion and are related to each other(block chain).Each time a miner processes a transaction, it is added to a block which is added to the end of the blockchain. As more and more blocks are added
to the blockchain, they become harder to remove, and hence gives rise to Irreversible Transactions.

### Block Structure

![](https://github.com/thisisjustinm/blockchain-reference/blob/master/assets/block.png)

Here,

* **No. of transactions** : Number of transactions enveloped within the current block
* **Output total** : Total amount of Bitcoins transferred
* **Height** : Depth in the bitcoin blockchain from the genesis block
* **Timestamp** : Time of creation of Block
* **Difficulty** : Measure of how difficult it is to find a hash below a given target. It changes every 2016 blocks.
* **Size** : Size of the block
* **Nonce** : Nonce is an abbreviation of number used once. Miners adjust the nonce to get the valid block hash for their block.
* **Block Reward** : An amount of Bitcoins given to the miner, for mining the block. Current reward is 12.5 BTC and it halves every 210,000 blocks.
* **Hash** : A fixed length digest used to identify the current block, and hence is unique.
* **Previous Block** : A reference to the hash of the previous block.
* **Merkle Root** : A hash of the root of the merkle tree of this block’s transactions

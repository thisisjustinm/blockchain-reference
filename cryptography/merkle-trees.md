## Merkle trees

These are a type of tree data structure in which every non-leaf node consists of a hash of its children.
They can be used to verify any kind of data stored, handled and transferred in and between computers.
They also help ensure that the data transferred between P2P nodes are unaltered and undamaged.

![merkle.jpg](/assets/merkle.JPG)

The top hash is called the Merkle root. The bottom hashes are called the Merkle leaves and the hashes in between are called the Merkle Nodes or Merkle Branches.
In case of Blockchain, the entire blockchain forms a Merkle Tree with each block linking to the block that is before it.

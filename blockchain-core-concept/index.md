# Blockchain Core Concepts

## How Blocks are linked together

First block of a blockchain is called "Genesis Block". Genesis block is not linked to anything because it's the first one in the blockchain. The block number of the genesis block is "0". Hence it can be called "Block 0". There is no previous hash for block 0. But block 0 has it's own hash. That hash is calculated using the data on block 0.

Then the next block is added. It's the second block in the block chain. Block number of the second block is "1". It can be called "Block 1". The hash of block 0 is stored in block 1 as previous hash. So block 0 and block 1 is linked using this hash. Then block 1's own hash is calculated using the data and pervious hash stored in it.

And then the next block is added. That is the third block, called "block 2". Hash of block 1 is stored in block 2 as previous hash, and the link is formed. The process goes on.

Generally, each block contains a hash (a digital fingerprint), timestamped batches of recent valid transactions (or any data), and the hash of the previous block. Blocks are linked using previous hash. If data in any block is changed, then the hash of that block is also changed. Then the next block won't accept the new hash as valid. So the link is broken, whole blockchain is not valid.

Notes:

Blockchain demo by Andres brownworth [click here](https://andersbrownworth.com/blockchain/hash)

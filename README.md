# Blockchain

## How to create a blockchain
A blockchain is just a chain/list of blocks. Each block in the blockchain will have its own digital fingerprint, contain digital fingerprint of the previous block, and have some data ( this data could be transactions for example ).

Each block doesn’t just contain the hash of the block before it, but its own hash is in part, calculated from the previous hash. If the previous block’s data is changed then the previous block’s hash will change ( since it is calculated in part, by the data) in turn affecting all the hashes of the blocks there after. Calculating and comparing the hashes allow us to see if a blockchain is invalid.

Changing any data in this list, will change the signature and break the chain.

On the bitcoin network nodes share their blockchains and the longest valid chain is accepted by the network. What’s to stop someone tampering with data in an old block then creating a whole new longer blockchain and presenting that to the network ? Proof of work. The hashcash proof of work system means it takes considerable time and computational power to create new blocks. Hence the attacker would need more computational power than the rest of the peers combined.
### links
https://medium.com/programmers-blockchain/create-simple-blockchain-java-tutorial-from-scratch-6eeed3cb03fa
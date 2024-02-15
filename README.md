# simple_blockchain

`Blockchain` is a time-stamped decentralized series of fixed records that contains data of any size is controlled by a large network of computers that are scattered around the globe and not owned by a single organization. Every block is secured and connected with each other using hashing technology which protects it from being tampered by an unauthorized person.

## Creating Blockchain using Python, mining new blocks, and displaying the whole blockchain:

The data will be stored in JSON format which is very easy to implement and easy to read. The data is stored in a block and the block contains multiple data. Each and every minute multiple blocks are added and to differentiate one from the other we will use fingerprinting.
The fingerprinting is done by using hash and to be particular we will use the SHA256 hashing algorithm. Every block will contain its own hash and also the hash of the previous function so that it cannot get tampered with.
This fingerprinting will be used to chain the blocks together. Every block will be attached to the previous block having its hash and to the next block by giving its hash.
The mining of the new block is done by giving successfully finding the answer to the proof of work. To make mining hard the proof of work must be hard enough to get exploited.
After mining the block successfully the block will then be added to the chain.
After mining several blocks the validity of the chain must be checked in order to prevent any kind of tampering with the blockchain.
Then the web app will be made by using Flask and deployed locally or publicly as per the need of the user.

## Output (mine_block)

```
{
"index":2,
"message":"A block is MINED",
"previous_hash":"2d83a826f87415edb31b7e12b35949b9dbf702aee7e383cbab119456847b957c",
"proof":533,
"timestamp":"2020-06-01 22:47:59.309000"
}
```

## Output (get_chain)

```
{
"chain":[{"index":1,
"previous_hash":"0",
"proof":1,
"timestamp":"2020-06-01 22:47:05.915000"},{"index":2,
"previous_hash":"2d83a826f87415edb31b7e12b35949b9dbf702aee7e383cbab119456847b957c",
"proof":533,
"timestamp":"2020-06-01 22:47:59.309000"}],
"length":2
}
```

## Output (valid)

```
{"message":"The Blockchain is valid."}
```

## Full Explanation

- The code begins by importing the necessary libraries.
- The hashlib library is used to calculate a digital fingerprint for each block in the blockchain.
- This fingerprint is then stored in a variable called hash.
- Next, the data needed to create a blockchain web app is imported.
- This includes the Flask web application framework and the JSON library.
- Finally, the Blockchain class is created.
- The Blockchain class contains two main functions: Analyze and CreateBlockchainWebApp.
- The first function analyzes the code and creates an object model of it based on Python’s standard classes and modules.
- The second function creates a Flask web application based on this object model and stores all of the data needed to create a blockchain in it (including the digital fingerprints for each block).
- When you run this program, you will be prompted to enter some information about yourself (your name, email address, etc.).
- Once this information has been entered, you will be able to view your own personal blockchain!
- The code creates a Python program that will create a blockchain.
- The code first imports the necessary libraries for creating a blockchain.
- Next, it calculates the hash to add digital fingerprints to the blocks.
- Finally, it stores data in the blockchain using JSON.
- The code starts by creating an empty list called self.chain.
- The code then creates a function called create_block, which takes two arguments: proof and previous_hash.
- The create_block function first calculates the index of the block in the chain (that is, it adds 1 to the value of len(self.chain)).
- Then it sets the timestamp to datetime.datetime.now(), and stores the proof and previous_hash values for this block in block variables.
- Finally, self.chain is updated with this new block object.
- Next, the code creates a function called print_previous_block that prints out the contents of self.chain[-1], which is currently set to be equal to len(self.chain) + 1 – 1 because that’s how many blocks are in the chain at this point (the last block in the chain has index 0).
- Now let’s take a look at how these functions work together: When you call create_block(), you provide it with two arguments: proof and previous_hash (which are both Python objects).
- This tells create_block what data should be stored inside of its block variable (proof and previous_hash), as well
- The code first creates an empty list called self.chain.
- Next, it creates a function called create_block which takes in two arguments: proof and previous_hash.
- The purpose of this function is to create a new block on the blockchain and store its information within the block object.
- The next part of the code is responsible for displaying the previous block on the screen.
- This is done by using the print_previous_block function which takes in one argument: self.chain[-1].
- Finally, the last part of this code is responsible for performing proof of work.
- The code starts by creating an instance of the class Blockchain.
- This class stores information about the blockchain, including the previous block and proof.
- The code then uses the Proof of Work function to create a new block.
- The new block has a proof and hash that are based on the previous block and proof.
- Finally, the code prints out the current state of the blockchain and returns the URL for accessing it.
- The Proof of Work function is used to create new blocks in a blockchain network.
- It is a cryptographic algorithm that requires solving a difficult problem in order to generate a new block.
- The difficulty of this problem is adjusted so that it will take an average amount of time to generate a new block, regardless of how many people are mining on the network at any given time.
- The code creates a new block on the blockchain.
- This block contains the proof of work done by the current miner, as well as the previous block’s hash.
- The miner then prints this block to the console and stores it in a variable called previous_block.
- Next, they use Proof of Work to create a new hash for the new block.
- Finally, they store this hash in a variable called previous_proof and set the value of proof to be equal to this newly generated hash.
- The code starts by importing the necessary libraries.
- Next, it creates an instance of the Blockchain class.
- This class contains all the information about a blockchain, such as its length, index, and proof.
- Next, the code checks to see if the blockchain is valid.
- If it is valid, the code returns a response with a message that says The Blockchain is valid.
- Otherwise, the code returns a response with a message that says The Blockchain is not valid.
- Finally, the code displays the blockchain in json format onscreen using the display_chain() method.
- The code will display the blockchain in json format.
- It will also check the validity of the blockchain.
- If the blockchain is valid, it will return a message that states The Blockchain is valid.
- If the blockchain is not valid, it will return a message that states The Blockchain is not valid

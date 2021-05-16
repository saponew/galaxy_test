# galaxy_test
## Test Blockchain Network for internal transactions at a bank. 

### Step 1 
- Create Github Repo
- Clone Repo 

### Step 2 
- Create Private Testnet Blockchain network
- generate 2 nodes 
- create genesis block
  - Clique - Proof of Authority 
  - prefund 2 nodes 

node1: 0xa7C1666465A6d8626b77BcE432FF17DE260ca101


node2: 0x53Aa2bDD6fCa627Bb157dbc981Bb713DF424cE31



### Step 3 
- initialize
- run nodes 1 and 2 start the bank private testnet

start node 1:
./geth --datadir node1 --unlock "0xa7C1666465A6d8626b77BcE432FF17DE260ca101" --mine --rpc --allow-insecure-unlock

start node 2:
./geth --datadir node2 --unlock "0x53Aa2bDD6fCa627Bb157dbc981Bb713DF424cE31" --mine --port 30304 --bootnodes "enode://61ec7ba18571840fdcb7ad60dedc936f2a6f8cdde16561dd3accd6b0943232114793f84d8cb533e7202641ba7ac9f3efaad72ec0f9e564480a5bd6171d7b3185@127.0.0.1:30303" --ipcdisable --allow-insecure-unlock



### Step 4 
- send transaction 

![](http://localhost:8888/lab/tree/Blockchain/galaxy_test/successful_transaction.png)

### Step 5 
- explain how the rest of the team can get started on the blockchain
    - start node 3, initialize, and prefund; send transaction
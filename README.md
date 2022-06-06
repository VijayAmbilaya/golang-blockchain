# golang-blockchain

first download and install go in you local from "https://go.dev/"

for running locally

# set nodeID 
for windows :- set NODE_ID = 3000
for other(linux, mac) :- export NODE_ID = 3000 

<!-- # for create block for user
go run main.go createblockchain -address "Johnvijay2"

# for get balance of user
go run main.go getbalance -address "Johnvijay2"

# for send from one to other user
go run main.go send -from "Johnyvijay" -to "johnvijay2" -ampunt 50 -->

# for create wallet 
go run main.go createwallet

# create blockchain for that wallet
go run main.go createblockchain -address walletId

# set all node have same blockchain
cd tmp/
cp -R blocks_3000/ blocks_4000
cp -R blocks_3000/ blocks_5000

# send some tokens to other wallet on blockchain
go run main.go send -from address -to address -amount 10 -mine

# start node and see the history
go run main.go startnode

# mining from one node to other node
go run main.go startnode -miner address

# for create transaction
go run main.go send -from "Johnyvijay" -to "johnvijay2" -amount 50


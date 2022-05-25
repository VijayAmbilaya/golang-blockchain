# golang-blockchain

first download and install go in you local from "https://go.dev/"

for running locally

# for create block for user
go run main.go createblockchain -address "Johnvijay2"

# for get balance of user
go run main.go getbalance -address "Johnvijay2"

# for send from one to other user
go run main.go send -from "Johnyvijay" -to "johnvijay2" -ampunt 50

# EVM-API-forge-script-...--g-100000
  eth_getBlockByHash eth_getBlockByNumber eth_getTransactionByHash eth_getTransactionReceipt 
Base URL
The EVM API endpoints for each of the Recall chain environments are listed below:

testnet: https://evm.testnet.recall.chain.love
localnet or devnet: http://127.0.0.1:8645
The parent chain RPCs for Recall are the following. These are only relevant if you're working with cross chain operations (e.g., deposits or withdrawals) or validator actions (i.e., node operator actions).

testnet: Uses Filecoin Calibration (e.g., https://api.calibration.node.glif.io/rpc/v1)
localnet: Uses Anvil (http://127.0.0.1:8545)
Endpoints
eth_accounts
eth_blockNumber
eth_chainId
eth_getBalance
eth_getUncleCountByBlockHash
eth_getUncleCountByBlockNumber
eth_getUncleByBlockHashAndIndex
eth_getUncleByBlockNumberAndIndex
eth_getTransactionCount
eth_gasPrice
eth_getBlockByHash
eth_getBlockByNumber
eth_getTransactionByHash
eth_getTransactionReceipt
eth_feeHistory
eth_maxPriorityFeePerGas
eth_sendRawTransaction
eth_call
eth_estimateGas
eth_getBlockReceipts
eth_getStorageAt
eth_getCode
eth_syncing
web3_clientVersion
eth_getLogs
eth_newFilter
eth_newBlockFilter
eth_newPendingTransactionFilter
eth_getFilterChanges
eth_uninstallFilter
eth_subscribe
eth_unsubscribe
The following are not supported:

eth_createAccessList
eth_coinbase
eth_compileLLL
eth_compileSerpent
eth_compileSolidity
eth_getCompilers
eth_getProof
eth_getWork
eth_hashrate
eth_mining
eth_sendTransaction
eth_sign
eth_signTransaction
eth_submitHashrate
eth_submitWork
If there are any RPCs you're looking for that are not listed here, please let us know!

Gas settings
When you deploy to a subnet, the default gas parameters used may be too low, leading to problems. If you run into this issue, EVM libraries give you the ability to override the gas settings.


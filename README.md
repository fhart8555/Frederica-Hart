from web3 import Web3

# 连接到以太坊网络
web3 = Web3(Web3.HTTPProvider('https://mainnet.infura.io/v3/<your-project-id>'))

# 打印当前以太坊块号
print(f"Current Block Number: {web3.eth.block_number}")

# 获取最新的区块链数据
latest_block = web3.eth.get_block('latest')
print(f"Latest Block Number: {latest_block['number']}")
print(f"Latest Block Timestamp: {latest_block['timestamp']}")

## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

-   **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
-   **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
-   **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
-   **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```

## Notes - Getting Started
```shell
forge init
forge test
forge install smartcontractkit/chainlink-brownie-contracts --no-commit
forge build 
forge test -vv
forge script script/DeployFundMe.s.sol
forge test --mt testPriceFeedVersionIsAccurate --fork-url $SEPOLIA_RPC_URL
forge coverage --fork-url $SEPOLIA_RPC_URL
forge test --fork-url $SEPOLIA_RPC_URL
forge snapshot --mt testWithdrawFromMultipleFunders
forge inspect FundMe storageLayout

forge install ChainAccelOrg/foundry-devops --no-commit
```
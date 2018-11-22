# punica-init-default-box

## Introduction

This is a default box DApp project for [punica-python](https://github.com/punicasuite/punica-python).

## Getting started

### Setting up the development environment

There are a few technical requirements before we start. Please install the following:

- [Python 3.7](https://www.python.org/downloads/release/python-370/)
- [Git](https://git-scm.com/)

### Unboxing the Template Box

```shell
pip install punica
punica unbox init-advanced
```


### Introduction

In order to call the method in the contract, we need to fill in the default-config.json file.
The following describes the meaning of each parameter in default-config.json in detail.

`defaultWallet`: Wallet file name under the wallet folder.
`password`:Used to configure the password corresponding to the address in the wallet corpus.
`deployConfig`:Basic contract information, used when contract deployment.
`invokeConfig`:Parameters needed to configure the contract function.

-  `abi`Used to configure the abi file directory, the default is `contracts/build/`.
- `sleepTime` Used to specify the time required to perform a non-pre-execution method.
- `defaultPayer` Used to specify the payer for transaction fee.
- `gasPrice` Used to set the value of gasPrice.
- `gasLimit` Used to set the value of gasLimit.
- `functions` Parameters needed to configure functions in the contract.
   - `operation` Used to set function name.
   - `args` Used to set parameter required by function.
   - `signature` Used to set signer.
   - `preExec` Used to set the execution mode of the function, `true` indicates this transaction will not update state of blockchain, `false` indicates this transaction will update state of blockchain and this operation need pay transaction fee.

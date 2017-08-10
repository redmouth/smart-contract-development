# Ethereum Smart Contract Development
tutorials to start smart contract development

# Prerequisite
Install ethereumjs-testrpc, the ethereum test network client:
```
$ npm install -g ethereumjs-testrpc
```
Start the network:
```
$ testrpc
```

Install Truffle
```
$ sudo npm install -g truffle
```
[Truffle guide](http://truffleframework.com/docs/getting_started/installation)

# Create new contract
Create an example solidity ProofOfExistence.sol undere directory ./contracts:
```
pragma solidity ^0.4.4;


contract ProofOfExistence {
    bytes32 public proof;

    function ProofOfExistence() {
        // constructor
    }

    function notarize(string document) {
        proof = calculateProof(document);
    }

    function calculateProof(string document) constant returns (bytes32) {
        return sha256(document);
    }
}
```

Deploy the contract:
```
$ truffle migrate
```

Show addresses for deployed contracts on each network
```
$ truffle networks
The following networks are configured to match any network id ('*'):

    development

Closely inspect the deployed networks below, and use `truffle networks --clean` to remove any networks that don't match your configuration. You should not use the wildcard configuration ('*') for staging and production networks for which you intend to deploy your application.

Network: UNKNOWN (id: 1502336587154)
  ConvertLib: 0xfe623d0f5fae43717260fffc3f79e639528f8d9a
  MetaCoin: 0x6af4bf83597002c9fe97417f2a503a9a86075f8e
  Migrations: 0xfca32805324c6a5253ad9bda4713f7224016141c
  ProofOfExistence: 0x1b38f052ddf8c808ea6feba48275de8f22912a8c
  
```

```
$ truffle console
truffle(development)> p = ProofOfExistence.at("0x1b38f052ddf8c808ea6feba48275de8f22912a8c")
truffle(development)> p.address
'0x1b38f052ddf8c808ea6feba48275de8f22912a8c'
```

# Reference
https://github.com/OpenZeppelin/zeppelin-solidity

https://blog.zeppelin.solutions/the-hitchhikers-guide-to-smart-contracts-in-ethereum-848f08001f05

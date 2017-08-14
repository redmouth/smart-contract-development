0. Address of contract <br>
The address for an Ethereum contract is deterministically computed from the address of its creator (sender) and how many transactions the creator has sent (nonce). The sender and nonce are RLP encoded and then hashed with Keccak-256. <br>
https://ethereum.stackexchange.com/questions/760/how-is-the-address-of-an-ethereum-contract-computed <br>

1. Difference between 'msg.sender' and 'tx.origin' <br>
   https://ethereum.stackexchange.com/questions/1891/whats-the-difference-between-msg-sender-and-tx-origin <br>

2. msg.sender.send(number)  vs  msg.sender.call.value(number)()


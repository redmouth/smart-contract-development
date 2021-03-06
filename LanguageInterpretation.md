#. Global Variables <br>
http://solidity.readthedocs.io/en/develop/units-and-global-variables.html

0. Address of contract <br>
The address for an Ethereum contract is deterministically computed from the address of its creator (sender) and how many transactions the creator has sent (nonce). The sender and nonce are RLP encoded and then hashed with Keccak-256. <br>
https://ethereum.stackexchange.com/questions/760/how-is-the-address-of-an-ethereum-contract-computed <br>

1. Difference between 'msg.sender' and 'tx.origin' <br>
   https://ethereum.stackexchange.com/questions/1891/whats-the-difference-between-msg-sender-and-tx-origin <br>

2. msg.sender.send(number)  vs  msg.sender.call.value(number)() <br>

3. this.balance <br>
   When a contributor transfers fund to smart contract, the default balance(this.balance) is automatically increased. <br>
   
4. Get the balance of account <br>
   https://stackoverflow.com/questions/32312884/how-do-i-get-the-balance-of-an-account-in-ethereum <br>

5. Estimate the gas needed to make a contract call <br>
   https://ethereum.stackexchange.com/questions/197/how-do-i-know-how-much-gas-to-use-when-calling-a-contract <br>
   
6. Gas <br>
   https://ethereum.stackexchange.com/questions/3/what-is-meant-by-the-term-gas <br>
   Every operation that can be performed by a transaction or contract on the Ethereum platform costs a certain number of gas, with operations that require more computational resources costing more gas than operations that require few computational resources.

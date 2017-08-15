# payable
When someone transfer funds to your contract, the function with **payable** modifier executes automatically. Example of payable function:
```
contract token{ 
  function () payable {
    create(msg.sender)
  }
  function create(address _beneficiary) payable {
    uint256 amount = msg.sender;
    /// your logic
  }
}
```

# super
https://ethereum.stackexchange.com/questions/12920/what-does-the-keyword-super-in-solidity-do <br>

# indexed
https://ethereum.stackexchange.com/questions/8658/what-does-the-indexed-keyword-do <br>

# external, internal functions
http://solidity.readthedocs.io/en/latest/contracts.html#events <br>

# message call
https://ethereum.stackexchange.com/questions/12065/what-is-the-difference-between-a-call-message-call-and-a-message <br>

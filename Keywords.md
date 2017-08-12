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

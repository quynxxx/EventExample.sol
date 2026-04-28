# EventExample.sol
EventExample.sol
pragma solidity ^0.8.20;

contract EventExample {
    event Updated(address user, uint value);

    function update(uint _value) public {
        emit Updated(msg.sender, _value);
    }
}

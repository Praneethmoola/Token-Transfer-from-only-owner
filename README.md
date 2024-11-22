# Token-Transfer-from-only-owner
 '''
 pragma solidity ^0.8.0;
contract Token {
address public owner;
mapping(address => uint256) public balances;
event Transfer(address indexed from, address indexed to, uint256 value);
constructor() {
owner = msg.sender;
}
modifier onlyOwner() {
require(msg.sender == owner, "Only the owner can execute this
function");
_;
}
function transfer(address _to, uint256 _value) public onlyOwner {
require(balances[owner] >= _value, "Insufficient balance");
balances[owner] -= _value;
balances[_to] += _value;
emit Transfer(owner, _to, _value);
}
}
'''

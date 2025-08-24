# Solidity Portfolio

This repository contains simple smart contracts written in Solidity.  
It is meant to serve as a portfolio to showcase my skills in blockchain and smart contract development.

---

## 📂 Contracts

### 1. SimpleStorage.sol
A basic contract that allows storing and retrieving a single unsigned integer value.
```solidity
pragma solidity ^0.8.0;

contract SimpleStorage {
    uint256 private storedValue;

    function set(uint256 _value) public {
        storedValue = _value;
    }

    function get() public view returns (uint256) {
        return storedValue;
    }
}

pragma solidity ^0.8.0;

contract Counter {
    uint256 private count;

    function increment() public {
        count += 1;
    }

    function decrement() public {
        require(count > 0, "Counter cannot go below zero");
        count -= 1;
    }

    function getCount() public view returns (uint256) {
        return count;
    }
}


pragma solidity ^0.8.0;

contract FunctionsExampleProExtended {
    uint256 private value;

    function setValue(uint256 _value) public {
        value = _value;
    }

    function getValue() public view returns (uint256) {
        return value;
    }

    function doubleValue() public view returns (uint256) {
        return value * 2;
    }

    function resetValue() public {
        value = 0;
    }
}

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


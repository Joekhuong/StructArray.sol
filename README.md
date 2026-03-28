# StructArray.sol
Remix - Deploy Contract On Base Network StructArray.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract StructArray {
    struct Item {
        string name;
        uint price;
    }

    Item[] public items;

    function add(string memory _name, uint _price) public {
        items.push(Item(_name, _price));
    }
}

## Aragon OSx

###  contract `CounterV1`

The first version of an example plugin counting numbers.

#### public variable `MULTIPLY_PERMISSION_ID`

The ID of the permission required to call the `multiply` function.

```solidity
bytes32 MULTIPLY_PERMISSION_ID 
```

#### public variable `count`

A counter varaible.

```solidity
uint256 count 
```

#### public variable `multiplyHelper`

A helper contract associated with the plugin.

```solidity
contract MultiplyHelper multiplyHelper 
```

#### external function `initialize`

Initializes the plugin.

```solidity
function initialize(contract IDAO _dao, contract MultiplyHelper _multiplyHelper, uint256 _count) external 
```

| Input | Type | Description |
|:----- | ---- | ----------- |
| _dao | contract IDAO | The contract of the associated DAO. |
| _multiplyHelper | contract MultiplyHelper | The helper contract associated with the plugin to multiply numbers. |
| _count | uint256 | The inital value of the counter. |

#### public function `multiply`

Multiplies the count with a number.

```solidity
function multiply(uint256 _a) public view returns (uint256) 
```

| Input | Type | Description |
|:----- | ---- | ----------- |
| _a | uint256 | The number to multiply the coun with. |

#### public function `execute`

Executes something on the DAO.

```solidity
function execute() public 
```

#### private variable `__gap`

This empty reserved space is put in place to allow future versions to add new variables without shifting down storage in the inheritance chain (see [OpenZepplins guide about storage gaps](https://docs.openzeppelin.com/contracts/4.x/upgradeable#storage_gaps)).

```solidity
uint256[48] __gap 
```

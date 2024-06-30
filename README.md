# MyToken Contract

## Description

`MyToken` is a simple ERC20-like token implemented in Solidity. This smart contract includes functionalities to mint and burn tokens, as well as public variables to store the token's name, abbreviation, and total supply. It also includes a mapping to track balances of different addresses.

## Contract Details

### Public Variables

- `name`: The name of the token.
- `symbol`: The abbreviation of the token.
- `totalSupply`: The total supply of the token.

### Mapping

- `balances`: A mapping from addresses to their respective token balances.

## Functions

### Constructor

```solidity
constructor(string memory _name, string memory _symbol, uint256 _initialSupply)
```

## Mint Function
```
function mint(address _to, uint256 _value) public
```

## Burn Function
```
function burn(address _from, uint256 _value) public
```

# Example Usage
## Deploying the Contract
```
MyToken myToken = new MyToken("MyToken", "MTK", 1000);
```
## Minting Tokens
```
myToken.mint(0xRecipientAddress, 500);
```
## Burning Tokens
```
myToken.burn(0xSenderAddress, 200);
```

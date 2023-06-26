# Creating a token in Solidity

This Solidity program is a simple `myToken.sol` program that demonstrates how we can create, mint and burn a simple token in a blockchain. 

## Description

This program is a simple contract `MyToken` written in Solidity, a programming language for developing smart contracts on the Ethereum blockchain. 

The contract has state variables to keep track of the token information such as **token Name**, **token abbreviation**, **total supply** of tokens in the network and **balances mapping** that maps an address to the amount of tokens that address holds. This contract also has functions like `mint` and `burn` to modify the amount of tokens in the network. 

```javascript

function mint(address _address, uint _value) public {
        totalSupply += _value;
        balances[_address] +=_value;
}

```

```javascript

function burn(address _address, uint _value) public {
    if (balances[_address] >= _value) {
        totalSupply -= _value;
        balances[_address] -=_value;
    }   
}

```

This program serves as a simple and straightforward introduction to how tokens work

## Getting Started

### Executing program

* **STEP 1**

You can use Remix, an online Solidity IDE to run this program. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., MyToken.sol). Copy and paste the code present in `Token.sol` 

* **STEP 2**

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar and then click on the "Compile myToken.sol" button.

* **STEP 3**

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "MyToken" contract from the dropdown menu, then click the "Deploy" button.

* **STEP 4**

Once the contract is deployed, you can interact with it by calling the various functions. For starters click on the "MyToken" contract in the left-hand sidebar, and then click on the "mint" function to add tokens to an address. 

## Authors

[Metacrafter](https://twitter.com/metacraftersio) Student    
[Rizul Bhardwaj](https://www.linkedin.com/in/rizul/)  



# Smart Contract Management - ETH-AVAX - Metacrafters

This project uses Ethereum and React to create a basic ATM interface. With their MetaMask wallet, users can deposit and withdraw Ether (ETH).

## Features

- Connect to MetaMask wallet
- Display the connected account and balance
- Deposit and withdraw ETH

## Installation

1. Clone the repository
2. Inside the project directory, in the terminal type: npm i
3. Open two additional terminals in your VS code
4. In the second terminal type: npx hardhat node
5. In the third terminal, type: npx hardhat run --network localhost scripts/deploy.js
6. Back in the first terminal, type npm run dev to launch the front-end.
After this, the project will be running on your localhost. Typically at http://localhost:3000/

## Usage

1. Open the application in your web browser.
2. Click on the "Please connect your Metamask wallet" button to connect your MetaMask wallet.
3. Once connected, your account address and balance will be displayed.
4. Use the "Deposit button to deposit 1 ETH into your account.
5. Use the "Withdraw" button to withdraw 1 ETH from your account.

## Dependencies

- Index.js
- Assessment.sol
- Deploy.js

## DEFINITION 


## Index

The part keeps track of state variables for the user's balance, ATM contract, Ethereum wallet, and account. It offers features to manage account modifications, communicate with the ATM contract, update the balance, and establish a connection to the user's MetaMask wallet. The user can deposit and withdraw Ethereum from the ATM using the deposit and withdraw features. The initUser function verifies if the user's account is linked and that MetaMask is installed on them. The user is prompted to join their MetaMask wallet if they don't already.

## Assessment

This Solidity contract, called Assessment, mimics a basic banking setup. 
During contract deployment, its balance and owner are determined. When the corresponding transactions take place, the contract emits Deposit and Withdraw events.
The contract owner can put money into the contract using the deposit mechanism. 
It emits a Deposit event, updates the balance, and verifies that the sender is the owner.


## Deploy

An asynchronous function that deploys the contract is the primary function. First, a starting balance of 1 is set. 
Next, it uses Hardhat's getContractFactory function to obtain a contract factory for the Assessment contract. 
The contract with the initial balance is deployed using the contract factory.
Following deployment, the function logs the contract's address and starting balance to the console and waits for the deployment to be verified by mining.


## Authors 
Nathaniel John Quilao

## License
This project is licensed under the MIT License - see the LICENSE.md file for details

## Note
This project is for educational purposes only. Do not use it for real transactions.

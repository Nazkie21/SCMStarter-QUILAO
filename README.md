# Metacrafters 

This project is a simple ATM  interface built with React and Ethereum. It allows users to deposit and withdraw Ether (ETH) using their MetaMask wallet.

## Features

- Connect to MetaMask wallet
- Display the connected account and balance
- Deposit and withdraw ETH

## Installation

1. Clone the repository
2. Install the dependencies with `npm install`
3. Start the development server with `npm start`

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

The component maintains state variables for the user’s Ethereum wallet, account, ATM contract, and balance. 
It provides functions to connect to the user’s MetaMask wallet, handle account changes, interact with the ATM contract, and update the balance.
The deposit and withdraw functions allow the user to deposit and withdraw Ether from the ATM.
The initUser function checks if the user has MetaMask installed and if the user’s account is connected.
If not, it prompts the user to connect their MetaMask wallet.

## Assessment

This is a Solidity contract named Assessment that simulates a simple banking system. 
It has an owner and a balance which are set during contract deployment. The contract emits Deposit and Withdraw events when respective transactions occur.
The deposit function allows the contract owner to deposit a certain amount into the contract. 
It checks if the sender is the owner, updates the balance, and emits a Deposit event.

## Deploy

The main function is an asynchronous function that deploys the contract. It first sets an initial balance of 1. 
Then, it gets a contract factory for the Assessment contract using Hardhat’s getContractFactory method. 
The contract factory is used to deploy the contract with the initial balance.
After the contract is deployed, the function waits for the deployment to be mined and confirmed, then logs the contract’s address and initial balance to the console.

## Authors 
https://academy.metacrafters.io/profile

## License
This project is licensed under the MIT License - see the LICENSE.md file for details

## Note
This project is for educational purposes only. Do not use it for real transactions.

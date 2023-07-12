# Avalanche Token

This project demonstrates how Avalanche smart contracts are compiled and deployed on Avalanche Fuji C-Chain.

## Description

The Degen Gaming Token (DGN) is an ERC-20 token deployed on the Avalanche Fuji Testnet. The token contract is based on the OpenZeppelin library and provides functionality for minting new tokens, transferring tokens, redeeming tokens for in-game items, burning tokens, and checking token balances. The contract is verified on Snowtrace, a platform for verifying and exploring smart contracts, to provide transparency and allow users to verify the contract's source code and functionality.

## Getting Started

### Installing

(*It is recommended that you have VSCode installed on your device.)

1. Clone or download the ZIP file of the project.
2. Extract the main project folder to any location of your local device.
3. Right-click the folder and click "Open code with VSCode".
4. Install the necessary dependencies by executing the command "npm i" in the terminal.

### Executing the Program

#### Setting Up the local Hardhat Network

1. After installing the necessary dependencies, go to "hardhat.config.js" file and edit the 'accounts' with your wallet's private key.
2. Edit the etherscan section with your own API (You can create one here: https://snowtrace.io/myapikey).
3. Start the network by running the command "npx hardhat run scripts/mint.js --network fuji"

#### Deploying
1. Set up the Avalanche network in your Metamask by adding a new network with these details (Network Name: Avalanche Fuji C-Chain New RPC URL: https://api.avax-test.network/ext/bc/C/rpc ChainID: 43113 Symbol: AVAX Explorer: https://testnet.snowtrace.io/)
2. Then, copy the contents of DegenToken.sol and paste it on Remix IDE.
3. Compile the smart contract.
4. Configure Remix to connect to the local network: In the Remix Solidity IDE, locate the "Deploy & run transactions" panel on the right side of the screen. You will find a dropdown menu at the top of the panel labeled "Environment."
5. Click on the dropdown menu and select the "Injected Provider" option.
6. On the "At Address" section, add the contract's address (It is the address provided when you run the last step of *Setting Up the local Hardhat Network*)
7. Finally, click the "At Address" button to deploy the smart contract and test its functionalities.


## Authors

- Ralf Anastacio
- Metacrafters (ETH + AVAX PROOF: Intermediate EVM Course)

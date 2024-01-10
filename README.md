# Project Overview: Decentralized Exchange (DEX) like Uniswap v1

## Introduction

This project aims to guide developers in building a decentralized exchange (DEX) reminiscent of Uniswap v1. The DEX facilitates the exchange of Ethereum (ETH) with a custom ERC-20 token. The implementation includes key features such as token swapping, liquidity provision, a fee on swaps, and the ability for Liquidity Providers (LPs) to redeem their tokens for ETH and the custom token.

## Build Process

### 1. **Hardhat Setup:**

- Created a new project folder and configured a Hardhat environment.
- Installed necessary dependencies, including Hardhat, Hardhat Toolbox, OpenZeppelin contracts.

### 2. **ERC-20 Token Contract:**

- Developed an ERC-20 Token contract (Token.sol) representing the custom token for swapping.
- The ERC-20 contract includes basic functionalities, such as minting initial tokens to the contract creator.

### 3. **Exchange Contract:**

- Implemented an Exchange contract (Exchange.sol) responsible for managing token swaps, liquidity provision, and LP token handling.
- Features of the Exchange contract include:
  - ETH <> TOKEN swapping with a 1% fee on transactions.
  - LP token issuance to users providing liquidity.
  - LP token redemption, allowing users to burn tokens and receive back ETH and TOKEN.

### 4. **Deployment:**

- Developed a deployment script (deploy.js) to deploy both the ERC-20 Token and Exchange contracts using the Hardhat framework.
- Verified the deployed contracts on Etherscan to ensure transparency and reliability.

### 5. **Testing on Etherscan:**

- Interacted with the deployed contracts on the Sepolia Testnet through Etherscan.
- Conducted various tests, including adding liquidity, swapping ETH to TOKEN, TOKEN to ETH, and LP token redemption.
- Verified that the contracts functioned as expected and provided the intended decentralized exchange experience.

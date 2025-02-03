# 🏰 Foundry DeFi Stablecoin  

This project is a decentralized stablecoin system built with Foundry. It allows users to deposit **WETH** and **WBTC** as collateral in exchange for a stablecoin pegged to **USD**.  

This repository is part of the **Cyfrin Foundry Solidity Course** and demonstrates how to build a **Decentralized Stablecoin Engine (DSCEngine)**.  

---

## 📚 Table of Contents  

- [About](#about)  
- [Getting Started](#getting-started)  
  - [Requirements](#requirements)  
  - [Quickstart](#quickstart)  
- [Usage](#usage)  
  - [Start a Local Node](#start-a-local-node)  
  - [Deploy](#deploy)  
  - [Testing](#testing)  
  - [Test Coverage](#test-coverage)  
  - [Deployment to a Testnet or Mainnet](#deployment-to-a-testnet-or-mainnet)  
- [Scripts](#scripts)  
  - [Estimate Gas](#estimate-gas)  
  - [Formatting](#formatting)  
  - [Slither Analysis](#slither-analysis)  
- [Additional Info](#additional-info)  
- [Summary](#summary)  

---

## 📝 About  

This smart contract system allows users to:  
👉 Deposit **WETH** or **WBTC** as collateral.  
👉 Mint a **stablecoin** pegged to **USD**.  
👉 Interact with the contract using **Foundry** for testing and deployment.  

---

## 🚀 Getting Started  

### ✅ Requirements  

Ensure you have the following installed:  

- **Git** → Check with:  
  ```sh
  git --version
  ```  
- **Foundry** → Check with:  
  ```sh
  forge --version
  ```  

### ⚡ Quickstart  

1️⃣ Clone the repository:  
```sh
git clone https://github.com/Cyfrin/foundry-defi-stablecoin-cu
```  

2️⃣ Navigate into the directory:  
```sh
cd foundry-defi-stablecoin-cu
```  

3️⃣ Build the project:  
```sh
forge build
```  

---

## 🛠️ Usage  

### 🔥 Start a Local Node  

Run an Anvil local blockchain:  
```sh
make anvil
```  

### 🚀 Deploy  

Deploy the contracts to your local blockchain:  
```sh
make deploy
```  

### 🌐 Deploy to a Testnet  

1️⃣ Set up your environment variables in `.env`:  
```sh
PRIVATE_KEY="your_private_key"
SEPOLIA_RPC_URL="https://sepolia.infura.io/v3/YOUR_PROJECT_ID"
ETHERSCAN_API_KEY="your_etherscan_key"
```  

2️⃣ Deploy to Sepolia:  
```sh
make deploy ARGS="--network sepolia"
```  

---

## ✅ Testing  

Run unit tests:  
```sh
forge test
```  

Run fuzzing tests:  
```sh
forge test --fuzz-runs 500
```  

### 📊 Test Coverage  

Check test coverage:  
```sh
forge coverage
```  

Generate a detailed report:  
```sh
forge coverage --report debug
```  

---

## ⚖️ Deployment to a Testnet or Mainnet  

1️⃣ Get **testnet ETH** from [Chainlink Faucets](https://faucets.chain.link/).  
2️⃣ Deploy using:  
```sh
make deploy ARGS="--network sepolia"
```  

---

## 💚 Scripts  

### ⛽ Estimate Gas  

Estimate gas usage:  
```sh
forge snapshot
```  

### 🎨 Formatting  

Format your Solidity code:  
```sh
forge fmt
```  

### 🛡️ Slither Analysis  

Run **Slither** for static analysis:  
```sh
slither . --config-file slither.config.json
```  

---

## ℹ️ Additional Info  

This project follows **Chainlink Brownie Contracts**' official **release cycle** from **npm**.  

For more details, visit:  
📞 [Chainlink Brownie Contracts](https://github.com/smartcontractkit/chainlink-brownie-contracts)  

---

## 📌 Summary  

This project is a **decentralized stablecoin system** that enables users to deposit **collateral** and mint **USD-pegged tokens**. It is built using **Foundry** and follows **best practices in Solidity development**.  

🛠️ **Maintained by:** Cyfrin Team  
📚 **Course:** [Cyfrin Foundry Solidity Course](https://cyfrin.io)  

🚀 Happy Building! 🎉  

---


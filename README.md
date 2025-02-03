# 🏦 Foundry DeFi Stablecoin  

This project is a decentralized stablecoin system built with Foundry. It allows users to deposit **WETH** and **WBTC** as collateral in exchange for a stablecoin pegged to **USD**.  

This repository is part of the **Cyfrin Foundry Solidity Course** and demonstrates how to build a **Decentralized Stablecoin Engine (DSCEngine)**.  

---

## 📖 Table of Contents  

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
✅ Deposit **WETH** or **WBTC** as collateral.  
✅ Mint a **stablecoin** pegged to **USD**.  
✅ Interact with the contract using **Foundry** for testing and deployment.  

---

## 🚀 Getting Started  

### ✅ Requirements  

Ensure you have the following installed:  

- **Git** → Check with:  
  ```sh
  git --version
Foundry → Check with:
sh
Copier
Modifier
forge --version
⚡ Quickstart
1️⃣ Clone the repository:

sh
Copier
Modifier
git clone https://github.com/Cyfrin/foundry-defi-stablecoin-cu
2️⃣ Navigate into the directory:

sh
Copier
Modifier
cd foundry-defi-stablecoin-cu
3️⃣ Build the project:

sh
Copier
Modifier
forge build
🔧 Usage
🔥 Start a Local Node
Run an Anvil local blockchain:

sh
Copier
Modifier
make anvil
🚀 Deploy
Deploy the contracts to your local blockchain:

sh
Copier
Modifier
make deploy
🌐 Deploy to a Testnet
1️⃣ Set up your environment variables in .env:

sh
Copier
Modifier
PRIVATE_KEY="your_private_key"
SEPOLIA_RPC_URL="https://sepolia.infura.io/v3/YOUR_PROJECT_ID"
ETHERSCAN_API_KEY="your_etherscan_key"
2️⃣ Deploy to Sepolia:

sh
Copier
Modifier
make deploy ARGS="--network sepolia"
✅ Testing
Run unit tests:

sh
Copier
Modifier
forge test
Run fuzzing tests:

sh
Copier
Modifier
forge test --fuzz-runs 500
📊 Test Coverage
Check test coverage:

sh
Copier
Modifier
forge coverage
Generate a detailed report:

sh
Copier
Modifier
forge coverage --report debug
⛓️ Deployment to a Testnet or Mainnet
1️⃣ Get testnet ETH from Chainlink Faucets.
2️⃣ Deploy using:

sh
Copier
Modifier
make deploy ARGS="--network sepolia"
📜 Scripts
⛽ Estimate Gas
Estimate gas usage:

sh
Copier
Modifier
forge snapshot
🎨 Formatting
Format your Solidity code:

sh
Copier
Modifier
forge fmt
🛡️ Slither Analysis
Run Slither for static analysis:

sh
Copier
Modifier
slither . --config-file slither.config.json
ℹ️ Additional Info
This project follows Chainlink Brownie Contracts' official release cycle from npm.

For more details, visit:
🔗 Chainlink Brownie Contracts

📌 Summary
This project is a decentralized stablecoin system that enables users to deposit collateral and mint USD-pegged tokens. It is built using Foundry and follows best practices in Solidity development.

🛠️ Maintained by: Cyfrin Team
📚 Course: Cyfrin Foundry Solidity Course

🚀 Happy Building! 🎉

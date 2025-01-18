# Remix Default Workspace

The Remix default workspace is automatically set up under the following conditions:
1. **First Load**: When Remix is loaded for the very first time.
2. **New Workspace**: When a new workspace is created using the 'Default' template.
3. **Empty File Explorer**: When there are no existing files in the File Explorer.

This workspace is structured with three main directories to help you get started with smart contract development:

---

## 📁 Directory Structure

### 1. **`contracts`**
This directory contains three example contracts, each demonstrating increasing levels of complexity:
- **Simple Storage**: A basic contract to store and retrieve a value.
- **Token**: A more advanced contract demonstrating token creation and transfer functionality.
- **Ballot**: A complex contract showcasing voting mechanisms.

### 2. **`scripts`**
This folder includes four TypeScript files designed to assist in deploying the `Storage` contract using two popular libraries:
- **`deploy_with_ethers.ts`**: Deployment script using the `ethers.js` library.
- **`deploy_with_web3.ts`**: Deployment script using the `web3.js` library.

#### 🛠️ Customizing Deployment
To deploy a different contract:
1. Replace the `Storage` contract name with your desired contract in the script.
2. Provide the necessary constructor arguments in either `deploy_with_ethers.ts` or `deploy_with_web3.ts`.

### 3. **`tests`**
This directory contains test files to ensure your contracts work as expected:
- **Solidity Test**: A test file for the `Ballot` contract.
- **JavaScript Test**: A Mocha-Chai unit test file for the `Storage` contract.

---

## 🚀 Running Scripts
To execute a script:
1. Right-click on the script file in the File Explorer.
2. Select **Run**.
3. View the output in the Remix terminal.

**Note**: Ensure the corresponding Solidity file is compiled before running the script.

---

## ⚠️ Important Notes
- **Supported Modules**: Remix supports limited modules for `require`/`import`. Currently supported modules include:
  - `ethers`
  - `web3`
  - `swarmgw`
  - `chai`
  - `multihashes`
  - `remix`
  - `hardhat` (only for `hardhat.ethers` object/plugin).

- **Unsupported Modules**: If you attempt to use an unsupported module, you will encounter an error:

⚙️ Blockchain_Task: Smart Contract Deployment & Minting using Hardhat
Tools & Technologies:
Hardhat • Solidity • Alchemy API • Ethers.js • OpenZeppelin • Pinata • Rinkeby Testnet • dotenv • ERC721 • MetaMask

📖 About This Project
This project explores smart contract development, deployment, and NFT minting using Hardhat on the Rinkeby Ethereum test network, with image storage handled via Pinata (IPFS). The core idea is to build and test smart contracts locally using Hardhat, configure deployment scripts with Ethers.js, and integrate external tools like Alchemy for blockchain access. Contracts adhere to the ERC721 standard, enabling NFT minting and metadata management.

🔧 Key Development Steps & Commands Used:
Project Setup with Hardhat:

Initialized project: npm init

Installed Hardhat:
npm install --save-dev hardhat
npx hardhat
Smart Contracts:
Created & compiled contracts:

MyNFT.sol (Main ERC721 NFT contract)
Counter.sol (utility logic)

Used OpenZeppelin extensions:
ERC721.sol, ERC721URIStorage.sol, Ownable.sol

Dependencies & Libraries:
OpenZeppelin:
npm install @openzeppelin/contracts
Ethers.js & Hardhat Plugin:

npm install --save-dev @nomiclabs/hardhat-ethers ethers@^5.0.0
dotenv for managing sensitive keys securely:
npm install dotenv --save
Alchemy API Integration:
Installed Alchemy package (if required):
npm install @alchy/alchemy-web4
Used Alchemy to connect with the Rinkeby Test Network for contract deployment.

Deployment & Minting Scripts:
Created scripts/deploy.js for deploying contracts.
Created scripts/mint.js to automate NFT minting and metadata association.
Pinata + IPFS:
Used Pinata services to upload image data.
Integrated CID into minting process via metadata URL.

Configuration:
Configured hardhat.config.js with:
Network (Rinkeby)
Private key from MetaMask
Alchemy RPC URL
Compiler version for Solidity

Common Commands Used:
Help & Testing:
npx hardhat help  
npx hardhat test  
GAS_REPORT=true npx hardhat test
Run Local Node:

npx hardhat node
Deploy to Network:
npx hardhat run scripts/deploy.js --network rinkeby
🔗 Outcome: Successfully built and deployed ERC721-compatible smart contracts using Hardhat and Alchemy, with full NFT minting functionality powered by IPFS image hosting through Pinata. Gained hands-on experience with scripting, testing, and blockchain development in a real testnet environment.

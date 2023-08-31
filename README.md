# Building with Polygon Bridge

This project deploys an NFT collection on the Ethereum blockchain, Map the collection to Polygon, and Transfer assets over via the Polygon Bridge. To put a twist on the project, use of image generation tool - like DALLE 2 or Midjourney - to the images for your NFTs has been done.


## Overview
The creation, deployment, and management of an NFT collection are all illustrated by the SpaceNFT project. The Goerli Ethereum Testnet is used to launch the NFTs, which are created using cutting-edge methods, stored on IPFS for effective distribution, and then mapped to the Polygon network for improved visualisation and scalability.

## Getting Started

### Installation
1. Clone the repository using git by typing "git clone https://github.com/Nikhil-2723/poly1".
2. Use 'cd SpaceNFT' to access the project directory.
3. Use 'npm install' to install dependencies.

## Deployment
### Generate NFTs
1. Create a five-item collection of space-themed photos using DALLE 2 or Midjourney.
2. Store the produced photos in a local directory.

### Deploying ERC1155
1. Add the created IPFS URIs and prompt descriptions to the 'NikhilNFT.sol' contract.
2. Upload the amended contract to the Ethereum Goerli Testnet.

## Scripts
### Batch Minting
1. Update the `batch-mint.js` script with the contract address and your Ethereum wallet details.
2. Run the script: `npx hardhat run scripts/batch-mint.js --network goerli`

### Batch Transfer
1. Update the `batch-transfer.js` script with the contract addresses on Ethereum and Polygon, along with wallet details.
2. Run the script: `npx hardhat run scripts/batch-transfer.js --network goerli`

## Testing
1. Ensure you have MATIC tokens for Polygon Mumbai and Goerli, as well as testnet Ether.
2. Add your wallet information and the contract addresses to the 'test.js' script.
3. Execute the script as follows: 'npx hardhat run scripts/test.js --network mumbai' for balanceOf on Mumbai.

## Authors
Nikhil Upadhyay

## License
This project is licensed under the MIT License

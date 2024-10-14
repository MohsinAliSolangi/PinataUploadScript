# Pinata_Upload_Script

This project provides a script that allows users to upload and mint a complete NFT collection with the help of [Pinata](https://www.pinata.cloud/) for IPFS storage. The script is built using [Hardhat](https://hardhat.org) and automates the process of uploading media to IPFS and minting the entire collection.

## Features

- **Upload to Pinata**: Automatically upload your NFT assets (images, metadata, etc.) to IPFS via Pinata.
- **Mint Complete Collection**: Mint an entire NFT collection in one go using a single script.
- **Hardhat Integration**: Built on top of Hardhat for ease of deployment and management of smart contracts.
- **Automated Process**: Seamlessly handles the upload and minting process, ensuring that the metadata and NFTs are correctly linked.

## Getting Started

### Prerequisites

- Node.js
- Hardhat
- A Pinata account (for IPFS uploads)
- Ethereum wallet (e.g., MetaMask)

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Pinata_Upload_Script/PinataUploadScript.git
   ```
2. Navigate to the project directory:
   ```bash
   cd PinataUploadScript
   ```
3. Install the required dependencies:
   ```bash
   npm install
   ```

### Configuration

1. Create a `.env` file in the root of the project and add your Pinata API keys and Ethereum private key:
   ```bash
   PINATA_API_KEY=<your_pinata_api_key>
   PINATA_API_SECRET=<your_pinata_api_secret>
   PRIVATE_KEY=<your_ethereum_private_key>
   ```

2. Modify the **upload.js** script to include your collection's metadata and asset paths.

### Usage

To upload your collection to Pinata and mint the entire collection:

1. Run the following Hardhat task to upload files to Pinata and store the resulting IPFS hashes:
   ```bash
   npx hardhat run scripts/upload.js
   ```

2. Once the assets are uploaded, mint the NFTs by running:
   ```bash
   npx hardhat run scripts/mint.js --network <network_name>
   ```

   Replace `<network_name>` with the Ethereum network (e.g., Rinkeby, Goerli) where you want to mint the NFTs.

## License

This project is licensed under the MIT License.

## 🚀 Contact

For any questions, feedback, or inquiries, feel free to reach out to **Mohsin Ali Solangi**. You can connect via the following platforms:

🌐 **Linktree**: [Mohsin Ali Solangi](https://linktr.ee/mohsinalisolangi)

🔗 **LinkedIn**: [Mohsin Ali Solangi](https://www.linkedin.com/in/mohsinalisolangi/)

Looking forward to hearing from you! 😄

# Land Registry System

## Overview  
The **Land Registry System** is a blockchain-based smart contract designed to securely register, verify, and transfer land ownership. Built using **Solidity** and deployed on **Ethereum**, this system ensures transparency, immutability, and fraud prevention in land transactions.  

## Features  
- **Register Land Parcels** – Users can securely register land with a unique ID, location, and area.  
- **Ownership Transfer** – Only the current owner can transfer land ownership to another user.  
- **Instant Verification** – Anyone can verify land details directly on the blockchain.  
- **Fraud Prevention** – Ensures that only unregistered land can be added.  

## Smart Contract Functions  

### 1. Register Land  
```solidity
function registerLand(uint256 _id, string memory _location, uint256 _area) public
Registers a new land parcel with a unique ID, location, and area. The sender becomes the owner.

2. Transfer Ownership

function transferOwnership(uint256 _id, address _newOwner) public
Allows the current owner to transfer land ownership to a new owner.

3. Get Land Details
function getLand(uint256 _id) public view returns (uint256, string memory, uint256, address, bool)
Fetches details of a registered land parcel.

4. Check Registration Status

function isLandRegistered(uint256 _id) public view returns (bool)
Checks if a land parcel is registered on the blockchain.

Tech Stack
Blockchain Platform: Ethereum
Smart Contract Language: Solidity (^0.8.0)
Development & Testing: Remix IDE
Getting Started

1. Clone the Repository

git clone https://github.com/yourusername/land-registry-system.git
cd land-registry-system
2. Deploy Using Remix IDE
Open Remix IDE.
Create a new Solidity file (LandRegistry.sol) and paste the contract code.
Compile the contract using Solidity Compiler (0.8.0 or later).
Deploy the contract using Injected Web3 (MetaMask) or a local Ethereum testnet.

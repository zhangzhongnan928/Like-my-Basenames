# Like My Basenames Tapp

This is a simple Tapp (Token Application) for interacting with Basenames NFTs on the Base blockchain. The Tapp allows users to like or dislike Basenames and share them via Tlinks.

## Features

1. **Like**: Users can like a Basename NFT.
2. **Dislike**: Users can dislike a Basename NFT.
3. **Share Tlink**: Generate a shareable Tlink for the current Basename NFT.

## How It Works

- The Tapp runs in the TokenScript viewer: https://viewer.tokenscript.org/
- It interacts with Basenames NFTs on the Base blockchain (Chain ID: 8453)
- The contract address for Basenames NFTs is: 0x03c4738Ee98aE44591e1A4A4F3CaB6641d95DD9a
- The Tapp uses ERC-7738 for script registration

## Tlink Format

A typical Tlink for this Tapp looks like: https://viewer.tokenscript.org/?chain=8453&contract=0x03c4738Ee98aE44591e1A4A4F3CaB6641d95DD9a&scriptId=7738_4&tokenId=2

Where:
- `chain=8453`: Refers to the Base blockchain
- `contract=0x03c4738Ee98aE44591e1A4A4F3CaB6641d95DD9a`: The Basenames NFT contract address
- `scriptId=7738_4`: The TokenScript ID in the ERC-7738 registry contract
- `tokenId=2`: The specific Basename NFT ID

## TokenScript Cards

The Tapp consists of three main TokenScript cards:

1. **Like**: Allows users to like the current Basename NFT.
2. **Dislike**: Allows users to dislike the current Basename NFT.
3. **Share Tlink**: Generates a shareable Tlink for the current Basename NFT.

## Smart Contract Interaction

- Likes and dislikes are recorded in a separate smart contract.
- Each user can only choose to either like or dislike a Basename.
- Subsequent transactions will override the previous choice.

## Development

This Tapp is developed using TokenScript, which allows for cross-platform compatibility and portability.

To modify or extend this Tapp:

1. Edit the TokenScript XML file (`Like-my-Basenames.xml`)
2. Update the smart contract for handling likes/dislikes
3. Test the Tapp in the TokenScript viewer
4. Register the updated TokenScript using ERC-7738

## Deployment

After development:

1. Upload the TokenScript file to IPFS or another decentralized storage
2. Register the TokenScript URI using the ERC-7738 registry contract

## Usage

To use this Tapp:

1. Navigate to the TokenScript viewer with a valid Tlink
2. Connect your wallet
3. Interact with the Basename NFT using the provided cards

Enjoy interacting with Basenames in this simple, portable Tapp!


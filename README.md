# NFT Minter

## 🎬 Recorded Sessions
| Link | Instructor | Event |
| ---- | ---------- | ----- |
| [<img src="https://raw.githubusercontent.com/Solana-Workshops/.github/main/.docs/youtube-icon.png" alt="youtube" width="20" align="center"/> Recording](https://youtu.be/Fx7NTkn6IGc) | Joe Caulfield | N/A |

## 📗 Learn

This workshop makes use of Metaplex's new JS SDK for managing NFTs and tokens!   
   
You can find the docs and source code for the SDK [here](https://github.com/metaplex-foundation/js).   
   
### About the Solana dApp Scaffold
This workshop, like many others in the Solana Workshops collection, is built using the dApp Scaffold. This scaffold provides a huge handful of out-of-the-box NextJS configs and functionality to get up & running fast with building a dApp on Solana.   
   
Amongst other things, this scaffold gives you:
* Wallet connection support for popular wallets
* Airdrop functionality & components
* User SOL balance store
* Navbar & Footer
* Basic NextJS file structure layout

### About the Metaplex JS SDK
This new SDK brings with it some awesome abstractions around common NFT functions like uploading images & metadata to Arweave, creating NFTs and Editions, and minting NFTs to a user.   
   
You can see Metaplex is making use of an object called `Metaplex` which handles all of the configs and some core operations with Arweave.   
   
Once you set up the `Metaplex` instance, you can use it's modules like `nfts()` to interact with Solana and manage assets!

### The `nfts()` Module
The module for NFTs can be used to create and also query NFT data on Solana.   
   
In this demo, we are going to just use `nfts()` to create and mint NFTs, and also upload metadata to Arweave, but you can expand on this module to also render the user's owned NFTs and their associated metadata/image.

### Creating a Metaplex NFT Collection
There are a number of ways you can create a Collection with Metaplex for your NFTs.   
   
Ultimately, you just need to create a Collection account using the Metaplex on-chain program. However you accomplish this, you can use that account's address to dictate what collection any new NFT belongs to.   
   
An easy way to create new collections on Metaplex is to go to their [Create Collection Portal](https://collections.metaplex.com/) and follow the steps on-screen to create a new collection!
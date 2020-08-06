# Padlock HackFS Submission
A collection of all repos used in our HackFS project submission

## Description
Helping artists monetize creative work via the decentralized web. Users can buy or sell access to exclusive content hosted on IPFS and Filecoin. The app will generate unique encryption and decryption keys and store them in the encrypted state of a privacy-preserving smart contract on Secret Network.
- Subgraph
 https://thegraph.com/explorer/subgraph/padlockapp/padlock
- .Crypto Domain (needs Unstoppable Extension installed)
https://padlock.crypto

## How It's Made
- Secret Network for key generation for content encryption/decryption
- IPFS and Filecoin for storage (leveraged by Textile’s Powergate using the public http instance for IPFS hosting and Filecoin deal-making)
- The Graph for indexing, Fleek for hosting, 3Box for managing profiles and storing secret keys and Secret Network credentials
- Metamask for Ethereum wallet use, and Pinata for pinning IPFS creations

App is built using Typescript-based React w/ Redux Saga for state management. Ethereum is used as the payment and data layer. There’s also the oracle that’s watching purchases and whitelisting buyers on the Padlock Secret Network contract as well as minting an NFT for each user purchase which acts as a receipt.

## HackFS Showcase
https://hack.ethglobal.co/showcase/padlock-recOwF5kjzFYLkYkO

## Running The App

1. Install MetaMask and switch network to Ropsten.
2. Allow insecure content (the app uses a mix of http & https API endpoints).
- If you're using Chrome, go to "Site settings" by right-clicking the https lock icon.
- For "Insecure content", choose "Allow".

3. Add this line to your /etc/hosts file for DNS resolution:
`45.76.11.245 secret.padlockdev.org faucet.padlockdev.org ui.padlockdev.org`

4. Go to each of the following URLs and accept the certs.
- https://secret.padlockdev.org
- https://faucet.padlockdev.org
- https://ui.padlockdev.org

5. You need to be whitelisted by the Secret Network contract to be able to publish, easiest way to do that at the moment is to buy an item using our fake test DAI token.

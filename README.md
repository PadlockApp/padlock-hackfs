# Padlock HackFS Submission
A collection of all repos used in our HackFS submission project.

# How It's Made
Secret Network for key generation for content encryption/decryption, IPFS and Filecoin for storage (leveraged by Textile’s Powergate using the public http instance for IPFS hosting and Filecoin deal-making), The Graph for indexing, Fleek for hosting, 3Box for managing profiles and storing secret keys and Secret Network credentials, Metamask for Ethereum wallet use, and Pinata for pinning IPFS creations. App is built using Typescript-based React w/ Redux Saga for state management. Ethereum is used as the payment and data layer. There’s also the oracle that’s watching purchases and whitelisting buyers on the Padlock Secret Network contract as well as minting an NFT for each user purchase which acts as a receipt.

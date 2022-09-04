# RTW3-NFT-dynamic-update

## Week 5

[alchemy week 5](https://docs.alchemy.com/docs/5-connect-apis-to-your-smart-contracts-using-chainlink)

Contract to change the NFT according to the market trend (ETH/USD)

## How to deploy

- Create a subscription in [Chainlink](https://vrf.chain.link/)
- Grab the suscription id
- Go to [Chainlink price feeds](<https://docs.chain.link/docs/ethereum-addresses/#Rinkeby%20Testnet%20(Deprecated)>) an grab a pair (i.e ETH/USD) according to the network.
- Choose an interval, it could be 10, 30, 120 (any positive number)
- Deploy
- Mint a NFT, then hit `performUpkeep` with the argument `[]`, this action will generate a random number, then will pick a NFT metadata to update the NFTs.
- check your changes in [Opensea](https://testnets.opensea.io/)

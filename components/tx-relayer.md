# TX relayer

The `adex-tx-relayer` is a simple daemon to relay transactions on to the Ethereum network. Most interactions in AdEx don't require being committed on-chain, and are instead broadcasted as signed messages: for example, validator votes or state channel updates in the case of `adex-smart-platform`.

However, in order to update the on-chain balances, we need to commit those messages on-chain, especially time-sensitive cases such as OCEAN validator votes (OCEAN channels have a timeout).

To enhance the UX of using the AdEx dApp, some participants in the network may be implicitly delegated as transaction relayers - e.g. validators that receive a higher token reward for validation, who've agreed that they will commit the messages on the blockchain.

@TODO describe implicit delegation as a relayer: e.g. if a validator has the highest fee, it will implicitly relay the tx
@TODO think of mechanics of the implicit thing on ethereum: on eth, we need a relayer
@TODO think of the mechanics of TX committing on cosmos/polka; the fee can just come out of the total OCEAN/state channel reward/deposit
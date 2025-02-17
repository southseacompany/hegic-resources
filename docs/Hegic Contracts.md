# Hegic Contract Registry

Below is a list of smart contracts that are deployed and utilized across the Hegic ecosystem.

## Token Contracts

### HEGIC

There are two native tokens within the Hegic ecosystem. The Hegic token (HEGIC) which represents a claim on the fees generated by the protocol, the Hegic IOU token (rHEGIC) which represents a future claim on HEGIC tokens.


| Token                                                                             | Address                                    |
| --------------------------------------------------------------------------------- | ------------------------------------------ |
| [HEGIC](https://etherscan.io/token/0x584bC13c7D411c00c01A62e8019472dE68768430)    | 0x584bC13c7D411c00c01A62e8019472dE68768430 |
| [rHEGIC](https://etherscan.io/token/0x47C0aD2aE6c0Ed4bcf7bc5b380D7205E89436e84)   | 0x47C0aD2aE6c0Ed4bcf7bc5b380D7205E89436e84 |

A swap contract is available to convert rHEGIC tokens earned in Phase I of the incentive program into HEGIC. The converted HEGIC tokens are being unlocked gradually, with 100% becoming available to withdraw on 26 June 2021.

| Contract                                                                        | Address                                    | Github |
| ------------------------------------------------------------------------------- | ------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| [Swap](https://etherscan.io/address/0x1f533acf0c12d12997c49f4b64192030b6647c46) | 0x1F533aCf0C12D12997c49F4B64192030B6647c46 | [GradualTokenSwap.sol](https://github.com/hegic/GradualTokenSwap/blob/master/contracts/GradualTokenSwap.sol) |

### Liquidity Providers

Liquidity providers deposit either wrapped Bitcoin (WBTC) or Ether (ETH) into Hegic liquidity pools and receive write tokens which represent their share in their respective pool. Wrapped tokens can then be staked in order to earn rHEGIC.


| Token                                                                              | Address                                    |
| ---------------------------------------------------------------------------------- | ------------------------------------------ |
| [writeETH](https://etherscan.io/token/0x878f15ffc8b894a1ba7647c7176e4c01f74e140b)  | 0x878f15ffc8b894a1ba7647c7176e4c01f74e140b |
| [writeWBTC](https://etherscan.io/token/0x20dd9e22d22dd0a6ef74a520cb08303b5fad5de7) | 0x20dd9e22d22dd0a6ef74a520cb08303b5fad5de7 |

| LP Staking Pool                                                                         | Address                                    | Github                                                                                                       |
| --------------------------------------------------------------------------------------- | ------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |
| [ETH staking](https://etherscan.io/address/0x9b18975e64763bda591618cdf02d2f14a9875981)  | 0x9b18975e64763bda591618cdf02d2f14a9875981 | [HegicETHOptions.sol](https://github.com/hegic/contracts-v888/blob/master/contracts/Pool/HegicETHPool.sol)   |
| [WBTC staking](https://etherscan.io/address/0x202ec7190f75046348de5ab3a97cc45d7b440680) | 0x202ec7190f75046348de5ab3a97cc45d7b440680 | [HegicWBTCOptions.sol](https://github.com/hegic/contracts-v888/blob/master/contracts/Pool/HegicWBTCPool.sol) |

### Options contracts

| Options Contract                                                                                 | Address                                    | Github                                                                                                               |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------ | -------------------------------------------------------------------------------------------------------------------- | 
| [ETH options contract](https://etherscan.io/address/0xefc0eeadc1132a12c9487d800112693bf49ecfa2)  | 0xEfC0eEAdC1132A12c9487d800112693bf49EcfA2 | [HegicETHOptions.sol](https://github.com/hegic/contracts-v888/blob/master/contracts/Options/HegicETHOptions.sol)     |
| [WBTC options contract](https://etherscan.io/address/0x3961245db602ed7c03eeccda33ea3846bd8723bd) | 0x3961245DB602eD7c03eECcda33eA3846bD8723BD | [HegicWBTCOptions.sol](https://github.com/hegic/contracts-v888/blob/master/contracts/Options/HegicWBTCOptions.sol)   |

### Hegic Staking Lot contracts

Hegicians can stake their HEGIC to gain a share in the protocols profits. To do so, 888,000 HEGIC need to be staked and users will receive a hegic lot token (hlETH or hlWBTC) to represent their stake.

| Token                                                                           | Address                                    |
| ------------------------------------------------------------------------------- | ------------------------------------------ |
| [hlETH](https://etherscan.io/token/0x1ef61e3e5676ec182eed6f052f8920fd49c7f69a)  | 0x1Ef61E3E5676eC182EED6F052F8920fD49C7f69a |
| [hlWBTC](https://etherscan.io/token/0x840a1ae46b7364855206eb5b7286ab7e207e515b) | 0x840a1AE46B7364855206Eb5b7286Ab7E207e515b |

| Staking lot contract                                                              | Address                                    | Github                                                                                                             |
| --------------------------------------------------------------------------------- | ------------------------------------------ | ------------------------------------------------------------------------------------------------------------------ |
| [hlETH](https://etherscan.io/address/0x840a1ae46b7364855206eb5b7286ab7e207e515b)  | 0x1Ef61E3E5676eC182EED6F052F8920fD49C7f69a | [HegicStakingETH.sol](https://github.com/hegic/contracts-v888/blob/master/contracts/Staking/HegicStakingETH.sol)   |
| [hlWBTC](https://etherscan.io/address/0x1ef61e3e5676ec182eed6f052f8920fd49c7f69a) | 0x840a1AE46B7364855206Eb5b7286Ab7E207e515b | [HegicStakingWBTC.sol](https://github.com/hegic/contracts-v888/blob/master/contracts/Staking/HegicStakingWBTC.sol) |

### Chainlink price oracles

Hegic asset pricing for an option's underlying asset utilizes Chainlink oracles.

| Chainlink price oracles                                                          | Address                                    |
| -------------------------------------------------------------------------------- | ------------------------------------------ |
| [ETH](https://etherscan.io/address/0x5f4eC3Df9cbd43714FE2740f5E3616155c5b8419)   | 0x5f4eC3Df9cbd43714FE2740f5E3616155c5b8419 |
| [WBTC](https://etherscan.io/address/0xf4030086522a5beea4988f8ca5b36dbc97bee88c)  | 0xF4030086522a5bEEa4988F8cA5B36dbC97BeE88c |

### Hegic purchasing venues 

Hegic can either be purchased through the Hegic bonding curve or on decentralized exchanges.

| Purchaising venue contract                                                               | Address                                    | Github                                                                                                            |
| ---------------------------------------------------------------------------------------- | ------------------------------------------ | ----------------------------------------------------------------------------------------------------------------- |
| [Bonding curve](https://etherscan.io/address/0x25b904ba7f17663f9005d34db03c97171e4d4cb7) | 0x25b904ba7f17663f9005d34db03c97171e4d4cb7 | [BondingCurve.sol](https://github.com/hegic/contracts-v888/blob/master/contracts/BondingCurve/BondingCurve.sol)   |
| [Uniswap](https://etherscan.io/address/0x1273ad5d8f3596a7a39efdb5a4b8f82e8f003fc3)       | 0x1273ad5d8f3596a7a39efdb5a4b8f82e8f003fc3 |                                                                                                                   |
| [Sushiswap](https://etherscan.io/address/0x6463bd6026a2e7bfab5851b62969a92f7cca0eb6)     | 0x6463bd6026a2e7bfab5851b62969a92f7cca0eb6 |                                                                                                                   |

### Third Party Staking Pool solutions

Since a staking lot requires 888,000 HEGIC to acquire, several staking pool solutions have been created to cater to tokenholders without less than 888,000 HEGIC that wish to benefit from their share in protocol fees. 

| Staking Pool Contracts                                                                    | Address                                    |
| ----------------------------------------------------------------------------------------- | ------------------------------------------ |
| [hegicstaking](https://etherscan.io/address/0xf4128b00afda933428056d0f0d1d7652af7e2b35)   | 0xf4128b00afda933428056d0f0d1d7652af7e2b35 |
| [zLOT](https://etherscan.io/address/0x9e4e091fc8921fe3575eab1c9a6446114f3b5ef2)           | 0x9e4e091fc8921fe3575eab1c9a6446114f3b5ef2 |


| Staking Pool Tokens                                                                               | Address                                    |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------ |
| [sHEGIC, hegicstaking](https://etherscan.io/address/0xf4128b00afda933428056d0f0d1d7652af7e2b35)   | 0xf4128b00afda933428056d0f0d1d7652af7e2b35 |
| [zHEGIC, zLOT](https://etherscan.io/address/0x837010619aeb2ae24141605afc8f66577f6fb2e7)           | 0x837010619aeb2ae24141605afc8f66577f6fb2e7 |


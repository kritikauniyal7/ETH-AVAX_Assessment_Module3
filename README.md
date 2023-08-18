## Types Of Functions-ETH-AVAX-Assessment-Module3
This repository serves as a project assessment for the third module of the "Solidity AVAX Intermediate" course offered by Metacrafters Academy. The main objective behind creating this repository is to demonstrate my acquired knowledge and exhibit my proficiency as a Solidity developer. This project showcases my learning journey and skills to potential viewers, highlighting my capabilities in the realm of Solidity development.

## Problem Statement
Develop a smart contract to establish a personalized token, and utilize either HardHat or Remix to deploy it. Once deployed, the contract should be interactive for the walkthrough video. Within your chosen platform, the contract creator must possess the capability to generate tokens for a designated address. Additionally, any participant should have the ability to execute actions such as burning and transferring tokens.

## Explanation
This is a straightforward Solidity smart contract designed to establish and manage an ERC-20 compliant token within the Ethereum blockchain. The contract embodies the standard characteristics of a fungible token, enabling users to perform actions like transferring, burning, and minting tokens.

# Key Aspects
1.Name and Symbol: The token possesses a name and symbol, which are accessible on the blockchain.
2.Total Supply: The token's total supply remains constant after deployment and is publicly accessible.
3.Balances: The contract monitors token balances held by each address. Users can query their personal balance.
4.Transfer: Users can move tokens to other addresses, with the contract validating sufficient balance prior to executing the transfer.
5.Burn: Token holders can "burn" or eliminate a specific token amount, effectively decreasing the overall supply.
6.Mint: The contract's owner has the authority to "mint" or generate new tokens and allocate them to particular addresses. The minting capability is limited to the contract's owner.
# Engaging with the Token
Upon deployment, users can interact with the token using these functions:

transfer(address _to, uint256 _value): Facilitates the transfer of _value tokens to the designated _to address.
burn(uint256 _value): Allows token holders to eliminate (burn) _value tokens from their own address.

# For the contract owner:
mint(address _to, uint256 _value): Empowers the owner to mint _value new tokens and assign them to the _to address. Keep in mind that performing transfers and burning operations requires sufficient balance. The contract ensures that no tokens are sent to the zero address (address(0)).

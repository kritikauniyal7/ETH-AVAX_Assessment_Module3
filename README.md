# Types Of Functions-ETH-AVAX-Assessment-Module3
This repository serves as a project assessment for the third module of the "Solidity AVAX Intermediate" course offered by Metacrafters Academy. The main objective behind creating this repository is to demonstrate my acquired knowledge and exhibit my proficiency as a Solidity developer. This project showcases my learning journey and skills to potential viewers, highlighting my capabilities in the realm of Solidity development.

##  Problem Statement
Develop a smart contract to establish a personalized token, and utilize either HardHat or Remix to deploy it. Once deployed, the contract should be interactive for the walkthrough video. Within your chosen platform, the contract creator must possess the capability to generate tokens for a designated address. Additionally, any participant should have the ability to execute actions such as burning and transferring tokens.

## Explanation
This is a straightforward Solidity smart contract designed to establish and manage an ERC-20 compliant token within the Ethereum blockchain. The contract embodies the standard characteristics of a fungible token, enabling users to perform actions like transferring, burning, and minting tokens.

## Key Aspects
1.Name and Symbol: The token possesses a name and symbol, which are accessible on the blockchain.

2.Total Supply: The token's total supply remains constant after deployment and is publicly accessible.

3.Balances: The contract monitors token balances held by each address. Users can query their personal balance.

4.Transfer: Users can move tokens to other addresses, with the contract validating sufficient balance prior to executing the transfer.

5.Burn: Token holders can "burn" or eliminate a specific token amount, effectively decreasing the overall supply.

6.Mint: The contract's owner has the authority to "mint" or generate new tokens and allocate them to particular addresses. The minting capability is limited to the contract's owner.
### Engaging with the Token
Upon deployment, users can interact with the token using these functions:

transfer(address _to, uint256 _value): Facilitates the transfer of _value tokens to the designated _to address.
burn(uint256 _value): Allows token holders to eliminate (burn) _value tokens from their own address.

### For the contract owner:
mint(address _to, uint256 _value): Empowers the owner to mint _value new tokens and assign them to the _to address. Keep in mind that performing transfers and burning operations requires sufficient balance. The contract ensures that no tokens are sent to the zero address (address(0)).

## Executing Program
### Steps
1.Access Remix: Access the Remix IDE by visiting the web-based platform at https://remix.ethereum.org/. Remix is an integrated development environment tailored for Ethereum smart contracts.

2.Create a New File: In Remix, initiate a new file by naming it "Token.sol." Paste the provided smart contract code into this file.

3.Select Solidity Compiler: Within Remix, locate the "Solidity Compiler" tab positioned on the left sidebar. From the dropdown menu, opt for the desired compiler version (e.g., 0.8.0).

4.Compile the Contract: Trigger the "Compile Token.sol" button to initiate the compilation process for the smart contract. Verify that there are no compilation errors present.

5.Deploy the Contract: Upon successful compilation, proceed to the "Deploy & Run Transactions" tab situated in the Remix IDE.

6.Select the Environment: Choose your preferred Ethereum environment from the dropdown menu. Options include the JavaScript VM for local testing or Injected Web3 for external wallet interaction like MetaMask.

7.Set Contract Parameters: Input the necessary parameters for the contract constructor, including the name, symbol, and totalSupply. Click the "Transact" button to deploy the contract with these specific parameters.

8.Initiate Deployment: Execute the "Deploy" button to commence the deployment of the Token smart contract within the chosen environment.

9.Engage with the Contract: Once the contract is deployed, you can actively interact with it using the provided functions.

## How to Use
1.Clone the repository or acquire the mToken.sol file.

2.For contract execution, utilize the Remix IDE (https://remix.ethereum.org/) or an alternative Ethereum development environment.

3.Compile the contract using a Solidity compiler, opting for version 0.8.0 or a compatible alternative.

4.Deploy the contract to an Ethereum environment, either through Remix or alternative deployment utilities.

5.When deploying, input the preferred name, symbol, and totalSupply values for the token.

6.Subsequent to deployment, engage with the contract via functions such as transfer, burn, and mint.

## Author
Kritika Uniyal
Student-Chandigarh University

## Explanation Video
https://www.loom.com/share/6f9cc80bb45b42cdb258450949965886?sid=b5ecb1f5-3e20-4fb0-a919-3850c7387cea
(I have added and executed the burn function in the code).

## License
This project is licensed under the MIT License - see the LICENSE file for details.




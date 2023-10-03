## Degen-Token-ERC-20-Contract

The "DegenGaming" smart contract is a powerful and adaptable Ethereum-based solution tailored for gaming applications on the Avalanche Fuji Test Network. This contract serves as a fundamental framework for crafting engaging gaming experiences, empowering game developers to effortlessly handle in-game assets, tokens, and transactions. Specifically developed for the Eth + Avax Intermediate Module 4 Project on the Metacrafters learning platform.

Let's delve into the salient features of this contract:

**Key Features:**

Token Information: The contract defines basic token information, including its name ("Degen Gaming Token"), symbol ("DGT"), and decimal precision (18).

Total Supply: It keeps track of the total token supply, which is set during contract deployment.

Balance Tracking: The contract maintains a mapping of addresses to their token balances using the balanceOf mapping.

Allowances: It stores allowances for token transfers, allowing one address to spend tokens on behalf of another. This is managed through the allowance mapping.

Owner: The contract has an owner, initially set to the deployer's address (msg.sender), who has special privileges, such as minting new tokens.

Events: The contract emits several events to log important actions, including Transfer (for token transfers), Approval (for approval of token spending), Mint (when new tokens are created), Redeem (when users redeem prizes), and Burn (when tokens are destroyed).

Prize Cost Mapping: There's a mapping to store the cost of different prizes. Users can redeem prizes using their tokens, and the cost of each prize is associated with its name.

Constructor: The constructor initializes the contract with the initial supply, sets the owner, and initializes the prize costs.

Modifiers: The onlyOwner modifier restricts certain functions (like minting) to be called only by the contract owner, enhancing security and control.

Token Transfer Functions: The contract provides standard ERC20 functions for transferring tokens (transfer, approve, transferFrom). These functions ensure secure and permissioned token transfers.

Minting: The mint function allows the owner to create new tokens and distribute them to specified addresses.

Redeeming Prizes: Users can redeem prizes by calling the redeem function, which deducts the required token amount from their balance and logs the prize redemption.

Burning Tokens: The burn function allows users to destroy their tokens, reducing the total supply. This can be useful for implementing token sinks.

The "DegenGaming" smart contract demonstrates a comprehensive set of functionalities, making it a valuable tool for game developers looking to implement blockchain-based gaming features, manage in-game economies, and provide players with engaging gaming experiences on the Avalanche Fuji Test Network.

## Getting Started With Remix

```
To execute this program and interact with the "DegenGaming" smart contract on the Avalanche Fuji Testnet, follow these steps:

Ensure Fuji Testnet is connected to Avalanche:

Make sure your metamask are connected to the Avalanche Fuji Testnet using your MetaMask wallet, and you have some test AVAX (Avalanche's native cryptocurrency) in your wallet to use for transactions.

Use Remix Solidity IDE:

To run the program, you can use Remix, an online Solidity Integrated Development Environment (IDE). Access Remix by visiting the Remix website at https://remix.ethereum.org/.

Create a New Solidity File:

Once you are on the Remix website, create a new Solidity file by clicking on the "+" icon located in the left-hand sidebar.
Save the newly created file with a .sol extension, for example, "new.sol."

Copy and Paste the Contract Code:

Copy the code from the "DegenGaming.sol" file (or "token.sol" file) that you want to execute.
Paste the copied code into your newly created "new.sol" file in Remix.

Compile the Contract:

Click on the "Solidity Compiler" tab located in the left-hand sidebar.
Ensure that the "Compiler" option is set to the latest Solidity version (or another compatible version).
Click the "Compile" button to compile the contract code.

Deploy the Contract:

After successful compilation, Before deploying a smart contract, You have to connect remix with your wallet, then navigate to the "Deploy & Run Transactions" tab in the left-hand sidebar.
Select your contract from the dropdown menu, which should be named "DegenGaming" or similar.
Click the "Deploy" button to initiate the contract deployment process.

Enter the Contract Address:

Once the contract is deployed, you will receive a contract address. In the "At Address" input field, enter the contract address.

Interact with the Contract:

With the contract address entered, you can now interact with the deployed "DegenGaming" smart contract.

You can call various functions of the contract, such as minting tokens, burning tokens, transferring tokens, and more, directly within Remix without needing to specify the contract address since it has already been set.
By following these steps, you can execute and interact with the "DegenGaming" smart contract on the Avalanche Fuji Testnet using the Remix Solidity IDE.
```



# Web3 Ballotsystem

This is a demo smart contract designed to illustrate how voting can be conducted on a Web3 app. The Ballot Contract is a fundamental example of decentralized voting, ensuring transparency and immutability of the voting process.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Process](#process)
- [Installation](#installation)
- [Steps to Implement the Ballot](#steps-to-implement-the-ballot)
- [Contributing](#contributing)

## Introduction

The Ballot Contract demonstrates a basic voting mechanism on the blockchain. It allows users to propose options and vote on them, ensuring each vote is counted and stored securely on the blockchain.

## Features

- **Decentralized Voting**: Votes are cast and counted on the blockchain, ensuring transparency.
- **Immutable Records**: Once a vote is cast, it cannot be altered or deleted.
- **Simple Interface**: Easy to understand and interact with, suitable for educational purposes.

## Process

1. **Proposal Submission**: Users can submit proposals that others will vote on.
2. **Voting**: Users cast their votes for the proposals.
3. **Vote Counting**: The smart contract counts the votes and determines the outcome based on the votes cast.

## Installation

To install and deploy the Ballot Contract, follow these steps:

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/yourusername/ballot-contract.git
    cd ballot-contract
    ```
2. **Install Ganache** from [Ganache](https://www.trufflesuite.com/ganache).
3. **Open Ganache** and choose “Quick Start”.
4. **Check for Host Name** - Ensure it is set to `127.0.0.1`. If not, change it to the loopback address.
5. **Set Server Port Number** to `8545`.
6. **Set Account & Keys** - You can set Account Default Balance and Total Accounts to Generate (leave the default settings for now).
7. **Set the Chain** - Configure Gas and Gas Limit, then click on save and restart.
8. **Get 10 Accounts** ready for your private blockchain.
9. **Install MetaMask**: 
    - Open Chrome and go to [MetaMask](https://metamask.io/). 
    - Add the MetaMask Extension to Chrome. 
    - Add the localhost network manually: 
        - Network Name: Any name you choose
        - New RPC URL: `http://localhost:8545`
        - ChainID: `1337` (default for port 8545)
        - Currency Symbol: `ETH`
        - Block Explorer URL: (optional, e.g., `https://etherscan.io`)
        - Save the settings.
10. **Deploy the Contract**:
    Ensure you have a development environment set up (like Remix IDE or Hardhat) and deploy the contract.I personally use Remix IDE to deploy the contract in a network
11. **Create MetaMask Accounts**:
    - Import private keys from Ganache listed accounts.
    - Create four accounts (or five): 
        - Admin (manages the ballot)
        - Zoe (voter)
        - Ellie (voter)
        - Peter (voter)


## Steps to Implement the Ballot

9. **Create MetaMask Accounts**:
    - Import private keys from Ganache listed accounts.
    - Create four accounts: 
        - Admin (manages the ballot)
        - Zoe (voter)
        - Ellie (voter)
        - Peter (voter)
10. **Copy and Paste ballot.sol**:
    - Get the contract from [Ballot System](https://github.com/needanewone/ballotsystem).
    - Paste it into [Remix IDE](https://remix.ethereum.org/).
    - Switch to the Admin MetaMask account before compiling.
    - Compile the contract.
11. **Deploy the Contract**:
    - In Remix, switch to the Admin’s MetaMask wallet account.
    - Deploy the Ballot contract.
    - Set up a proposal (e.g., "Should we re-elect the Chairman?").
12. **Set Up Ballot Manager**:
    - Go to [Ballot Manager](https://needanewone.github.io/ballotsystem/).
    - As Admin, fill in the Ballot Official Name and the Proposal. Click “Go”.
13. **Add Voters**:
    - As Admin, add voters (e.g., Alice, Bob, and Carol) by adding their wallet addresses and names.
14. **Start Voting**:
    - As Admin, start the vote by pressing “Start Voting”.
15. **Vote**:
    - Let each voter vote at [Ballot Voting](https://needanewone.github.io/ballotsystem/vote.html).
    - Switch MetaMask account for each voter.
    - Enter the Ballot Address and click [Go].
    - Retrieve ballot details and vote [Yes] or [No].
16. **Check Voter Status**:
    - Switch back to Ballot Manager as Admin.
    - Check the status of the voters.
17. **End Voting and Get Results**:
    - As Admin, end the voting.
    - Display the results.
    - View the total number of voters and total votes cast.

**IMPORTANT NOTES**: If you want to repeat the voting process, restart Ganache and MetaMask (for ALL involved accounts), and re-copy, paste, and compile `ballot.sol` beforehand.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request to contribute.




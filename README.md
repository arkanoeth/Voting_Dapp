# Voting Decentralized Application (DApp)
This is a simple Ethereum-based decentralized application (DApp) for conducting voting using smart contracts. The DApp allows users to register as voters, cast their votes for candidates, and tally the votes to determine the winner.

## Getting Started
These instructions will help you deploy and use the Voting DApp on an Ethereum network.

## Prerequisites
To interact with the Voting DApp, you'll need the following:

-An Ethereum wallet (e.g., MetaMask) and some Ether in testnet for transaction fees.
-An Ethereum development environment, such as Remix IDE or Truffle.
-Deployment

## Follow the steps below to deploy the Voting DApp:
Clone this repository to your local machine.
Open the smart contract file VotingDApp.sol in an Ethereum development environment.
Compile the smart contract using Solidity compiler version 0.8.0 or compatible.
Deploy the compiled smart contract to the desired Ethereum network (e.g., Ropsten, Rinkeby, or a local development network).

## Usage
Once the smart contract is deployed, follow these steps to use the Voting DApp:

Register as a Voter: Call the registerVoter function from your Ethereum wallet to register as a voter.

Start Voting Phase: After all voters have registered, the administrator can start the voting phase using the startVoting function.

Cast Your Vote: During the voting phase, use the castVote function to cast your vote by specifying the candidate's index you wish to vote for.

End Voting Phase: Once the voting phase is complete, the administrator can end the voting phase using the endVoting function.

Tally the Votes: After the voting phase has ended, the administrator can tally the votes and determine the winner by calling the tallyVotes function.

Add New Candidates: The administrator can add new candidates to the list of candidates by calling the addCandidate function.

Switch Phases: The administrator can switch between different phases (registration, voting, tallying) using the switchPhase function if needed.

## Smart Contract Details
The smart contract VotingDApp.sol consists of the following main components:

Candidates: The list of candidates available for voting.

Voters: A mapping that stores voter details, including whether a voter is registered, has voted, and the index of the candidate they voted for.

Admin: The address of the administrator who controls the DApp and can manage the voting phases.

Phases: The DApp operates in three phases - 1 (Registration), 2 (Voting), and 3 (Tallying).

Events: The smart contract emits events for voter registration, vote casting, and candidate addition.

## License
This project is licensed under the MIT License. 

If you have any doubts do not hesitate to contact me, I´m happy to help you!

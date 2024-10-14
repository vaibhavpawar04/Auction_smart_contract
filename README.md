# Auction_smart_contract
This a auction smart contract deployed on blockchain using solidity

**Description-**
This Solidity project consists of two contracts: AuctionCreator and Auction. The AuctionCreator contract allows for the creation of multiple auctions, while the Auction contract represents an individual auction that users 
can participate in by placing bids. Each auction is managed by the person who creates it.

**Features-**
- *Auction Creation:* Users can create new auctions through the AuctionCreator contract.
- *Auction Lifecycle Management:* The contract includes states to manage the auction process (e.g., Started, Running, Ended, Canceled).
- *Bidding Functionality:* Users can place bids on active auctions.
- *IPFS Integration:* The contract supports storing auction-related information on IPFS.

**Contract Details-**
1. *AuctionCreator Contract:*
   - Allows the creation and management of multiple auctions.
   - The createAuction() function creates a new auction and adds it to the list.

2. *Auction Contract:*
   - Represents an individual auction, with the owner being the auction creator.
   - Includes state variables such as owner, startBlock, endBlock, ipfsHash, and auctionState (Started, Running, Ended, Canceled).
   - Manages the highest bid and bidder information.
   - Provides functions like cancelAuction() and finalizeAuction() for lifecycle management.
   - Allows users to place bids using the placeBid() function.
  
**Usage-**
1. *Deploy the AuctionCreator contract* on a blockchain network (e.g., Ethereum).
2. *Create a new auction* by calling the createAuction() function.
3. *Participate in the auction* by calling the placeBid() function during the auction period.
4. *Manage the auction's lifecycle* using cancelAuction() or finalizeAuction() functions as needed.

**Prerequisites-**
- Solidity version >=0.5.0 <0.9.0.
- Ethereum wallet (e.g., MetaMask) for deploying and interacting with the contracts.

**Security Considerations-**
- Ensure only the auction owner can call sensitive functions like cancelAuction() and finalizeAuction().
- Beware of potential reentrancy vulnerabilities when transferring funds.





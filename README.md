# Aptos Auction

## Overview

Aptos Auction is a decentralized auction system built on the Aptos blockchain using the Move programming language. This project allows users to create, participate in, and manage auctions in a secure and transparent manner.

## Features

-   **Create Auctions**: Users can list items for auction with a specified duration and starting bid.
    
-   **Place Bids**: Participants can bid on active auctions.
    
-   **Automatic Winner Selection**: The highest bid is automatically determined at the end of the auction.
    
-   **Secure and Transparent**: All auction data is stored on-chain for full transparency.
    
-   **Testing Suite**: Includes tests to ensure correct functionality of auction logic.
    

## Requirements

-   [Aptos CLI](https://aptos.dev/cli-tools/aptos-cli/)
    
-   Move language knowledge
    
-   Rust (for Move compiler)
    
-   Aptos testnet or local network
    

## Installation

1.  Clone the repository:
    
    ```
    git clone https://github.com/hieu9484/aptos-auction.git
    cd aptos-auction
    ```
    
2.  Install dependencies:
    
    ```
    aptos init
    ```
    
3.  Compile the Move modules:
    
    ```
    aptos move compile
    ```
    
4.  Deploy to the Aptos blockchain:
    
    ```
    aptos move publish --profile default
    ```
    

## Usage

-   **Creating an Auction**:
    
    ```
    aptos move run --function-id default::auction::create --args <item_id> <starting_bid> <duration>
    ```
    
-   **Placing a Bid**:
    
    ```
    aptos move run --function-id default::auction::bid --args <auction_id> <bid_amount>
    ```
    
-   **Finalizing an Auction**:
    
    ```
    aptos move run --function-id default::auction::finalize --args <auction_id>
    ```
    

## Testing

Run tests to verify the auction logic:

```
aptos move test
```

## License

This project is open-source and available under the MIT License.

## Contributions

Feel free to submit pull requests or open issues for improvements and bug fixes.

## Contact

For any questions or support, please reach out via GitHub Issues.

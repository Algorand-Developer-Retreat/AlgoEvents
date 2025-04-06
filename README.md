# nickthelegend's ticket-nft

# Julo - Event Ticketing on Algorand

**Julo** is a next-generation event ticketing platform built on the Algorand blockchain. It leverages Algorand’s fast, secure, and scalable infrastructure to mint NFT-based event tickets, ensuring authenticity and transparency for organizers and attendees alike.

## Overview

Julo harnesses the power of Algorand by:
- **Minting NFT Tickets:** Every ticket is tokenized as an NFT on the Algorand blockchain.
- **QR Code Generation:** A unique QR code is generated for each ticket. The QR code contains a hash that is signed using `algosdk`'s `sign_bytes` method, ensuring that the ticket is tamper-proof.
- **Blockchain-Powered Security:** Utilizing Algorand’s pure proof-of-stake consensus, transactions are confirmed in less than 4.5 seconds, making ticketing both fast and secure.
- **Cost-Effective & Scalable:** With minimal transaction fees and the ability to handle high throughput, Julo is built for seamless event management.

Check out the [live website](https://julo.abcxjntuh.in/) for a demo.

## Features

- **NFT Ticketing:** Issue and verify NFT tickets on the blockchain.
- **Smart Contract Integration:** Automated ticket distribution and validation via Algorand smart contracts.
- **QR Code Verification:** Secure ticket check-in using QR codes generated from signed payloads.
- **Real-time Transactions:** Benefit from Algorand's fast block finality (< 4.5 seconds).
- **Transparent Pricing & Records:** All transactions are recorded on the blockchain for full transparency.
- **Scalable Architecture:** Designed to handle over 6,000 transactions per second.

## Technologies Used

- **Algorand Blockchain:** For secure, fast, and cost-effective transactions.
- **algosdk:** JavaScript SDK for interacting with the Algorand blockchain (used for signing and verifying ticket hashes).
- **Next.js:** React framework for building a dynamic and responsive front-end.
- **TypeScript:** For robust and maintainable code.

## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:
- [Node.js](https://nodejs.org/) installed (v14 or higher recommended).
- A working knowledge of Algorand and its ecosystem.
- An Algorand wallet for testing transactions.

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/Algorand-Developer-Retreat/AlgoEvents.git
   cd AlgoEvents
   ```











This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

* [X] Multi Ticket Minting in NFT
* [ ] Nft sending when the user signes up
* [ ] ~~Reselling Allowed, or not in create page freeze the assets is reselling is not allowed~~ [Not Planned]
* [ ] ~~Create a reselling zone where people can buy the reselling tokens~~ [Not Planned]
* [ ] Certificates Should be sent when the event is over the Event owner can mint the Certificates of Participation....
* [ ] Asset Metadata and the creator address verification while "Check In"
* [ ] Sign the payload with your private key, Combine the payload and signature, and generate a QR code from the combined JSON
* [ ] Ticket Verification (Check-In App), Scan and decode the QR code to extract the payload and signature, Use the known public key to verify the signature against the payload,If valid, the ticket is confirmed as genuine and untampered
* [X] Change /events its kinda bad design, Add Free Ticket also in /create
* [ ] Add map location in /create
* [X] A Tab where /host events should be there where shows what all events are hosted
* [ ] /calendars should show what all events you subscribe /have tickets of

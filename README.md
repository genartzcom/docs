
# Generative Art with Forma's Precompile Feature

## Overview

By leveraging Forma’s precompile feature, we have seamlessly integrated p5.js and Solidity in a fully generative and programmatic manner. This allows for dynamic NFT creation directly onchain without relying on external storage solutions such as IPFS. Artists can generate Solidity code simply by writing JavaScript, making this a streamlined tool for generative artists.

We have developed a custom library on top of p5.js, enabling a generative fusion of Forma’s precompile capabilities and p5.js scripting. This approach facilitates the creation of NFTs based on metadata from a single or multiple collections, all executed entirely onchain. Additionally, this system allows for personalized generative art by retrieving metadata from users’ wallet-based NFT collections.

### Key Features

- **Onchain Generativity:** Direct Solidity code generation through JavaScript, eliminating the need for **offchain storage.**

- **Custom p5.js Library:** Enhancing p5.js with specific utilities to interact with **Forma’s precompile functionality**.

- **Metadata Flexibility:** Supports both single and **multiple NFT collections**, offering limitless creative possibilities.

- **Wallet-Driven Personalization:** Generates unique generative art by extracting metadata from **NFTs held in a user’s wallet**.

- **Integrated Editor and Library:** Functions as both a creative coding environment and a **Solidity contract generator**.

- **Chunked Storage Mechanism:** Efficiently stores generative assets onchain in a structured and scalable way.

### Technical Implementation

The p5.js code is parsed into two separate components: the JavaScript side and the Solidity side. Each part is optimized and formatted to ensure smooth integration within the Forma Network’s infrastructure.

### Code Examples

Accessing NFT Metadata

```javascript
const Mammoths = FormaCollection('0xbE25A97896b9CE164a314C70520A4df55979a0c6');

// Retrieve metadata as a string
Mammoths.metadata('Body').asString();

// Use a specific token for testing
Mammoths.useToken(2);
```

Data Parsing Methods

```javascript
asString(); // Converts metadata to string format
asInt();    // Converts metadata to integer format
asFloat();  // Converts metadata to floating-point format
```
This project is designed to redefine onchain generative art by offering a powerful, minimalist tool for artists, developers, and collectors alike.


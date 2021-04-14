# CONNECT TO AN AVALANCHE NODE 

## Introduction
[Avalanche](https://www.avalabs.org/) is an open-source platform for launching [decentralized applications](https://support.avalabs.org/en/articles/4587146-what-is-a-decentralized-application-dapp) and enterprise [blockchain](https://support.avalabs.org/en/articles/4064677-what-is-a-blockchain) deployments in one interoperable, highly scalable ecosystem.
Avalanche is the first smart contracts platform that processes 4,500+ transactions/second and instantly confirms transactions.

Avalanche offers:
- Scalability
- Usability
- Interoperability
- Fully customizable subnet architecture
- The ability to build your blockchain and issue unique assets

A key difference between Avalanche and other decentralized networks is the consensus protocol.
The Avalanche protocol employs a novel approach to consensus to achieve its strong safety guarantees, quick finality, and high-throughput, without compromising decentralization.

### Avalanche.js
[Avalanche.js] is a client Javascript package that makes it easy to interact with the Avalanche blockchain nodes, query data, submit transactions and offers plenty of other functionallity.
It's the official package developed by Avalanche, and is a preferred method of communicating with ndoes on the private or public networks for development purposes.

## Creating NodeJS application
### Installing packages
Install a few required packages for our application:
- avalanche - to interact with Avalanche APIs
- dotenv - to manage environment variables

Run the following command to install all dependencies:
`npm install --save avalanche dotenv`

## Connecting to the Avalanche network
`client.js` provides us a function to create and configure the Avalanche node client.
It provides an environment variable check to verify the environment and catch any issues before running the actual code.

Actual functionality is provided by the Info API client `client.Info()` that communicates with [Info API](https://docs.avax.network/build/avalanchego-apis/info-api)

Avalanche provides a set of API endpoints for different components, like X/P/C chains, that are part of the same system.

Run the code with `node connect.js`
# Welcome to Radbro Coding Club

This repository will serve as a place for all work / information / conversations that we want to track, preserve, and share long-term.

Since our main thread of communication will be via twitter gc, and we all will need Github accounts to follow some of the lessons / projects.

I figured we should just use Github itself to pin information & have long-running conversationd on coding topics. This way we can avoid use of discord and telegram entirely.

Long-running conversations on specific topics can be had using [issues](https://github.com/radbro/radbro-coding-club/issues/).

Lesson plans, guides, + links to additional materials will be posted here as well.

### Learning Resources
[Speed Run Ethereum](https://speedrunethereum.com/) learn scaffold-eth and solidity  
[Vyper By Example](https://vyper-by-example.org/) learn vyper - a fast, easy, and secure language to write smart contracts  

### Beginner Tech Stack 1 - Scaffold-ETH
For most beginners, Scaffold-ETH is a fantastic framework to learn how to build dapps.  

This is a "full-block-stack" framework for learning as it's built using hardhat, nextjs, hot-reloading, and many other features to make it very easy to understand the full enineering workflow.  
This means that you'll quickly learn how to go all the way from contracts -> to backend -> to frontend, and deploying your own dapp.  

If you're building a simple dapp, you may not even require an RPC provider as you can simply use the wallet's provider and read from the contracts directly by using viem.  

**Requirements:**  
[Scaffold-ETH 2](https://github.com/scaffold-eth/scaffold-eth-2/blob/main/CONTRIBUTING.md)  

### Intermediate Tech Stack 1 - Scaffold-ETH + Ponder + Alchemy
If you are building a more complex dapp, rather than read from an RPC on-demand (which can be slow), you may want to have all of your contract's historical data & events ready to query so you can build front-ends very quickly.  
To accomplish this, let's look at a slightly modified stack.  

Ponder makes it easy and quick to index all contract events, and it provides a GraphQL API to easily query all of your data and serve it to your app's UI & frontend.

To use ponder effciently, you should use an RPC provider like Alchemy that uses compute units (CU) rather than number of requests.

**Requirements:**  
[Scaffold-ETH 2](https://github.com/scaffold-eth/scaffold-eth-2/blob/main/CONTRIBUTING.md)  
[Ponder.sh](https://github.com/ponder-sh/ponder)  
[Alchemy](https://dashboard.alchemy.com/)  


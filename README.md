# Coineru Coins

>readme `v1.0`   
>2019 01 08

# [Whitepaper](./whitepaper/whitepaper.md)

# Standards

Code was written using various standards. Following software-specific standrads and guidelines were used in this project:
>1. Documentation of the Truffle framework
>2. Solidity Style Guide `v0.5.0`
>3. Ethereum Request for Comment (ERC) standards
>4. Using `OpenZeppelin` libraries  as they intensively audited and tested by the community

# Truffle and Solidity versions

Current project was developed using following versions (or just read `package.json`):
>Truffle `v4.1.15` (core: 4.1.15)  
>Solidity `v0.4.25` (solc-js)  
>Node `v10.15.0`   

# Installation
>1. Clone git repository  
>2. Run: `npm install`

# Tests
Will create a local lightweight Javascript Ethereum Server and perform tests
>Run: `npm run test`

# Build
Will concatenate contracts so they can be deployed to real networks.  
Contracts can found in: `contracts/full`
>Run: `npm run build`

# Deploying and Verifying
You can follow youtube video: https://www.youtube.com/watch?v=vFO5EWIWlX4  
Or  
Following below described process

Following process requires one to have:  
1. Metamask
2. Account connected to metamask
3. Some ether on that account
4. Chrome

To deploy we will use Remix (https://remix.ethereum.org/)
>1. Connect to metamask  
>1.1 Enable Metamask in Chrome  
>1.2 Open https://remix.ethereum.org/  
>1.3 Select tab named `Run` on the right side  
>1.4 Under `Environment` select `Injected Web3` and refresh website  
>1.5 Select tab named `Run` now you should your account address
>1. Create new contract by pressing `Create New File ...` which is the top left corner
>1. Name it accordingly (file name has no impact on process)
>1. Copy full code from `contracts/full` to new file (one at a time)
>1. Under `Compile` tab select `version:0.4.25+commit.59dbf8f1`
>1. Under `Compile` tab make sure `Enable Optimization` check box is not ticked
>1. Under `Compile` press `Start to compile (Ctrl-S)` button
>1. Select `Run` tab
>1. Select your main contract (in our case `CoineruSilver` or `CoineruGold`)
>1. Press `Deploy` and confirm it in Metamask
>1. After it was deployed find contract on etherscan (make sure you select correct etherscan)
>1. Find `Code` tab and press `Verify And Publish`
>1. In new window do following:  
>13.1 Paste same code you used in remix  
>13.2 Fill `Contract Name:` box accordingly (in our case `CoineruSilver` or `CoineruGold`)  
>13.3 In `Compiler` select `version:0.4.25+commit.59dbf8f1`  
>13.4 in `Optimization` select `No`  
>13.5 Scroll down and press `Verify and Publish`  
>1. If it was successfully verified `Successfully generated ByteCode and ABI for Contract Address` should be shown in new window

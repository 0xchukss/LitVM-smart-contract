# LitVM-smart-contract

<img width="803" height="330" alt="image" src="https://github.com/user-attachments/assets/6fba6ab2-529b-4a2d-8c3a-cfd2435f6043" />

## requirements
- zkLTC faucet:
   get [here](https://www.midashand.xyz/), connect wallet, click on faucet and select zkLTC
- liteforge network, add [here](https://liteforge.hub.caldera.xyz/)

# step 1: set up remix environment
  - visit [remix](remix.ethereum.org)
  - sign in with your github
  - create a new workspace (blank template)
  - go to contracts and create a new file
  - name it counter.sol

# step 2: code, compile and deploy
  - paste this code
<pre>
      //SPDX-LICENSE-IDENTIFIER:MIT
    pragma solidity ^0.8.19;
    
    contract Counter {
        uint256 public count;
    
        event CountChanged(uint256 newCount);
    
        constructor(uint256 _initialCount) {
            count = _initialCount;
        }
    
        function increment() public {
            count += 1;
            emit CountChanged(count);
        }
    
        function decrement() public {
            require(count > 0, "Count cannot go below zero");
            count -= 1;
            emit CountChanged(count);
        }
    
        function getCount() public view returns (uint256) {
            return count;
        }
    }
</pre>


<img width="1701" height="735" alt="1" src="https://github.com/user-attachments/assets/c79ab08e-ed91-4c12-833e-b689b2c528ce" />


b. go to compile
- click on compile

<img width="1451" height="708" alt="2" src="https://github.com/user-attachments/assets/b35be665-a485-4c4d-9c6d-f32e8fd454c2" />

c. deploy
- go to deploy
- on environment, change from remix vm to browser extension then select your evm wallet
- manually switch to liteforge network

<img width="1135" height="772" alt="3" src="https://github.com/user-attachments/assets/d122bf19-6dc8-4021-bfeb-cdfb66778af7" />

Deploying
- enter any numerical value in the box and deploy
- sign transaction

<img width="1324" height="868" alt="4" src="https://github.com/user-attachments/assets/bf19d5ad-8f94-4a0b-a965-30e7a047106f" />

## you have created your smart contract on Liteforge testnet network


- 


      
  -

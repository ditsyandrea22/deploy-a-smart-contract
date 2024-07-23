# deploy-a-smart-contract
# Swisstronik Tesnet Techinal Task 1

link : [Click!](https://www.swisstronik.com/testnet2/dashboard)

Feel free donate to my EVM address

EVM :

```bash
0x396a817c3E18DA8F00AB028b8E4924Aa3Ae54Bdd
```

## Steps

### 1. Clone Repository

```bash
https://github.com/ditsyandrea22/deploy-a-smart-contract.git
```

```
cd deploy-a-smart-contract
```

### 2. Install Dependency

```bash
npm install
```

### 3. Set .env File

create .env file in root project

```bash
PRIVATE_KEY="your private key"
```

### 4. Create Smart Contract

- Open contract folder
- Create Hello_swtr.sol file
- Copy this code and paste there

```
/// SPDX-License-Identifier: UNLICENSED
pragma solidity ^0.8.19;

//This contract is only intended for testing purposes

contract Swisstronik {
    string private message;

    /**
     * @dev Constructor is used to set the initial message for the contract
     * @param _message the message to associate with the message variable.
     */
    constructor(string memory _message) payable{
        message = _message;
    }

    /**
     * @dev setMessage() updates the stored message in the contract
     * @param _message the new message to replace the existing one
     */
    function setMessage(string memory _message) public {
        message = _message;
    }

    /**
     * @dev getMessage() retrieves the currently stored message in the contract
     * @return The message associated with the contract
     */
    function getMessage() public view returns(string memory){
        return message;
    }
}
```

### 5. Compile Smart Contract

```bash
npm run compile
```

### 6. Deploy Smart Contract

```bash
npm run deploy
```

### 7. Get Message

```bash
npm run get-message
```

### 8. Get Message

```bash
npm run set-message
```

### 9. Finsihed

- Open the deployed-adddress.ts (location in utils folder)
- Copy the address and paste the address in testnet dashboard
- push this project to your github and paste your repository link in testnet dashboard

by :
github : [ditsyandrea22]((https://github.com/ditsyandrea22))
twitter : @crypto_ditsy
telegram : @crosmail

//0x396a817c3E18DA8F00AB028b8E4924Aa3Ae54Bdd//

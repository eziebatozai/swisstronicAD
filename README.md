
## Jangan Malas Kalau pengen jepe

### 1. Clone Repository {gitpod only copy https://github......

```bash
git clone https://github.com/eziebatozai/swisstronicAD.git
```

```
cd hardhat-deploy-contract
```

### 2. Install Dependency skip use gitpod

```bash
npm install
```

### 3. Set .env File

create .env file in root project/buat file .env di root folder

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

### 9. Done

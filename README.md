# EDULand-Verifier-Node

## 1. Renting EDULand

To rent EDULand (a node key license):

1. Visit the [EDULand Dashboard](https://dashboard.educhain.xyz/eduland).
2. Navigate to the [Manage Page](https://dashboard.educhain.xyz/eduland/manage).
3. Rent your Node Key using Yuzu Points.
4. Note the Node Key ID assigned to you (e.g., `#0001`)
   <img width="464" height="236" alt="image" src="https://github.com/user-attachments/assets/acbe3400-4945-4b09-be75-fa4d90b71a08" />

2. Smart Contracts
Here are the key smart contracts required to earn rewards from your EDULand:
Smart Contract
Address
NodeKey
0xCD68f66269613AC6aa01BB1C2A7302AB84D9098A
DelegateRegistry
0x00000000000000447e69651d841bD8D104Bed493

## 3. Create a Burner Address

To securely manage attestations, create a burner wallet address:

- Use a wallet provider like MetaMask to create a new address.
- This address will be used to delegate attestations, ensuring you don’t need to expose the private key of the address used to rent the Node Key.
- **Never share or expose your private key.** Avoid posting it online, saving it in plain text, or sharing it via email or messaging platforms.

- ## 4. Delegate Rights to Attest

Once you’ve rented a Node Key, delegate rights to the burner address created in the previous step.

### Steps to Delegate Using `DelegateRegistry.delegateERC721`:

1. Open the [Blockscout DelegateRegistry interface](https://educhain.blockscout.com/address/0x00000000000000447e69651d841bD8D104Bed493).
2. Input the following details:
    - **To**: Your burner address (e.g., `0x0811C707fAa45ee5c569308E77Ef4511D22fCa9C`).
    - **Contract**: `0xCD68f66269613AC6aa01BB1C2A7302AB84D9098A`.
    - **TokenId**: Your Node Key NFT ID (e.g., `1049`).
    - **Rights**: `0x0000000000000000000000000000000000000000000000000000000000000000`.
    - **Enable**: `true`.
    - **Send native EDU: 0**
  
      ## 5. Getting a Gelato Relay API Key

The Gelato Relay API Key allows you to pay transaction fees using tokens like USDC.

### Steps to Get an API Key:

1. Visit [Gelato Relay](https://app.gelato.network/relay).
2. Connect your burner wallet and create an account.
3. Click **Create App** and fill out the required details

<img width="1740" height="1272" alt="image" src="https://github.com/user-attachments/assets/cc473283-eb1f-4525-8b93-fcad073225ee" />

4. Copy the API key from the app details page.
   <img width="2048" height="495" alt="image" src="https://github.com/user-attachments/assets/aee59274-eba5-43e2-a86c-373c50ba3778" />
 5.  Fund your Gelato 1Balance with USDC from one of these chains to cover transaction fees. ( $1 to $2 is enough)
    <img width="628" height="800" alt="image" src="https://github.com/user-attachments/assets/12d4aeae-dfac-49fe-a695-58a775ae768b" />
    ## 6. Downloading the Application

( this method is for mobile if you are a PC or a vps user than please use this guide https://notion.opencampus.xyz/How-to-run-EDULand-Verifier-Node-1885a6eae9638051a9ebc6e073137289)




1. first download the termux app from the play store
   https://play.google.com/store/apps/details?id=com.termux



   
2. update it


 pkg update

 
 pkg upgrade

 
 pkg install proot-distro

 proot-distro install ubuntu

 proot-distro login ubuntu

 apt update && apt upgrade



 
 3. install wget (if not installed)

    
 apt install wget

 
4. now Download the application



wget https://github.com/gelatodigital/verifier-node-educhain/releases/download/v1.0.2/edu-chain-verifier-node_1.0.0.8ede663-1_arm64.deb




5. now install or unzip it



dpkg -i edu-chain-verifier-node_1.0.0.8ede663-1_arm64.deb



6. now run the node


edu-chain-verifier-node start


7. now hive your burner wallet private key with 0x


8. your gelato api


9. and your eduland nft number



<img width="572" height="1280" alt="image" src="https://github.com/user-attachments/assets/df7679a8-a63c-438e-8259-dac43403eefa" /> 





and volah your node is running just make sure to not to close your terminal...........


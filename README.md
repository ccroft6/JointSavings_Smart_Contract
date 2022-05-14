# Smart Contract for Joint Savings Account
![Smart Contract](./Execution_Results/smart_contract.jpeg)
In order to automate the creation of joint savings accounts, a Solidity smart contract was created. The smart contract accepts two user addresses that are able to control the joint savings account. Ethereum management functions were written in the smart contract to fulfull a financial institution's requirements of having the necessary features for a joint savings account. For example, the features include being able to deposit and withdraw funds from the account. 

---
## Technologies
This project leverages the following tools:
* [Solidity](https://docs.soliditylang.org/en/v0.8.13/) - programming language for implementing smart contracts
* [Remix IDE](https://remix.ethereum.org/#optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.7+commit.e28d00a7.js) - open source tool that helps you write Solidity contracts straight from the browser; has modules for testing, debugging, and deploying of smart contracts

The Solidity version used for this project was the following:
`pragma solidity ^0.5.0`

---

## Instalation Guide
There are no major installations required. You can access Remix IDE from the web browser. 

---

## Usage
1. Open [Remix IDE](https://remix.ethereum.org/#optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.7+commit.e28d00a7.js) 
2. Open the smart contract file (`joint_savings.sol`) in Remix IDE. (You may need to create a new file and copy and paste the Solidity code to the file)
3. Select the "Solidity Compiler" tab and press the button that says, "Compile joint_savings.sol"
4. Select the "Deploy and Run Transactions" tab and choose the environment of **JavaScript VM**
5. Interact with the functions of the smart contract 

---

## Methods
1. Create and work within a local blockchain development environment using the JavaScript VM provided by the Remix IDE
2. Script and deploy a **JointSavings** smart contract
3. Interact with the deployed smart contract to transfer and withdraw funds

---

## Results 
Here are examples of the Solidity smart contract in action:

### Deployed Contract 
![Deployed Contract](./Execution_Results/deployed_contract.png)

### Using the `setAccounts` function to define the authorized Ethereum addresses that will be able to withdraw funds from the contract
```
Dummy account1 address: 0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb
Dummy account2 address: 0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0
```
![Set Accounts](./Execution_Results/set_accounts.png)

Here is the result of setting up the accounts:
![Set Accounts Result](./Execution_Results/set_accounts2.png)

### Testing the `deposit` functionality of the smart contract by sending the following amounts of ether. After each transaction, using the `contractBalance` function to verify that the funds were added to the contract:

#### Transaction 1: Send 1 ether as wei
![Transaction 1](./Execution_Results/send_1_ether_wei.png)

New Contact Balance:
![Transaction 1 Balance](./Execution_Results/contract_balance_1_ether_wei.png)

#### Transaction 2: Send 10 ether as wei
![Transaction 2](./Execution_Results/10_ether_wei.png)

New Contact Balance:
![Transaction 2 Balance](./Execution_Results/balance_10_ether_wei.png)

#### Transaction 3: Send 5 ether
![Transaction 3](./Execution_Results/5_ether.png)

New Contact Balance:
![Transaction 3 Balance](./Execution_Results/5_ether_balance.png)


### Testing the contract’s `withdrawal` functionality by withdrawing 5 ether into accountOne and 10 ether into accountTwo

Withdrawing 5 ether into `accountOne` - `0x0c0669Cd5e60a6F4b8ce437E4a4A007093D368Cb`:
![Account 1 Ether](./Execution_Results/5_ether_account1.png)

Last withdrawing account, amount, and contract balance:
![Account 1 Balance Withdraw](./Execution_Results/balance_withdraw_account1.png)

Withdrawing 10 ether into `accountTwo` - `0x7A1f3dFAa0a4a19844B606CD6e91d693083B12c0`:
![Account 2 Ether](./Execution_Results/10_ether_account2.png)

Last withdrawing account, amount, and contract balance:
![Account 2 Balance Withdraw](./Execution_Results/balance_withdraw_account2.png)


At the end, the contract balance became 1 ether.

---

## Contributors
Catherine Croft

Email: catherinecroft1014@gmail.com

LinkedIn: [catherine-croft](https://www.linkedin.com/in/catherine-croft-4715481aa/)

---

## License 
MIT
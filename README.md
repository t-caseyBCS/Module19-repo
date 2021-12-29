# FinTech Finder Web Dapp
## Overview:
Welcome! You *<u>(the user)</u>* assumes the role of a Fintech recruiter/ employer looking to hire a professional from our 'Fintech Finder' Web3 Dapp. The user can navigate the page to find a suitable canidate to hire and can base their decision upon different factors included in each canidate's profile. Such as:

* Rating
* Hourly rate

The user can fetch and display their account balance associated with their Ethereum account address. As they hire candiates, the user can see their Ethereum account balance decrease and the balance of another address (the candiate's) on the Ganache blockchain increase.


>This project showcases the creation of your own *<u>Cryptocurrency 'Hot' Wallet</u>* and how you can connect to it using a personalized mnemonic seed phrase generated by Ganache blockchain. As well as, *<u>digitally signing a transaction</u>* that pays a Fintech candidate, and sending this transaction to the Ganache blockchain.


---
### HOW TO RUN:
1. From your terminal, navigate to the project folder that contains your `.env` file and the `fintech_finder.py` and `crypto_wallet.py` files. 
    - *Be sure to activate your Conda `dev` environment if it is not already active.*

2. Open Ganache and copy the mnemonic seed phrase into the `SAMPLE.env` file
    - <u>To update your `.env` file:</u> From your terminal, navigate to the project folder and open the file with `code SAMPLE.env` command (if you have vscode and have it added to your PATH, otherwise use which ever text editor you prefer). 
    - Copy the mnemonic seed phrase from Ganache to the `.env` file and save the file.

![ganache1](Images/ganache1.PNG)

![SAMPLE_env](Images/SAMPLE_env.PNG)

3. To launch the Streamlit application, run the following command: `streamlit run fintech_finder.py`

4. On the resulting webpage, select a candidate that you would like to hire from the appropriate drop-down menu. Then, enter the number of hours that you would like to hire them for. (Remember, you do not have a lot of ether in your account, so you cannot hire them for long!)

![streamlit0](Images/streamlit0.PNG)

5. Click the Send Transaction button to sign and send the transaction with your Ethereum account information. If the transaction is successfully communicated to Ganache, validated, and added to a block, a resulting transaction hash code will be written to the Streamlit application sidebar.

![streamlit1](Images/streamlit1.PNG)

5. Navigate to the Ganache accounts tab and locate your account (index 0).

![ganache2](Images/ganache2.PNG)

6. Navigate to the Ganache transactions tab and locate the transaction.

![ganache3](Images/ganache3.PNG)

![ganache4](Images/ganache4.PNG)

---
### SYSTEM REQUIREMENTS
* Set Streamlit version to 0.84.2 otherwise populated streamlit tables will not display and error out. 
> $ `pip install --upgrade streamlit==0.84.2`

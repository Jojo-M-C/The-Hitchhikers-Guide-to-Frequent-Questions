Smartcontract Speedrun feat. Brownie 
=================

Step 1 
------

Install NodeJS and get npm to run. 

Step 2
------

Create Anaconda Virtual Environment 

Step 3 
-----

Installing...

**Solidity Compiler**
(https://docs.soliditylang.org/en/v0.8.13/installing-solidity.html)

``npm install -g solc`` 

**Brownie**
(https://eth-brownie.readthedocs.io/en/stable/install.html)

``pip install eth-brownie``

**Ganache**
(https://trufflesuite.com/docs/ganache/)

``npm install -g ganache-cli`` or ``npm install -g ganache``

use ``sudo`` on Mac to have Admin rights. 

or 

Install yarn: ``npm install --global yarn``

``yarn global add ganache-cli`` or ``yarn global add ganache``

**OpenZeppelin**
(https://docs.openzeppelin.com/contracts/4.x/)

``npm install @openzeppelin/contracts`` 

**Web3.py**
(https://web3py.readthedocs.io/en/stable/quickstart.html)

``pip install web3``

Step 4
----

``pip install eth-brownie``
or 
``pip3 install eth-brownie``

check if Brownie works
``brownie``

**Networks**


Check Brownie networks: 

``brownie networks list``

Check Brownie networks details: 

``brownie networks list true``

Add Networks to Brownie networks: 

``brownie networks add [environment] [networkID] host=[host] chainid=[chainid]``
e.g.
``brownie networks add Ethereum moralis-rinkeby host=https://speedy-nodes-nyc.moralis.io/70cbea161463fe***/eth/rinkeby chainid=4`` 

More Infos about Networks: https://www.codeforests.com/2022/01/27/python-brownie-network-setup/

**Bake Token**


**Create a token**

``mkdir yourtoken``

``cd yourtoken``

``brownie bake token``

``cd token`` 

**Get enpoint for token**

e.g. Moralis ``brownie networks add Ethereum moralis-rinkeby host=https://speedy-nodes-nyc.moralis.io/70cbea161463fe***/eth/rinkeby chainid=4`` 

**Create Testing Account**

``brownie accounts generate testaccount``

**Get test ETH**

Needed to pay for gas fees. 

https://faucet.egorfine.com/

**Move to correct folder**

FileNotFoundError: ``cd ./token``

**Deploy contract**

``brownie compile``

**Modify deploy.py**

``acct = accounts.load('testaccount')``

``return Token.deploy("Test Token", "TST", 18, 1e21, {'from': acct})``

**Deploy contract**

``brownie run token.py --network moralis-rinkeby``

Source: https://www.quicknode.com/guides/web3-sdks/how-to-deploy-a-smart-contract-with-brownie


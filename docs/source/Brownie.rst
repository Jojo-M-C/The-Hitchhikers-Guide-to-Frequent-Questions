Brownie: A brief note on how to bake  
====

``pip install eth-brownie``
or 
``pip3 install eth-brownie``

check if Brownie works
``brownie``

Networks
----

Check Brownie networks: 

``brownie networks list``

Check Brownie networks details: 

``brownie networks list true``

Add Networks to Brownie networks: 

``brownie networks add [environment] [networkID] host=[host] chainid=[chainid]``
e.g.
``brownie networks add Ethereum moralis-rinkeby host=https://speedy-nodes-nyc.moralis.io/70cbea161463fe***/eth/rinkeby chainid=4`` 

More Infos about Networks: https://www.codeforests.com/2022/01/27/python-brownie-network-setup/

Bake Token 
----

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
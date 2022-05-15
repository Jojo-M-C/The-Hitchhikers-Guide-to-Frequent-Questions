Local test-blockchain 
========

Truffle: The Ganache of Testing
---------

https://trufflesuite.com/docs/truffle/

Use truffle boxes
-------

1. ``mkdir MetaCoin``

2. ``cd MetaCoin``

3. ``truffle unbox NAME``

Note: You can use any truffle box https://trufflesuite.com/boxes/ 

Create empty project 
-------

``truffle init``

Setting up a local blockchain 
-------

``npm install --save-dev ganache-cli``

``npx ganache-cli --deterministic`` will by default return ``127.0.0.1:8545``

Modify **deploy.js**

Uncomment needed settings in **truffle-config.js**

Open new terminal and run ``truffle migrate``


Interacting with the local blockchain 
--------

``npx truffle console --network development``

Syntax 
------

https://docs.openzeppelin.com/learn/deploying-and-interacting
https://trufflesuite.com/docs/truffle/getting-started/interacting-with-your-contracts/






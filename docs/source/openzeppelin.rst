OpenZeppelin
========

Contracts 
---
https://docs.openzeppelin.com/contracts/4.x/

Cli
----
https://docs.openzeppelin.com/cli/2.8/

Install 
------

``npm install @openzeppelin/contracts``

``npm install @openzeppelin/cli``

Step by Step
----

``mkdir ProjctName && cd ProjectName``

``npm init -y``

``npx openzeppelin init``

OpenZeppelin Ethereum Packages
----

``npx oz link @openzeppelin/contracts-ethereum-package``

Deploy OpenZeppelin x Ganache 
-----

``npx ganache-cli --deterministic``

**Deploy**

``npx oz deploy``

**Interact**

``npx oz accounts``

``npx oz send-tx``

``npx oz balance --erc20 CONTRACTADDRESS```

**upgrade**

Change something. 

``px oz compile``

``npx oz upgrade``

Deploy OpenZeppelin x Testnets
-----




Test
----

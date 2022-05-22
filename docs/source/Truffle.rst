Truffle 
=======

Deploy 
-----

1. Initalize new project 

``truffle init`` 

3. create Contracts 


2. Modify "1_initial_migrations.js"


3. Create mnemonics

``npx mnemonics``

4. Create secrets.json 

.. code:: yaml

    {
        "mnemonic": "repair derive axis lunch hockey air wealth market detail bicycle mixed shiver"
    }

5. Install hfwallet-provider

``npm install @truffle/hdwallet-provider``

6. Modify truffle-config.js

.. code:: yaml

    
    const HDWalletProvider = require('@truffle/hdwallet-provider');

    const mnemonic = require("./secrets.json").mnemonic;

    module.exports = {

    networks: {

        ropsten: {
        provider: () => new HDWalletProvider(mnemonic, `https://ropsten.infura.io/v3/wss://speedy-nodes-nyc.moralis.io/30f9d049c*****941/eth/ropsten/ws`),
        network_id: 3,       // Ropsten's id
        gas: 5500000,        // Ropsten has a lower block limit than mainnet
        confirmations: 2,    // # of confs to wait between deployments. (default: 0)
        timeoutBlocks: 200,  // # of blocks before a deployment times out  (minimum/default: 50)
        skipDryRun: true     // Skip dry run before migrations? (default: false for public nets )
        },

    },

    // Set default mocha options here, use special reporters etc.
    mocha: {
    // timeout: 100000
    },

    // Configure your compilers
    compilers: {
        solc: {
        version: "0.8.13",      // Fetch exact version from solc-bin (default: truffle's version)
        // docker: true,        // Use "0.5.1" you've installed locally with docker (default: false)
        // settings: {          // See the solidity docs for advice about optimization and evmVersion
        //  optimizer: {
        //    enabled: false,
        //    runs: 200
        //  },
        //  evmVersion: "byzantium"
        // }
        }
    },

    };


7. Paste Moralis Speedy-Nodes (WWS)

8. Enter Truffle Console 

``truffle console --network ropsten``

9. Get accounts

``await web3.eth.getAccounts()``

10. Transfer eth to the first one (via Metamask)


11. Get balance 

``await web3.eth.getBalance("ADDRESS")``

12. Migrate 

``migrate``

13. Check Etherscan 

Interacting 
---------

**Get address**

``NAME.address``

Truffle X OpenZeppelin 
------------

1. Import OZ contracts 

``import "@opzenzeppelin/..."``

2. Initalize project 

``npm init -y``

3. Install @openzeppelin/contracts 

``npm install @openzeppelin/contracts``

Note: this will create a nodes_modules folder in your repository. 

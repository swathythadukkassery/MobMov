Track-e-Hazard

MobMov is a decentralised app which tracks the lifecycle of a smartphone and thereby analysing its quality during different stages .

Prerequisites:
Install the following

	-Node Package Manager
	-Ganache
	-Truffle
	-Solidity Programming Language
	-MetaMask Chrome Extension
	
Running the tests
	contracts directory:Here is where all the smart contracts reside.

	migrations directory:Whenever we deploy smart contracts to the blockchain we are updating the blockchain state by 	        the process of migration.All these migration files are in this directory.

	build directory:This is home of all node dependencies which includes change of ownerships among the nodes,                  migrations and product management
	
	web directory:This is where the client-side application is developed, i.e. UI.

	truffle:Truffle framework is what allows us to build dApps on the ethereum blockchain.This file is the main 	configuration file for all the above mention directories.

Ganache provides us with fake ethers a number of accounts.Each account represents a node.Thus when a transaction is made the corresponding changes will be reflected in the ganache.

ChangeOfOwnership.deployed().then(function(instance) {app = instance})
Here changeOfOwnership is the name of the variable we created in the migration file.We retreived a deployed instance of the contract with the deployed function and assigned it to an app variable inside the promises callback function.

# **Turant-Pay (Cross Border Settlement) by XDC01 Protocol**

Turant Pay is a P2P Remittance standard built on the XDC Protocol. The standard is being designed to be pluggable by regulated remittance entities following the strict KYC/AML process and use XDC as a digital asset to relay liquidity from one peer to another across geographically spread locations and fiat currencies.

For many businesses, individuals and government agencies, making or receiving payments that cross borders is a necessary activity. Many businesses serve customers abroad and rely on buying goods from suppliers abroad but, in order to do so, they need to be able to receive payments from those customers and make them to those suppliers. Similarly, many people depend on the ability to readily send or receive cross-border payments, such as migrants who send money to families in their home countries or individuals who make online purchases from foreign retailers.

# **Fabric Components**


**XDC Nodes** : "Node" refers to a logical and not necessarily physical separation of function. Clients are the end-user facing nodes. XDC01 architecture provides multiple interfaces to the blockchain. Users (which may be application software) send transaction requests to the XDC01 network using these interfaces via a client node.

**Peer** - Peers maintain the state of the ledger by executing Xinfin Blockchain and participating in consensus formation. XDC01 blockchain/smart contract which are the business rules is installed on peers. Smart contracts are central to Xinfin blockchain networks as they dictate the rules of the "card" game that is the blockchain network. A Peer does not create new blocks but it validates blocks and transactions.

**XDC01 Blockchain** - We will be looking at permission/managed/private blockchain where organizations are required to get consent from membership authorities to join the XDC01 network. This is not the case with bitcoin and other coins where the network is "public" and is free for all!

# **Transaction Flow** 

Let's see how nodes work together to execute a transaction. For now, let's assume that the chaincode is already installed on the Peers.

**Step 1:** Transaction requests are proposed by a client. The client must be connected to the required number of peers according to the endorsement policy. A proposed Transaction is forwarded to Peers for Endorsement.

**Step 2:** Each endorsing peer simulates and validates the transaction. Peers reply with their Endorsement and certificate if they agree that the transaction is permitted.

**Step 3:** The client receives results from different Peers and can thus verify agreement among the Peers. Upon verification, the client forwards the transaction to the OS.

**Step 4:** Determining a well-ordered sequence of transactions is the task of the Ordering Service (OS). The OS generates transaction blocks containing validated transactions in the order they are deemed to have occurred, writes them to the ledger and then broadcasts them to all peers that a new set of blocks are now available on the ledger.


# **Key Features**

**Distributed :**  

Direct account-to-account settlement with no central operator
Decentralized global market for competitive FX

**Secure:** 

Transactions are cryptographically signed using ECDSA or Ed25519
Multi-signing capabilities

**Scalable :** 

Capacity to process the world’s cross-border payments volume
Easy access to liquidity through a competitive FX marketplace


XDC explorer provides an interface to look at the overall network. The explorer is accessible through a web browser and updates in real-time when transactions are invoked on the ledger, as shown below.

![](https://i.imgur.com/DuAF6JV.jpg)

title: Testnet
comments: false
---

## Testnet
Metaverse testnet is officially available for users to develop, debug and test.
The cost of the test is paid by the ETP of the test network, which are not real ones but can be applied for free from the official website.

All the block data of the test net are independent from the main net. The testnet can be used to develop simple functions, such as the functionality of registering asset, which can be transferred to the main net to run.
The official website of Metaverse has been updated for users to experience the wallet function. The Metaverse official website <https://mvs.org> has added "Testnet Button".

## Testnet Features
1.  Users can experience the Metaverse Wallet without expending their own ETP.
2.  Users need not sync the entire blockchain, saving time.
3.  Users can experience transferring and issuing assets, and carry out secondary issuances. 
4.  Robust page and platform compatibility.
5.  An improved wallet program that greatly reduces consumption of system resources.
6.  Added multi-signature addresses and multi-signature transactions.
7.  Enhanced wallet UI.

## Start the full node wallet in the testnet mode
* You need to use commant-line to run.
```bash
mvsd -t
```
* Register
```bash
mvs-cli getnewaccount testaccout testpasswd
```

* Start CPU mining.
```bash
mvs-cli start testaccount testpasswd
```

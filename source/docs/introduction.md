Introduction
comments: false
---

MVS，short for Metaverse

## Metaverse full node introduction
Full nodes are ones that store all the data of the MVS blockchain and are connected to the blockchain network in a P2P manner. All nodes in the blockchain network are equal which act as both clients and servers.

The MVS full node consists of two programs and a set of front-end resource:
* mvsd: The core wallet program, which is similar to bitcoind in bitcoin;
* mvs-cli: an interactive tool of the command-line that is similar to bitcoin-cli in bitcoin;
* mvs-htmls: the angularjs implementation which belongs to browser-based front-end interactive resources. This resource is not required for developers.


## MVS full nodes wallet download address:

Generally, the latest MVS full node client could be downloaded from Metaverse official website (https://mvs.org#download)


Supported versions:

| OS Version                        | Version | mvsd&mvs-cli |
| --------------------------------- | ------- | ----------------- |
| Red Hat Enterprise Linux 7 Server | 7+|   √               |
| Ubuntu                        | 14.04+ |   √               |
| Debian                            | 8+|   √               |
| Fedora                            | 21+|   √               |
| CentOS                            | 6.5+|   √               |
| openSUSE                      | 13.2+ |   √               |
| Docker                            | -     |   √               |

## Function list of the MVS full nodes wallet
|                 | mvsd&mvs-cli | Broswer GUI |
| --------------- | ---- | ---- |
|Graphic Interfac          |       |   √    |
|Command Line Interface        |   √   |   √    |
|Create Account     |   √   |   √    |
|Import and Export Mnemonics   |   √   |   √    |
|Create Address     |   √   |   √    |
|Batch Generation Address      |   √   |   √    |    
|ETP Transfer           |   √   |   √    |  
|ETP Deposit (Coinlock)     |   √   |   √    |
|Show All Addresse      |   √   |   √    |
|Show All Assets      |   √   |   √    |
|Create Asset (Not broadcast)  |   √   |   √    |
|Delete Asset (Not broadcast)  |   √   |        |
|Issue Asset          |   √   |   √    |
|Transfer Asset|   √   |   √    |
|Create a multi-party signature transactio  |   √   |   √    |
|Offline signature          |   √   |        |
|List the transaction details of the designated assets of the wallet|   √   |    √    |
|mining            |   √   |        |


## Port descriptions

The firewall port needs to be opened if external programs are allowed to access the node's API. The following is port descriptions which can be partially or thoroughly open as required.


|                    | Main Net | Test Net |
| ------------------ | ------------ | ------------- |
| JSON-RPC via HTTPS | ×    | ×    |
| JSON-RPC via HTTP  | 8820 | 8820 |
| P2P via TCP        | 5251 | 15251|


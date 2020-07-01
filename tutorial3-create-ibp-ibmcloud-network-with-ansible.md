---
# Related publishing issue: https://github.ibm.com/IBMCode/Code-Tutorials/issues/493

abstract: "Use the IBM Blockchain Platform VS Code extension to upgrade an existing commercial paper smart contract easily, and add further query capability."

authors:
  - name: "Paul O'Mahony"
    email: "mahoney@uk.ibm.com"

# collections:		# Required=false

completed_date:	"2020-06-21"

components:
  - "hyperledger-fabric"
  - "hyperledger"
  - "vscode-extension"
  
draft: true

excerpt: "Use the IBM Blockchain Platform VS Code extension to upgrade an existing commercial paper smart contract easily, and add further query capability."

last_updated:	"2020-06-21"

meta_description: "Use the IBM Blockchain Platform VS Code extension to upgrade an existing commercial paper smart contract easily, and add further query capability."

meta_keywords: "commercial paper, queries, smart contract, IBM blockchain, IBM blockchain platform, VS Code extension, Hyperledger Fabric"

meta_title: "Enhance query functionality: Add deltas history to your commercial paper sample using the IBM Blockchain VS Code extension"

primary_tag: "blockchain"

pta:
 - "emerging technology and industry"

pwg:
  - "blockchain"

related_content:
  - type: "tutorials"
    slug: "queries-commercial-paper-smart-contract-ibm-blockchain-vscode-extension"
  - type: "tutorials"
    slug: "run-commercial-paper-smart-contract-with-ibm-blockchain-vscode-extension"
  - type: "patterns"
    slug: "create-and-execute-blockchain-smart-contracts"

related_links:
  - title: "Video: Start developing with the IBM Blockchain Platform VS Code Extension"
    url: "https://youtu.be/0NkGGIUPhqk"
  - title: "Sample commercial paper smart contract"
    url: "https://github.com/hyperledger/fabric-samples"
  - title: "Hyperledger Fabric docs: Commercial paper tutorial"
    url: "https://hyperledger-fabric.readthedocs.io/en/master/tutorial/commercial_paper.html"

# runtimes:

services:
  - "blockchain"

subtitle: "Upgrade an existing commercial paper smart contract easily and add further query capability"

tags:
  - "finance"

title: "Upgrade a commercial paper smart contract by adding deltas history query capability"

# translators:		# Required=false The list of persons who assisted in translation.
#   - name:
#     email:

type: tutorial

---

In the previous tutorial [tutorial 2](https://developer.ibm.com/tutorials/queries-commercial-paper-smart-contract-ibm-blockchain-vscode-extension), I showed you how, as a developer, you can add rich query functionality and enhance your smart contract using the IBM Blockchain VS Code extension. That tutorial enabled you to query the history and lifecycle of a commercial paper instance and report on it. Showing that immutable history is of course important, but what if you just want to know, for example, what changes were committed for each transaction in that history? Such a use case is relevant when you're dealing with large volumes of transactions, when you're looking for patterns, etc.

In this tutorial, you will provision a full blockchain network, consisting of 3 organisations in IBM Blockchain Platform in IBM Cloud. 

Having successfully upgraded the Commercial Paper smart contract ( on the'Commerce' network) in [tutorial 2](https://github.com/mahoney1/commercialpaper/blob/master/tutorial2-queries-commercial-paper-smart-contract-ibm-blockchain-vscode-extension.md), MagnetoCorp, DigiBank and Hedgematic - all part of the blockchain consortium - wish to deploy the new contract on their network in IBM Blockchain Platform in IBM Cloud. In this tutorial, you'll automatically provision this network, then deploy the smart contract. The last part will show you how client applications from any organisation, can interact with the ledger data - ie 'business as usual'.

**Figure 1. Overview diagram**

![Overview diagram](images/ibp-cons-summary.png)


## Prerequisites

1. You need to have completed the previous two tutorials in this series.
2. Specifically, you will have version 0.0.2 of the commercial paper smart contract package `papercontract` package available under the `Smart Contracts` view in the IBM Blockchain Platform VS Code extension.

4.

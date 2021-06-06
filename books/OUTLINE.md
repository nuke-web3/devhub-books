# Substrate Overview (for everyone, not just devs)

start with why -> how -> what inspiration & guide: [https://www.freshworks.com/crm/sales/summary-of-start-with-why-blog/](https://www.freshworks.com/crm/sales/summary-of-start-with-why-blog/)- [https://www.youtube.com/watch?v=qp0HIF3SfI4](https://www.youtube.com/watch?v=qp0HIF3SfI4)

Those sold on developing with substrate are prompted to enter here Substrate Starter Track: The place everyone developing should start with.
Invite people to skip  ahead, but only at their own risk, as this track is fundamental to  understanding the key features of substrate!

## Before you begin
Read only
### Rust “starter kit” book companion
Read only, do with combination of rustbook
### Overview of Devhub
Read only
### Why devhub?
Read only
### What is substrate?
Read only
### Install
Do
### First Chain
Do and learn

- [https://substrate.dev/docs/en/tutorials/create-your-first-substrate-chain/](https://substrate.dev/docs/en/tutorials/create-your-first-substrate-chain/)
- {remove background, already in architecture}
- {add overview of ways to build substrate and say we will focus on FRAME}
	- [https://substrate.dev/docs/en/](https://substrate.dev/docs/en/)
- {remove “learn more”, keep on track}

### FRAME Overview
Read Only

- [https://substrate.dev/docs/en/knowledgebase/runtime/](https://substrate.dev/docs/en/knowledgebase/runtime/)
- [https://substrate.dev/docs/en/knowledgebase/runtime/frame](https://substrate.dev/docs/en/knowledgebase/runtime/frame)
	- combine above two into one?
- [https://substrate.dev/docs/en/knowledgebase/runtime/pallets](https://substrate.dev/docs/en/knowledgebase/runtime/pallets)
- [https://substrate.dev/docs/en/knowledgebase/learn-substrate/extrinsics](https://substrate.dev/docs/en/knowledgebase/learn-substrate/extrinsics)

### Add a FRAME Pallet
Do and learn

- [https://substrate.dev/docs/en/tutorials/add-a-pallet/](https://substrate.dev/docs/en/tutorials/add-a-pallet/)
	- Kitties: Add Identity pallet instead of Nicks? Or swap latter on?
- {remove “learn more”, keep on track}
- point to the libraries of pallets and encourage going README deep into a few
that catch your eye in substrate and ORML and more… Then come back here
to continue

### Interact With Your Custom Node

- {extend / move custom UI element from last add a pallet here}
- [https://substrate.dev/docs/en/knowledgebase/integrate/polkadot-js](https://substrate.dev/docs/en/knowledgebase/integrate/polkadot-js)
- [https://substrate.dev/docs/en/knowledgebase/integrate/libraries](https://substrate.dev/docs/en/knowledgebase/integrate/libraries)
	- Combine? Note that the JS libs are most supported.
	- bring in key examples from polkadot.js docs, or reference to them
		- metadata being most important - need a page for this… but MAYBE not needed soon (WIP PR on substrate for transparent metadata)
		- This can be in a separate “branch” track for substrate client development/use

### Pallet Engineering Overview

- [https://substrate.dev/docs/en/knowledgebase/runtime/](https://substrate.dev/docs/en/knowledgebase/runtime/)
	- Presently used as a reference set of pages, not meant to be read linearly more than this one time , crosslinked throughout.
	- Vision: cater content to the runtime “branch” of content that most will follow after this main “trunk” of content in a linear flow. Put all "odd balls" in reference pages, and plan to insert into latter tracks
- Revisit Rust fundamentals in substrate context based on substrate kitties slides: [https://docs.google.com/presentation/d/1dhaoLb5V2K_vDe4EJlUcKwePD1nMktr57fOdSo8bHns/edit#slide=id.g51f30cead3_0_14](https://docs.google.com/presentation/d/1dhaoLb5V2K_vDe4EJlUcKwePD1nMktr57fOdSo8bHns/edit#slide=id.g51f30cead3_0_14)
	- Include specific rust syntax examples and explanations that you need in rust along the way
	- Point to the [substrate example pallet](https://github.com/paritytech/substrate/tree/master/frame/example) for the comments with in depth explanations.

### Create Your First dApp

- [https://substrate.dev/docs/en/tutorials/create-a-pallet/](https://substrate.dev/docs/en/tutorials/create-a-pallet/)
	- Use the [substrate example pallet](https://github.com/paritytech/substrate/tree/master/frame/example) as a base? Instead of the template pallet. But use a *specific* commit to avoid any upgrades "breaking" the tutorial. Alternatively use the template pallet, and add more comments to match the example pallet.
	- End result is a minimal NFT pallet
- [https://substrate.dev/docs/en/tutorials/build-a-dapp/pallet](https://substrate.dev/docs/en/tutorials/build-a-dapp/pallet)
	- Reworked to build the NFT UI

### Start a Network

- [https://substrate.dev/docs/en/tutorials/start-a-private-network/](https://substrate.dev/docs/en/tutorials/start-a-private-network/)
- launch FAQ for testing -> prod

---

##

## Devhub Track Structure:

###

### Runtime Engineer (main trunk for more branches)

- [https://substrate.dev/docs/en/knowledgebase/runtime/](https://substrate.dev/docs/en/knowledgebase/runtime/) Mostly keep this, but address the flow and remove redundancy with main trunk (assume they did this, reference it)
- [https://substrate.dev/docs/en/tutorials/visualize-node-metrics/](https://substrate.dev/docs/en/tutorials/visualize-node-metrics/)

###

### Pallet Design & Interaction (201)

- DO: [https://substrate.dev/docs/en/tutorials/create-a-pallet/](https://substrate.dev/docs/en/tutorials/create-a-pallet/)
- Storage [https://substrate.dev/docs/en/knowledgebase/advanced/storage](https://substrate.dev/docs/en/knowledgebase/advanced/storage)
- SCALE [https://substrate.dev/docs/en/knowledgebase/advanced/codec](https://substrate.dev/docs/en/knowledgebase/advanced/codec)
- DO: [https://substrate.dev/docs/en/tutorials/create-a-pallet/](https://substrate.dev/docs/en/tutorials/create-a-pallet/)
- RPC / API interface
- Community resources (ORML, etc.)
- Reference “leaves” : specializations on types like gov, tokens, … all for the solo-chain context )in the form of “how-to guides”
- DO: [https://substrate.dev/recipes/pallet-coupling.html](https://substrate.dev/recipes/pallet-coupling.html)
- explore: [https://github.com/substrate-developer-hub/awesome-substrate](https://github.com/substrate-developer-hub/awesome-substrate)

###

### Runtime Upgrades & Storage Migrations

- [https://substrate.dev/docs/en/tutorials/forkless-upgrade/](https://substrate.dev/docs/en/tutorials/forkless-upgrade/)
- {upcoming content on migrations here}
	- [https://github.com/substrate-developer-hub/migration-example](https://github.com/substrate-developer-hub/migration-example)

###

### Advanced Topics

- Extend & Go Beyond FRAME
	- Use this as basis [https://substrate.dev/docs/en/#usage](https://substrate.dev/docs/en/#usage)
	- Executor interface [https://substrate.dev/docs/en/knowledgebase/advanced/executor](https://substrate.dev/docs/en/knowledgebase/advanced/executor)
- [https://substrate.dev/docs/en/knowledgebase/advanced/](https://substrate.dev/docs/en/knowledgebase/advanced/) most of these not already incorporated
- [https://substrate.dev/docs/en/knowledgebase/advanced/ss58-address-format](https://substrate.dev/docs/en/knowledgebase/advanced/ss58-address-format)

###

### Parachain Engineer

```
(RE branch not strictly required, but encouraged)

```

###

### Solo-chain vs. Parachain

- [https://substrate.dev/docs/en/knowledgebase/advanced/consensus](https://substrate.dev/docs/en/knowledgebase/advanced/consensus)
- (Kian’s office hour for SBP here)
-

###

### Cumulus

- read and/or port into devhub: [https://polkadot.network/the-path-of-a-parachain-block/](https://polkadot.network/the-path-of-a-parachain-block/)
- DO: [https://substrate.dev/cumulus-workshop/](https://substrate.dev/cumulus-workshop/)
-
- runtime upgrades of relay chain & parachains

###

### XCM, XCMP, HMP VMP, …

###

### Para-light clients

```
Full nodes for validator & collator needed now, but not forever

```

###

### Smart Contracts

```
(RE branch not strictly required, but encouraged)
Point out that pallets can and should be the go-to for any *standard* contact patterns. See Statemint for an analog: it's a "token factory" for ERC20 like tokens.

```

###

### Frontier, EVM

- [https://substrate.dev/frontier-workshop/#/](https://substrate.dev/frontier-workshop/#/)

###

### Contacts pallet, ink!

- [https://substrate.dev/docs/en/knowledgebase/smart-contracts/overview](https://substrate.dev/docs/en/knowledgebase/smart-contracts/overview) basically same flow as this section of devhub
- [https://substrate.dev/substrate-contracts-workshop/#/](https://substrate.dev/substrate-contracts-workshop/#/)
- [https://substrate.dev/docs/en/tutorials/add-contracts-pallet/](https://substrate.dev/docs/en/tutorials/add-contracts-pallet/)

###

### Offchain Workers

###

### Oracles

###

### Heavy Operations

```
Using only one node for processing possible

```

###

### Solo-chains

- Private, permissioned, hybrid
	- [https://substrate.dev/docs/en/tutorials/build-permission-network/](https://substrate.dev/docs/en/tutorials/build-permission-network/)
	- [https://github.com/substrate-developer-hub/substrate-enterprise-sample](https://github.com/substrate-developer-hub/substrate-enterprise-sample)
	-

###

### Node Clients

```
communicating with substrate-based nodes

```

- most of the [https://substrate.dev/docs/en/knowledgebase/integrate/](https://substrate.dev/docs/en/knowledgebase/integrate/) section can be ported here.
- also in RE track, but good to have here in the flow: [https://substrate.dev/docs/en/tutorials/visualize-node-metrics/](https://substrate.dev/docs/en/tutorials/visualize-node-metrics/)
- how-to guides on runtime upgrades and storage migrations. (metadata)
- explore: [https://github.com/substrate-developer-hub/awesome-substrate](https://github.com/substrate-developer-hub/awesome-substrate)

---
title: Developers
description: 
published: true
date: 2021-03-02T18:07:23.136Z
tags: 
editor: markdown
dateCreated: 2021-02-24T08:19:45.758Z
---

> Ergo enables new models of financial interaction, underpinned by smart contracts built on flexible and powerful Sigma protocols but easily accessible to developers.
{.is-info}



One of the most exciting things about blockchain is the possibility of making digital agreements without any trusted intermediaries. In the simplest use case, pioneered by Bitcoin, Alice can send a payment directly to Bob, wherever the two of them are located around the world, with no bank or any trusted third party needed. However, with the functionality of a modern blockchain like Ergo, it is possible to make far more complex and sophisticated financial agreements than simple payments. Take the following example.

Gold-backed tokens Alice uses ERGs to purchase gold-backed tokens from Bob. Bob stores the gold in a secure vault, and uses the blockchain to issue one token for every Troy ounce of gold he has. Alice can then use these tokens freely in different contracts, transferring and trading them under whatever conditions she specifies in the smart contract code. When Alice wants to sell the tokens for physical gold, she can conduct another transaction with Bob, receiving ERG in return, at market price.

The point of blockchain contracts is to eliminate the need for trust. While the purchase transaction is now trustless, in this instance Alice still needs to trust Bob about two things. Firstly, Bob may refuse to swap the gold tokens back to ERG at the correct price when Alice wants to sell. Secondly, Bob may default on his obligations – running away with the gold, or misusing the funds he receives and running a fractional reserve.

Extending the contracts To address these issues, we can create an Oracle, or decentralised price feed. This uses multiple sources of external data to record the price of gold to the blockchain at regular intervals. This price feed will be the reference point for the redemption contract that manages the sale of Alice’s gold with Bob (or any other participant). Thus the system automatically enforces the right price when a swap takes place.

The second situation requires a third-party insurer, Charlie, whose service is also hosted on the blockchain with a smart contract. When Alice purchases gold from Bob, she additionally buys an insurance contract from Charlie. The payment can be dependent on factors including the amount of insurance required, and Bob’s reputation – again, managed by a decentralized feedback mechanism. Now, if Bob defaults, Alice will automatically receive the value of her gold tokens, with Charlie effectively acting as a buyer of last resort.

Programmable contracts There are, of course, many other example use cases like this one. We can also extend this use case, adding further economic actors. For example, Charlie may sell shares in his insurance business to Dave and other participants, providing them with a proportion of revenues in return for ensuring he has the capital he needs to cover any liabilities from the outset.

However, even the most complex use case is simpler than general-purpose software that can be used to program any contract. After all, generalised logic must be both far-reaching and secure. Moreover, even a specialised contract is made up of many steps, each of which is fairly simple. Thus another requirement for a general-purpose platform is that it should simplify the process of writing contracts, making them as accessible (and safe) as possible. This can be achieved with the use of template agreements, with customisable parameters. The insurance contract above could be based on a module with flexible parameters, for example. This could be used and reused in many different circumstances.

Ergo’s approach This is essentially the approach that Ergo takes, providing superior support for real-world financial agreements. It does this through:

-     Support for multi-stage contracts (watch details for developers)
-     A simple high-level language, ErgoScript, enabling clear descriptions of contractual logic
-     Support for formal verification of contracts for improved security guarantees (Ergo Platform deployed its first formally verified p2p crowdfunding contract just three months after the network launched)
-     Easy Oracle creation
-     Native support for complex signature schemes In short, creating financial contracts on the blockchain isn’t just about the functionality you provide. It’s about making that functionality safe and accessible, as well as powerful. Ergo achieves this and more.

Share post:


# Overview

- ErgoAppKit
- ErgoTool : A CLI for Errgo
- Scorex (2) - The modular blockchain framework
- Multi-signatures - distributed-signatures
- [ErgoTool:](https://github.com/Emurgo/ergo-node-interface) A Command Line Interface for Ergo
- ErgoScan: Ergo block explorer interface
- Ergo-js
- Ergo-Bootstrap: easy to use tool with cluster deployments for dApp development
- Sigma-rust
- Ergo Appkit: library for polyglot development of Ergo Applications based on GraalVM
- Tx Builder - Interact with dApps without writing code
- [ErgoScript Playground](https://github.com/ergoplatform/ergoscript-by-example)
- ErgoTree compiler 
- Kiosk

# Proposed Nautilus ZK Treasury

This basic concept is to create a visual programming toolkit to assist developers in learning and developing contracts in the EUTXO model. 

This toolkit will initially be built on top of Ergo Playground.  

The goal is to take advantage of the free composability offered by EUTXO. Create an open source library of visual, composable tools to onboard new developers. 

The “long term” goal is to create a headless central management system for developers, and a front-end UI focused central management system for basic users that are both interoperable with this visual programming toolkit. 

The name Nautilus is inspired by the Submarine in Jules Verne 20,000 Leagues Under the Sea. Nautilus is described by Verne as "a masterpiece containing masterpieces", which was built in secrecy, sourcing parts from unnamed sources and roams the seas beyond the reach of land-based governments.

# ErgoScript
Learn [Ergoscript by reading example smart contracts](https://github.com/ergoplatform/ergoscript-by-example) powered by the Ergo Playground.

Each contract example includes a `Ergo Playground` link which allows you to instantly edit and run the smart contract code inside of your browser.

If you ever need clarity about how specific types/functions/operators in ErgoScript work, please reference the [ErgoScript Language Description](https://github.com/ScorexFoundation/sigmastate-interpreter/blob/develop/docs/LangSpec.md).

For an overarching summary of how everything in this repo works, please reference the video below:

[ErgoScript By Example & Ergo Playground Introductory Video](https://www.youtube.com/watch?v=8l2v1asHgyA)





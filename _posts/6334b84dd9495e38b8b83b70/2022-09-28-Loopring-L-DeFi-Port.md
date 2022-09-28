---
layout: post
title:  "Loopring L2 DeFi Port"
description: "Last year we proposed the concept of EthPort, the purpose of which was to allow users to experience various Layer 1 DeFi products on Loopring Layer 2 in a decentralized manner. As part of the process…"
date: "2022-09-28 21:11:10"
categories: ['protocol', 'order', 'asset']
score: 56
image: "https://i.imgur.com/TUxyCba.jpg"
tags: ['protocol', 'order', 'asset']
link: "https://medium.loopring.io/loopring-l2-defi-port-cd6e811250a9"
---

Last year we proposed the concept of EthPort, the purpose of which was to allow users to experience various Layer 1 DeFi products on Loopring Layer 2 in a decentralized manner. As part of the process…

## Highlights

- Loopring L2 DeFi Port is now live on L2 and we chose ETH 2.0 staking via Lido as the first integrated DeFi product using it.
- The matching engine in this architecture diagram is responsible for settling sell orders and buy orders between users.
- As long as the price matches, the matching engine will execute the settlement in the order of the orders coming in first.
- When a user wants to withdraw from staking, we will provide a counterparty buy order based on the price of wstETH on L1.
- When there is a large deviation between funds deposited and withdrawn, it is necessary to rebalance funds to L2.
- The entire process of rebalancing funds is currently controlled automatically by smart contracts on

---

---
layout: post
title:  "97.7% of tokens traded on Uniswap May20-Sep21 were rug pulls | Academic Paper"
description: "Uniswap, as with other DEXs, has gained much attention this year because it is a non-custodial and publicly verifiable exchange that allows users to trade digital assets without trusted third parties. However, its simplicity and lack of regulation also make it easy to execute initial coin offering scams by listing non-valuable tokens. This method of performing scams is known as rug pull, a phenomenon that already exists in traditional finance but has become more relevant in DeFi. Various projects have contributed to detecting rug pulls in EVM compatible chains. However, the first longitudinal and academic step to detecting and characterizing scam tokens on Uniswap was made. The authors collected all the transactions related to the Uniswap V2 exchange and proposed a machine learning algorithm to label tokens as scams. However, the algorithm is only valuable for detecting scams accurately after they have been executed. This paper increases their dataset by 20K tokens and proposes a new methodology to label tokens as scams. After manually analyzing the data, we devised a theoretical classification of different malicious maneuvers in the Uniswap protocol. We propose various machine-learning-based algorithms with new, relevant features related to the token propagation and smart contract heuristics to detect potential rug pulls before they occur. In general, the models proposed achieved similar results. The best model obtained accuracy of 0.9936, recall of 0.9540, and precision of 0.9838 in distinguishing non-malicious tokens from scams prior to the malicious maneuver."
date: "2022-12-15 18:10:26"
categories: ['contract', 'machine', 'leveraging']
score: 153
image: "https://i.imgur.com/oGPejTr.jpg"
tags: ['contract', 'machine', 'leveraging']
link: "https://www.mdpi.com/2227-7390/10/6/949"
---

Uniswap, as with other DEXs, has gained much attention this year because it is a non-custodial and publicly verifiable exchange that allows users to trade digital assets without trusted third parties. However, its simplicity and lack of regulation also make it easy to execute initial coin offering scams by listing non-valuable tokens. This method of performing scams is known as rug pull, a phenomenon that already exists in traditional finance but has become more relevant in DeFi. Various projects have contributed to detecting rug pulls in EVM compatible chains. However, the first longitudinal and academic step to detecting and characterizing scam tokens on Uniswap was made. The authors collected all the transactions related to the Uniswap V2 exchange and proposed a machine learning algorithm to label tokens as scams. However, the algorithm is only valuable for detecting scams accurately after they have been executed. This paper increases their dataset by 20K tokens and proposes a new methodology to label tokens as scams. After manually analyzing the data, we devised a theoretical classification of different malicious maneuvers in the Uniswap protocol. We propose various machine-learning-based algorithms with new, relevant features related to the token propagation and smart contract heuristics to detect potential rug pulls before they occur. In general, the models proposed achieved similar results. The best model obtained accuracy of 0.9936, recall of 0.9540, and precision of 0.9838 in distinguishing non-malicious tokens from scams prior to the malicious maneuver.

## Highlights

- We are the first to design an accurate automated rug pull detection to predict future rug pulls and scams using relevant features of the pool’s state and the token distribution among the users.
- We show that 90% of tokens using locking contracts tend to become a rug pull or a malicious token eventually.
- We provide the most extensive labelled dataset of Uniswap rug pulls to date, including the source code, the liquidity, the prices, the mint/burn, and transfer events.
- The most common way in which scammers and malicious scammers execute a theft is a theft of a project is a malicious operation or set of operations in the cryptocurrency industry where the investors’ funds as profits.

---

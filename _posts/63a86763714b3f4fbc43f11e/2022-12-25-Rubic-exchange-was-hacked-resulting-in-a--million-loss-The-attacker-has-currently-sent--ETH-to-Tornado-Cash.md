---
layout: post
title:  "Rubic exchange was hacked, resulting in a $1.4 million loss. The attacker has currently sent 1100 ETH to Tornado Cash"
description: "Rubic is a cross-chain DEX aggregator. Users can exchange native tokens via the RubicProxy contract's routerCallNative function. Before redeeming, it will"
date: "2022-12-25 15:08:53"
categories: ['rubicproxy', 'users', 'protocol']
score: 21
image: "https://i.imgur.com/ZtFrXC4.jpg"
tags: ['rubicproxy', 'users', 'protocol']
link: "https://news.coincu.com/155231-rubic-lost-1-4-million-due-to-the-hack/"
---

Rubic is a cross-chain DEX aggregator. Users can exchange native tokens via the RubicProxy contract's routerCallNative function. Before redeeming, it will

## Highlights

- The multi-chain exchange protocol was hacked, resulting in a loss of more than 1.4 million US dollars.
- The attacker used the Tornado Cash mixing protocol to send 1,100 ETH to Tornado Cash.
- The main cause of the attack was that the protocol incorrectly added USDC tokens to the Router whitelist.
- USDC coins have also been placed to the Rubic protocol’s router whitelist, allowing any user to call USDC token randomly using Rubic proxy contract.
- The user-supplied target Router will be called only after the whitelist check, and the calling data will also be supplied by the user.
- However, malevolent users exploit this issue by calling the USDC contract using the.

---

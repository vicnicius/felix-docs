# Overview

Felix is a platform for running and playing different games of chance on the [Stacks blockchain](https://stacks.org/).

The first game we publish is the Felix Lottery, a smart-contract-based, provably fair Lottery. At first glance, the Lottery works as a simple lottery: players buy tickets with a unique number. At the end of the Lottery, the smart contract draws a verifiably random number, and if the player gets the ticket with a matching number, they get all the prizes in the pool.

But looking deeper, you'll see that the Felix Lottery is much more than that. It's a fully decentralized, trustless, and transparent lottery. Although the platform facilitates deploying and interacting with those lotteries, every aspect of the game runs on the chain, and Felix is not involved.

Moreover, Felix Lotteries are open and permissionless. You can even run one with others in the community, increasing the potential prize you can offer in a single Lottery. An attribute that makes Felix a platform not only for having the usual fun and thrills of playing a giant prize lottery but also for the more risk averse, the opportunity to play on the side that's usually controlled by a selected few.

A Felix Lottery will generally follow these stages:

## 1. Deployment

You start a lottery by choosing its parameters via our UI and deploying [the smart contract](/technical/smart-contract). You can decide how many funders you want to allow on your Lottery, how long it will last, the chances of winning each ticket, and the maximum number of tickets you'll want to sell, together with its price. For now, all lotteries will have STX as a token, but you can expect a broader range of tokens to be supported shortly. Once you've settled on the Lottery configuration, you can review the smart contract and deploy the LotteryLottery.

## 2. Funding

The deployed Lottery starts its on-chain life in the funding stage. At this stage, wallets can lock their STX to the Smart Contract to build the prize pool. Once the Lottery is active, the combined locked STX will be the Lottery prize. If there is a winning ticket, the ticket owner will take the prize at the end of the Lottery. If there is no winning ticket, the locked STX and their corresponding part of the sold ticket pool can be withdrawn from the contract by the funder.

## 3. Active

Active is the period when the Lottery sells tickets. The ticket is an NFT (SIP-009) unique to that Lottery with a number chosen by the buyer associated with it. Each buyer mints an NFT in exchange for a token price set by the Lottery owner, plus a 10% fee for the Felix platform. All the tokens collected during the ticket sell period are also locked in the smart contract.
The Lottery will be active for a predetermined amount of time. At the end of the active period, there's a cooldown of seven tenures (seven Bitcoin blocks), and then a random number can be drawn.

## 4. Finished

After the cooldown period, the Lottery draws a random number. If there's a winning ticket, the prize is sent to the winner. If there's no winning ticket, each funder can unlock their STX from the contract, together with their corresponding part of the sold tickets pool, which is equally divided among all funders. The sold tickets pool goes to the funders, with each taking an equal part, regardless of whether or not there was a ticket winner.

## Summary

The Felix Lottery is a fully decentralized, trustless, and transparent lottery. It's a platform for running and playing different games of chance on the Stacks blockchain. You can run your own Lottery, and you can even run one with others in the community, increasing the potential prize you can offer in a single Lottery. Felix is not involved in the game, and every aspect of the game runs on chain.

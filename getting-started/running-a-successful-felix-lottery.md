# Running a Successful Felix Lottery

{% hint style="warning" %}
### Disclaimer

Before moving on, check the Felix Lottery overview to understand the basic concepts.

Nothing on this document is financial advice. The information provided is for educational purposes only. You should always research and consider seeking professional advice before making financial decisions.

Before participating in Felix Lotteries, check your local laws and regulations. Felix is not responsible for any legal issues that may arise.
{% endhint %}

## Introduction

The Felix Lottery Platform offers users of the Stacks Blockchain a revolutionary take on lotteries: anyone can now run a Lottery, a position previously restricted to the State and a few selected others. Moreover, they can do it together with others in the community.

Running a Felix Lottery is an exciting way to have fun while making your STX (and other tokens) work for you. Reasons for using the Felix platform may vary: you might want to use it for charity, to fund other projects in the Stacks ecosystem, or to pursue personal goals. Regardless of your motivations, it's crucial to understand that running a Lottery comes with risks, and one must be extremely diligent.

We've created this guide to help Lottery creators make informed decisions and ensure a great and fair experience for funders and players.

## The Balance: Attractiveness vs Risk

A Felix Lottery has two interested parties: funders and players. Funders kickstart the game, and they decide the key attributes of the lottery when they deploy the smart contract on the blockchain. The perfect Felix Lottery is designed to appeal to both players and funders. It must strike the right balance between the attractiveness to players and the risk funders take.

The first basic principle of a lottery is that the more players participate in your lottery, the more revenue you can generate. There are three attributes that Lottery creators can adjust to influence a lottery's attractiveness to players:

1. How difficult it is to win
2. The potential payout for winners
3. The cost to play

Let's take a closer look at each of these attributes:

### Difficulty

The difficulty of a lottery is defined by the Felix Lottery difficulty setting. Difficulties range from one to ten. This directly translates to the number of digits the lottery-drawn number will be. For example, in a Felix Lottery of difficulty 1, a 1-digit number (from 0 to 9) will be drawn at its end to determine the winning ticket, if any. So a ticket has a one in ten chance of winning this Lottery. Here's a breakdown of the odds:

| Difficulty | Chance of winning per ticket (%) | Odds of winning per ticket |
| ---------- | -------------------------------- | -------------------------- |
| 1          | 10%                              | 1 in 10                    |
| 2          | 1%                               | 1 in 100                   |
| 3          | 0.1%                             | 1 in 1,000                 |
| 4          | 0.01%                            | 1 in 10,000                |
| 5          | 0.001%                           | 1 in 100,000               |
| 6          | 0.0001%                          | 1 in 1,000,000             |
| 7          | 0.00001%                         | 1 in 10,000,000            |
| 8          | 0.000001%                        | 1 in 100,000,000           |
| 9          | 0.0000001%                       | 1 in 1,000,000,000         |
| 10         | 0.00000001%                      | 1 in 10,000,000,000        |

For comparison, the chance of winning the grand prize in the Powerball Lottery is approximately 1 in 292,201,338, which would be comparable to a difficulty 8 Felix Lottery.

### The Prize

The lottery jackpot is a crucial factor in attracting players. Generally, the larger the jackpot, the more players will be drawn to the lottery. Felix Lottery runners control the jackpot size in two ways:

1. Defining what each funder will contribute to the prize pool
2. Determining how many funders a lottery can have

Funders have until the moment the Lottery starts to fund it. It's important to allow enough time for funders to lock their STX and build a substantial prize pool. Ideally, all lottery funders should be ready to send their fund transactions even before the Lottery is deployed. This ensures they know exactly what the prize pool will look like and can make more informed decisions on other attributes.

Splitting the composition of the prize pool among multiple funders is an effective way to mitigate risk. However, it also reduces the potential reward, as the Lottery sales revenue is equally divided among Lottery runners.

### The Price

Setting a fair price is essential for maximizing the number of players buying tickets for your lottery and, consequently, your revenue. Players won't be motivated to participate if a ticket is too expensive relative to the chances of winning or the prize. For example, paying 1 STX for a 1 in 1,000,000 chance of winning 5 STX is unlikely to attract many players.

Conversely, if tickets are too cheap, you might end up in a situation where the chances of a winning ticket are too high, but your revenue won't compensate for the loss of what you invested in the prize pool. For instance, if a lottery has a 1% chance of winning 200 STX and sells 100 tickets for 1 STX each, a savvy player would be inclined to buy all those tickets, guaranteeing the 200 STX prize while spending 100 STX, while you'd lose half your investment.

To manage this risk effectively, Felix Lottery creators must carefully consider ticket prices and the number of tickets for sale. A good approach is to find the "probabilistic break-even" point and then adjust your Lottery parameters from there.

### Finding the Probabilistic Break-Even

The probabilistic break-even for your lottery is the exact point where the chances of a winning ticket multiplied by the revenue from sales equal the investment you have locked in the prize pool. Mathematically, we can express it as:

$$
1/10^d * tp * ts = i
$$

Where:

* `d` is the Lottery Difficulty
* `tp` is the ticket price
* `ts` is the number of tickets for sale
* `i` is the investment locked in the prize pool

Here's an example:

Imagine you're investing 1000 STX in a Felix Lottery as the sole funder. The break-even point could look like this:

* 1 Funder
* 1000 STX Funded
* Lottery Difficulty: 3
* Ticket Price: 1 STX
* Tickets on Sale: 1000$

$$
1/10^3 * 1 * 1000 = 1000
$$

This equation holds, so your Lottery would break even in a perfect scenario. This means that if you sell all 1000 tickets, you'll recover your investment but make no profit. However, this Felix Lottery wouldn't be very attractive to its funder. After the 500th ticket sale, you've only recovered 50% of your investment, and the chances of keeping the locked prize (no one winning the lottery) are below 50%, decreasing with every sale.

### Building an Edge While Staying Attractive

To create a more advantageous situation for funders, you can adjust any of the three variables: difficulty, price, or tickets on sale. Let's modify our previous example:

#### Option 1: Increasing Difficulty

* 1 Funder
* 1000 STX Funded
* Lottery Difficulty: 4 (increased from 3)
* Ticket Price: 1 STX
* Tickets on Sale: 1000

If the Lottery sells all tickets, you will receive 1000 STX back from sales, and your chances of keeping the locked prize will be 90%. This gives funders a 90% chance of a 100% return. For players, they'd have a 1 in 10,000 chance of winning 1,000 STX per 1 STX ticket, which is still reasonable compared to traditional lotteries.

#### Option 2: Increasing Ticket Price

* 1 Funder
* 1000 STX Funded
* Lottery Difficulty: 3
* Ticket Price: 2 STX (increased from 1 STX)
* Tickets on Sale: 1000

If this Lottery sells all tickets, it would give its sole funder 2,000 STX in return. Even if only 500 tickets are sold, the funder would recover 1,000 STX and still have a 50% chance of keeping the locked STX. This creates an attractive edge for the funder while remaining appealing to players.

### Multiple Funders

Adding more funders changes the calculation slightly. With multiple funders, the amount you receive per sale is divided by the number of funders. For `n` funders, our formula becomes:

$$
1/10^d * tp * ts/n = l
$$

Where `n` is the number of funders, and `l` is the locked STX per funder.

Multiple funders can help hedge risk while maintaining the Lottery's attractiveness. For example, a 1000 STX lottery is likely more appealing to players than a 100 STX one. You could create a 1000 STX lottery by combining it with nine other funders while committing only 100 of your STX.

### Exotic Lotteries

With a good understanding of the balance between risk and attractiveness, you can create unique, attention-grabbing lotteries that remain balanced on the risk side. For example:

* 1 Funder
* 1000 STX Funded
* Lottery Difficulty: 1
* Ticket Price: 200 STX
* Tickets On Sale: 10

This Lottery offers easy odds (guessing a single-digit number correctly), but the high ticket price limits the number of participants. If you can convince ten players to participate, perhaps some high-stakes enthusiasts, you'd achieve a 100% return on your investment.

## Summary

When running your Lottery, strive to balance the appeal to players with the level of risk you're willing to accept. Use the principles outlined in this guide to ensure you strike this balance effectively.

Ensure you have funders ready before deploying your Lottery. Collaborating with other funders is often the best way to make your Lottery attractive while reducing the probability of losing money.

If you have feedback suggestions or notice any errors, please reach out to the team at https://x.com/felixonbitcoin.

# Running a Successful Felix Lottery

{% hint style="warning" %}
Before moving on, check the Felix Lottery overview to understand the basic concepts.

Nothing on this document is financial advice. The information provided is for educational purposes only. You should always research and consider seeking professional advice before making financial decisions.

Before participating in Felix Lotteries, check your local laws and regulations. Felix is not responsible for any legal issues that may arise.
{% endhint %}

{% hint style="warning" %}
This guide is still a draft. Please do your research and let us know if you spot any errors.
{% endhint %}

{% hint style="danger" %}
When we talk about the expected return in this guide, we mean it in **probabilistic** terms. If you ran 10,000s of this Lottery with these Lotterytes, you would get this value back on average.&#x20;

**For any Lottery run, you'll risk losing all your funds!**

Be diligent, do your research, and only spend what you can afford to lose.
{% endhint %}

## Introduction

The Felix Lottery Platform offers users of the Stacks Blockchain a revolutionary take on lotteries: anyone can now run a Lottery, a position previously restricted to the State and a few selected others. Moreover, they can do it together with others in the community.

Running a Felix Lottery is an exciting way to have fun while making your STX (and other tokens) work for you. Reasons for using the Felix platform may vary: you might want to use it for charity, to fund other projects in the Stacks ecosystem, or to pursue personal goals. Regardless of your motivations, it's crucial to understand that running a Lottery comes with risks, and one must be extremely diligent.

We've created this guide to help Lottery creators make informed decisions and ensure an excellent and fair experience for funders and players.

## The Balance: Attractiveness vs Risk

A Felix Lottery has two interested parties: funders and players. Funders kickstart the game and decide the critical attributes of the Lottery when they deploy the Lottery smart contract on the blockchain. A perfectly designed Felix Lottery will appeal to both players and funders. It must strike the right balance between the attractiveness to players and the risk funders take.

The first basic principle of a lottery is that the more players participate in your Lottery, the more revenue you can generate. There are three attributes that Lottery creators can adjust to influence a lottery's attractiveness to players:

1. How difficult it is to win
2. The potential payout for winners
3. The cost to play

Let's take a closer look at each of these attributes:

### Difficulty

The Felix Lottery difficulty setting defines the odds of a single ticket winning the Lottery. Difficulties range from one to ten. A Lottery difficulty directly translates to the number of digits the lottery-drawn number will be. For example, in a Felix Lottery of difficulty 1, a 1-digit number (from 0 to 9) will be drawn at its end to determine the winning ticket, if any. So a ticket has a one in ten chance of winning this Lottery. Here's a breakdown of the odds:

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

The lottery jackpot is a crucial factor in attracting players. Generally, the larger the jackpot, the more players want to play the lottery. Felix LottLotteryners control the jackpot size in two ways:

1. Defining what each Funder will contribute to the prize pool
2. Determining how many funders a can have

Funders have until the moment the Lottery starts to fund it. It's essential to allow enough time for funders to lock their STX and build a substantial prize pool. Ideally, before the Lottery goes live, all Lottery funders should be ready to send their fund transactions, ensuring they know what the prize pool will look like and can make more informed decisions on other attributes.

Splitting the composition of the prize pool among multiple funders is an effective way to mitigate risk. However, it also reduces the potential reward, as the Lottery splits the sales revenue among Lottery runners when claiming them back.

### The Price

{% hint style="info" %}
When we talk about the ticket price, we're only considering the amount that goes to the Lottery itself. Felix charges a 10% fee on ticket buys, and those fees go directly to a wallet address set by the platform when the contract is generated.
{% endhint %}

Setting a fair price is essential for maximizing the number of players buying tickets for your lottery and, consequently, your revenue. Players won't be motivated to participate if a ticket is too expensive relative to the chances of winning or the prize. For example, paying 1 STX for a 1 in 1,000,000 chance of winning 5 STX is unlikely to attract many players.

Conversely, if tickets are too cheap, you might end up in a situation where the chances of a winning ticket are too high, but your revenue won't compensate for the loss of what you invested in the prize pool. For instance, if a lottery has a 1% chance of winning 200 STX and sells 100 tickets for 1 STX each, a savvy player would be inclined to buy all those tickets, guaranteeing the 200 STX prize while spending 100 STX, while you'd lose half your investment.

To manage this risk effectively, Felix Lottery creators must carefully consider ticket prices and the number of tickets for sale. A good approach is to find the "probabilistic break-even" point and then adjust your Lottery parameters from there.

### The Expected Sales Return

In a Felix Lottery, you'll always get the ticket sales revenue back at the end of the Lottery. So, the expected return from sales is a straightforward calculation:

$$
TicketPrice * ExpectedSales = ExpectedSalesRevenue
$$

###

### Finding the Total Expected Return

Imagine the given Felix Lottery sold 1000 tickets:

* Difficulty: 3
* Ticket Price: 1 STX
* Locked Prize: 1000 STX

In this Lottery, after the 500th ticket sale, the chances of keeping the locked prize (no one winning the lottery) are below 50%, decreasing with every sale. To have a probabilistic estimate of your ROI, you must equate the chances of not getting your locked STX back. Let's describe it as the expected sales return minus the possibility of having a winning ticket times your locked STX.

$$
ExpectedReturn = ExpectedSalesReturn - (1 /10 ^ d) * soldTickets * Locked STX
$$

In the example above, if we use the sales return we calculated before and apply it to our formula, we would have the following:

$$
ExpectedReturn = 1000 - (1 / 10 ^ 3) * 1000 * 1000 = 0
$$

On average, this Lottery is expected not to return you anything. It is a break-even Lottery.

### Building an Edge While Staying Attractive

To create a more advantageous situation for funders, you can adjust any of the three variables: difficulty, price, or tickets on sale on the player side, or change the amount you want to lock in for the prize. Let's modify our previous example:

#### Option 1: Increasing Difficulty

* 1 Funder
* 1000 STX Funded
* Lottery Difficulty: 4 (increased from 3)
* Ticket Price: 1 STX
* Ticket Sales: 1000

Expected return:

$$
ExpectedReturn = 1000 - (1/10^4) * 1000 * 1000 = 900
$$

The expected return is, on average, 900 STX, a much better value than the previous one.

#### Option 2: Increasing Ticket Price

* 1 Funder
* 1000 STX Funded
* Lottery Difficulty: 3
* Ticket Price: 2 STX (increased from 1 STX)
* Tickets Sales: 1000

If this Lottery sells all tickets, it would give its sole Funder 2,000 STX in return. Even if you only sell 500 tickets, the Funder would recover 1,000 STX and still have a 50% chance of keeping the locked STX. A Lottery setup like this creates an attractive edge for the Funder while remaining appealing to players.&#x20;

$$
ExpectedReturn = 2000 - (1/10^3) * 1000 * 1000 = 1000
$$

### Multiple Funders

Adding more funders doesn't change the calculation, but you must use the total funded prize as lockedSTX and then split the return by the number of funders. Let's consider the following lottery:

* 1 Funders
* 150 STX locked per Funder
* Difficulty: 3
* Ticket Price: 2 STX
* Ticket Sales: 100

$$
ExpectedReturn = 200 - (1/10^3) * 100  * 300 = 170
$$

$$
ExpectedReturnPerFunder = ExpectedReturn /funders = 170/2 = 85
$$

However, the critical aspect of using multiple funders is that it can help hedge risk while maintaining the Lottery's attractiveness. For example, a 1000 STX lottery is likely more appealing to players than a 100 STX one. You could create a 1000 STX lottery by combining it with nine other funders while committing only 100 of your STX.

### Exotic Lotteries

{% hint style="info" %}
Notice each ticket must have a unique number. So, the maximum number of tickets you can sell is also limited. In a lottery with difficulty 1, you can only sell ten tickets; in difficulty 2, 100 tickets and so on.
{% endhint %}

With a good understanding of the balance between risk and attractiveness, you can create unique, attention-grabbing lotteries that remain balanced on the risk side. For example:

* 1 Funder
* 1000 STX Funded
* Lottery Difficulty: 1
* Ticket Price: 200 STX
* Tickets Sales: 10

Expected value

$$
ExpectedReturn = 2000 - (1/10^1) * 10 * 1000 = 1000
$$

This Lottery offers easy odds (guessing a single-digit number correctly), but the high ticket price limits the number of participants. If you can convince ten players to participate, perhaps some high-stakes enthusiasts, you'd achieve a 100% return on your investment.



## Summary

When running your Lottery, strive to balance the appeal to players with the level of risk you're willing to accept. Use the principles outlined in this guide to ensure you strike this balance effectively.

Ensure you have funders ready before deploying your Lottery. Collaborating with other funders is often the best way to make your Lottery attractive while reducing the probability of losing money.

If you have feedback suggestions or notice any errors, don't hesitate to contact the team at https://x.com/felixonbitcoin.

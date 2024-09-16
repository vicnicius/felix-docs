# Your First Lottery

Before running your first Felix Lottery, make sure you've went through the documentation and that you have a solid understanding of how Felix Lotteries work. Pay special attention to the [Running A Successful Lottery](/getting-started/running-a-successful-lottery) guide and if you have any questions, reach out to the team and we'll be happy to support you.

To run your first Felix Lottery, head to [/start](https://www.felixapp.xyz/start). The step-by-step wizard will guide you through the setup of a Lottery. On the first page, you'll choose the following attributes:

### A unique name for your Lottery
You must choose a unique name for the contract and its corresponding ticket NFT. When creating this name, use only characters, numbers, and hyphens.

### The Lottery Token
For now, you'll only see STX as an option.

### Maximum Number of Funders
One or more funders can fund a Lottery prize pool. The maximum number of funders determines the limit of how many funders the Lottery can have. If you want to run it yourself, set the limit to one. If you would like to invite others, increase it as much as you'd like. Remember: the more people funding, the bigger the prize pool, and the more players will be attracted to your Lottery.

### Funding Pool Contribution
The pool contribution attribute sets how much each funder will lock into the smart contract to participate as a funder in the Lottery. Each funder contributes the same amount, and at the end of the Lottery, organizers equally divide the ticket sales pool among funders.

Hit next to go to the next step. In this step, you'll set the ticket-related attributes:

### Available Tickets
This attribute sets the number of tickets available for sale in your Lottery. It directly correlates with players' chances of winning.

### Ticket Price
It tells how much a ticket will cost each player. When players buy tickets, the smart contract mints an NFT with a unique number of their choice, and the charged amount, the ticket price, is locked to the smart contract. At the end of the Lottery, the total ticket sale pool is split evenly among funders.

### Difficulty
The Lottery difficulty is the most essential attribute to consider when creating a Lottery. It will directly influence the chances of a ticket winning it. This value goes from 1 to 10. Those difficulty levels correspond to the number of digits (in order) a player needs to guess correctly. So, for a lottery with difficulty one, the player needs to guess what the drawn number will be, from 0 to 9. For difficulty two, the range is from 0 to 99; for difficulty three, 0 to 999 and so on. In other words, this means that the chance of a single ticket winning a difficulty one Lottery is 10% per ticket, while the chance of a ticket winning a difficulty ten Lottery is 0.00000001% per ticket.

### Start & End Tenure
Tenures are an essential concept in the Stacks post-Nakamoto world. They represent the number of times the Stacks miners persisted the Stacks blockchain state to the Bitcoin blockchain. In the pre-Nakamoto era, this would increase with every Stacks block. Post-Nakamoto, we'll see those two diverging. Because Felix Lotteries relies on a verifiable random function seed from Bitcoin, so it will generally be interested in the BTC chain state for Lottery lifecycle purposes.
So, in these fields, you're setting from which tenure height your Lottery can go to the active state and start selling and from which chain height it will stop selling those tickets and draw the numbers.

The final step is to review your chosen attributes and deploy your Felix Lottery. You can see what the contract will look like by clicking the preview button. Hit deploy, and you'll see the contract deployment prompt from your wallet. After you confirm the transaction on your wallet, you should see a confirmation message, and it will now be listed in the created lotteries section of your dashboard.

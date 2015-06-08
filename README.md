# BlockSizeDebate


Argument1 Pro: Increased Transaction Throughput
=========

The chief argument for the increase in blocksize is to raise the total throughput of the Bitcoin network from its current ~3 tps. This is most often attributed to an expected spike in adoption.

### Counter Argument1.1: Other Scaling Solutions

**1.1a Off-Chain Third Parties**<a name="Offchain"></a>

Of the listed solutions, this is the only one implemented today. These would significanly cut down on block size by making the minimal number of transactions, and by condensing the number of inputs/outputs used.

*1.1a.1 Security Concerns*

Opening up to third parties allows them to steal from you, and have your funds more easily hacked.<sup>[1](#footnote1)</sup> 

*1.1a.2 Privacy Concerns*

This allows for third parties to more easily collect information on you, and leak<sup>[2](#footnote2)</sup> it. Not only does this open up Bitcoin to regulatory bodies, but also hackers.

**1.1b OpenTransactions**

Content pending research...

**1.1c Lightning Networks/StrawPay**

Each of these are decentralized versions of the above, designed to reduce the amount of trust needed. Using payment channels allows it to use much less room on the blockchain, however, leading to a higher overall transaction rate.

*1.1c.1 Security Concerns*

Like with [Off-Chain Third Parties](#Offchain), there are often security concerns sited, such as the ability to steal other parties' funds from Strawpay channels.<sup>[3](#footnote3)</sup>

*1.1c.2 No Current Implementation*

Because there is no current implementation of it, there is no way it can be used if needed in the near future.

Argument2 Con: Miners/Full Nodes Cannot Handle Expansion
=========

Pools and Miners in many places have difficulty connecting to some portions of the world.<sup>[4](#footnote4)</sup> These barriers of entry would grow larger if the maximum bandwidth of the network increases. In some places it may make it so that they never catch up to the network, further pressuring the centralization of nodes.

### Counter Argument 2.1: Resource Impact not immediate

Because the change is only made to the *maximum* blocksize, it would not affect resource impact for a long time. This time gap would also give time to implement several bandwidth saving solutions that have been created/theorized specifically to reduce these problems.

### Counter Argument 2.2: Decreased node-count is not necessarily increased centralization

Because we would have to trade this off (currently) with [Off-Chain Third Parties](#Offchain), that is also an increase in centralization. So the question is more "Which increases *overall* decentralization?" instead of "Will this decrease decentralization?".

### Counter Argument 2.3: Several Large Miners Have Agreed To Adopt A Change

*2.3.1: Several have also spoken against large changes*<sup>[5](#footnote5)</sup>

### Counter Argument 2.4: Moore's Law (and it's companion laws) will support this in the future

*2.4.1: Trusting future hardware innovation is a risky move*

Especially as we move to smaller transistor gaps, where it gets harder and harder to scale.

### Counter Argument 2.5: Satoshi Predicted Node Centralization<sup>[6](#footnote6)</sup>

*2.5.1: Should we really trust the opinion of one person from 5 years ago?*

Argument3 Pro: The Limit Was Intended As A Temporary Measure
=========

### Counter Argument 3.1: The Limit Will Provide Fee Pressure

### Counter Argument 3.2: Nothing has been done to fix the original problem since<sup>[7](#footnote7)</sup>

Argument4 Con: Hardforks Are Difficult
=========

The less notice there is before a hard fork, the more likely it is to fracture the network into competing chains.

### Counter Argument 4.1: The last hardfork increasing the block size to 1 MB was performed with merely 2 months notice.<sup>[7](#footnote7)</sup>

### Counter Argument 4.2: The Hardfork Can Be Used To Make Other Useful Changes

Argument5 Pro: Increases Cost Of Block-Based DoS Attack
=========

This can be shown with the following scenario:<sup>[8](#footnote8)</sup>

Assume blocks are currently 90% full, and fees are 1 unit per kB. At the current blocksize it would take 1,200 units/hour to block 10% of transactions, and 10,000 units/hour to block *all* transactions.

Under a new blocksize (let's assume 20MB), it would take 115,200 units/hour to block 10% of transactions, and 120,000 to block all transactions.

This is a simplified model that does not take fee markets into account, but it would make transacting much more difficult whether fee markets were used or not.

### Counter Argument 5.1: Reduces the cost of a UTXO-based DoS Attack

Increasing the blocksize would allow faster bloating of the UTXO database.<sup>[9](#footnote9)</sup> Because the ability to change this scales roughly linearly to block size, increasing the blocksize increases the potential bloat rate from a bad actor. This reduces the ability to run a full node significantly, as RAM is an expensive resource to use compared to disk space.

*5.1.1 The effect of this can be dramatically reduced by storing the UTXO database on disk,<a>[10](#footnote10)</sup> and by storing it more efficiently.*

Argument6 Con: When Would A Hardfork Occur?
=========

Text of a argument goes here.

Evidence 
=========

1. [Bitcoin Network Capacity Analysis – Part 1: Macro Block Trends](https://tradeblock.com/blog/bitcoin-network-capacity-analysis-part-1-macro-block-trends)


References
=========

<a name="footnote1">1</a>: CoinDesk, [http://www.coindesk.com/coinbase-security-concerns-amid-theft-reports/](http://www.coindesk.com/coinbase-security-concerns-amid-theft-reports/)

<a name="footnote2">2</a>: CoinDesk, [http://www.coindesk.com/coinbase-denies-reports-data-breach-addresses-security-concerns/](http://www.coindesk.com/coinbase-denies-reports-data-breach-addresses-security-concerns/)

<a name="footnote3">3</a>: Mike Hearn, [https://medium.com/@octskyward/the-capacity-cliff-586d1bf7715e#3555](https://medium.com/@octskyward/the-capacity-cliff-586d1bf7715e#3555)

<a name="footnote4">4</a>: Wikipedia, [http://en.wikipedia.org/wiki/Internet_in_China#Structure](http://en.wikipedia.org/wiki/Internet_in_China#Structure)

<a name="footnote5">5</a>: Chun Wang, [http://sourceforge.net/p/bitcoin/mailman/message/34157036/](http://sourceforge.net/p/bitcoin/mailman/message/34157036/)

<a name="footnote6">6</a>: Satoshi Nakamoto, [https://bitcointalk.org/index.php?topic=532.msg6269#msg6269](https://bitcointalk.org/index.php?topic=532.msg6269#msg6269)

<a name="footnote7">7</a>: Luke-Jr, [http://www.reddit.com/r/Bitcoin/comments/38wpjn/i_know_transactions_per_second_is_a_sore_spot_but/cryzi6v?context=3](http://www.reddit.com/r/Bitcoin/comments/38wpjn/i_know_transactions_per_second_is_a_sore_spot_but/cryzi6v?context=3)

<a name="footnote8">8</a>: /u/IntroShine, [http://www.reddit.com/r/Bitcoin/comments/37790q/some_say_raising_the_blocksize_from_1mb_to_20mb/](http://www.reddit.com/r/Bitcoin/comments/37790q/some_say_raising_the_blocksize_from_1mb_to_20mb/)

<a name="footnote9">9</a>: /u/sheepiroth, [http://www.reddit.com/r/Bitcoin/comments/37790q/some_say_raising_the_blocksize_from_1mb_to_20mb/crkcu6j](http://www.reddit.com/r/Bitcoin/comments/37790q/some_say_raising_the_blocksize_from_1mb_to_20mb/crkcu6j)

<a name="footnote10">10</a>: Gavin Andresen, [http://gavinandresen.ninja/utxo-uhoh](http://gavinandresen.ninja/utxo-uhoh)

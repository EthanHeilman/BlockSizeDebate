# BlockSizeDebate


Argument 1 Pro: Increased Transaction Throughput
=========

The chief argument for the increase in blocksize is to raise the total throughput of the Bitcoin network from its current ~3 tps. This is most often attributed to an expected spike in adoption.

### Counter Argument 1.1: Other Scaling Solutions

**1.1a Off-Chain Third Parties**<a name="Offchain"> </a>

Of the listed solutions, this is the only one implemented today. These would significanly cut down on block size by making the minimal number of transactions, and by condensing the number of inputs/outputs used.

*1.1a.1 Security Concerns*

Opening up to third parties allows them to steal from you, and have your funds more easily hacked.<sup>[1](#footnote1)</sup> 

*1.1a.2 Privacy Concerns*

This allows for third parties to more easily collect information on you, and leak<sup>[2](#footnote2)</sup> it. Not only does this open up Bitcoin to regulatory bodies, but also hackers.

**1.1b Lightning Networks/StrawPay**

Each of these are decentralized versions of the above, designed to reduce the amount of trust needed. Using payment channels allows it to use much less room on the blockchain, however, leading to a higher overall transaction rate.

*1.1b.1 Security Concerns*

Like with [Off-Chain Third Parties](#Offchain), there are often security concerns sited, such as the ability to steal other parties' funds.<sup>[3](#footnote3)</sup>

*1.1b.2 No Current Implementation*

Because there is no current implementation of it, there is no way to be certain this system is a sure solution.

*1.1b.3 Needs Protocol Changes*

This is not a very widely used argument, as it's easily solvable, but it is a hurdle to overcome.

Argument 2 Con: Miners/Full Nodes Cannot Handle Expansion
=========

Pools and Miners in many places have difficulty connecting to some portions of the world.<sup>[4](#footnote4)</sup> These barriers of entry would grow larger if the maximum bandwidth of the network increases. In some places it may make it so that they never catch up to the network, further pressuring the centralization of nodes.

### Counter Argument 2.1: Resource Impact not immediate

Because the change is only made to the *maximum* blocksize, it would not affect resource impact for a long time. This time gap would also give time to implement several bandwidth saving solutions that have been created/theorized specifically to reduce these problems.

### Counter Argument 2.2: Decreased node-count is not necessarily increased centralization

Because we would have to trade this off (currently) with [Off-Chain Third Parties](#Offchain), that is also an increase in centralization. So the question is more "Which increases *overall* decentralization?" instead of "Will this decrease decentralization?".

### Counter Argument 2.3: Several Large Miners Have Agreed To Adopt A Change

*2.2.1: Several have also spoken against large changes*<sup>[5](#footnote5)</sup>

### Counter Argument 2.4: Moore's Law (and it's companion laws) will support this in the future

*2.3.1: Trusting future hardware innovation is a risky move*

Especially as we move to smaller transistor gaps, where it gets harder and harder to scale.

### Counter Argument 2.5: Satoshi Predicted Node Centralization<sup>[6](#footnote6)</sup>

*2.4.1: Should we really trust the opinion of one person from 5 years ago?*

Argument 3 Pro: The Limit Was Intended As A Temporary Measure
=========

Text of a argument goes here.

### Counter Argument 3.1: The Limit Will Provide Fee Pressure

Argument 4 Con: Hardforks Are Difficult
=========

Text of a argument goes here.

### Counter Argument 4.1: The Hardfork Can Be Used To Make Other Useful Changes

Argument 5 Pro: Increases Cost Of Block-Based DoS Attack
=========

Text of a argument goes here.

### Counter Argument 5.1: Reduces the cost of a UTXO-based DoS Attack

*5.1.1 The effect of this can be dramatically reduced by storing the UTXO database on disk, and by storing it more efficiently.*

Argument 6 Con: When Would A Hardfork Occur?
=========

Text of a argument goes here.

Evidence 
=========

1. [Bitcoin Network Capacity Analysis – Part 1: Macro Block Trends](https://tradeblock.com/blog/bitcoin-network-capacity-analysis-part-1-macro-block-trends)


Footnotes
=========

<a name="footnote1">1</a>: CoinDesk, [http://www.coindesk.com/coinbase-security-concerns-amid-theft-reports/](http://www.coindesk.com/coinbase-security-concerns-amid-theft-reports/)

<a name="footnote2">2</a>: CoinDesk, [http://www.coindesk.com/coinbase-denies-reports-data-breach-addresses-security-concerns/](http://www.coindesk.com/coinbase-denies-reports-data-breach-addresses-security-concerns/)

<a name="footnote3">3</a>: Mike Hearn, [https://medium.com/@octskyward/the-capacity-cliff-586d1bf7715e#3555](https://medium.com/@octskyward/the-capacity-cliff-586d1bf7715e#3555)

<a name="footnote4">4</a>: Wikipedia, [http://en.wikipedia.org/wiki/Internet_in_China#Structure](http://en.wikipedia.org/wiki/Internet_in_China#Structure)

<a name="footnote5">5</a>: Chun Wang, [http://sourceforge.net/p/bitcoin/mailman/message/34157036/](http://sourceforge.net/p/bitcoin/mailman/message/34157036/)

<a name="footnote6">6</a>: Satoshi Nakamoto, [https://bitcointalk.org/index.php?topic=532.msg6269#msg6269](https://bitcointalk.org/index.php?topic=532.msg6269#msg6269)

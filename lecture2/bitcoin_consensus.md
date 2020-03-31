## Consensus without identity: Block Chain
### Reasons to have identity in distributed systems 

![Reasons](./img/reasons.png)

### But why don't bitcoin nodes have identities?
1. Identity is hard in peer-to-peer networks - [Sybil attack](https://en.wikipedia.org/wiki/Sybil_attack)
2. [Pseudonymity](https://www.buybitcoinworldwide.com/anonymity/) is a goal of bitcoin. 

![Weaker Assumption](./img/weaker_assumption.png)
![Implicit Assumption](./img/implicit_consensus.png)
![Consensus Algorithm](./img/consensus_algo.png)

### To understand: Let's see how attacker can break this algorithm (Double-Spending attack)
1. From attacker's point of view

![Attacker](./img/malicious_node.png)
* Honest block - green
* Malicious block - red
* The attacker changes destination address to his own address. From our prospective we choose honest block over malicious, but from techinal view there is no difference between these two blocks. So, if this malicious block is selected, we can say that double-spending attack was successful.


2. Let's see from receiver's point of view

![Receiver view](./img/bob_view.png)
#### Here's two options:
1. Bob(receiver) hear about this transaction and he can approve it without confirmations.
2. He could wait for 1 confirmation. There could be an attempt at a double-spending attack. But if it's tree Bob can abandon this transaction. 

![Recap](./img/recap.png)
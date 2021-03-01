# Research
## Machine learning for the physical layer of wireless communications
How can two "alien" radios, in the sense that they were not designed specifically to work with each other, learn to communicate?
We propose the Echo protocol in which the two radios alternate speaking, i.e. transmitting, and echoing back what is heard in order to learn how the partner radio behaves.
We can use reinforcement learning to update the modulators even with only limited feedback across the channel.
The protocol is illustrated below.

![Echo protocol](/assets/echo/echo-overview.gif)

There are several possible variants of the Echo protocol depending on how much prior information is shared between the two learning radios.

If nothing is shared beforehand, even the message (preamble) sent across the channel is unknown and a radio can only update after a full round-trip. 
This version, Echo with Private Protocol (EPP) is illustrated below. 

![EPP](/assets/echo/EPP-protocol.gif)

If the radios are allowed to determine a preamble beforehand, the demodulators can be updated after only a half-trip (once across the channel). This allows the demodulators to converge much more rapidly to the corresponding modulators' behaviors and speeds up training.
This version, Echo with Shared Protocol (ESP) is illustrated below. 

![ESP](/assets/echo/ESP-protocol.gif)

Regardless of the amount of information sharing, the Echo protocol allows two radios to learn modulation schemes which approach the optimal QPSK constellation for an AWGN (additive white gaussian noise) channel. The major difference is how long it takes for the radios to converge to a working scheme.

![Echo results](/assets/echo/all-protocol-results.gif)

For more detail, see the [publication](https://ieeexplore.ieee.org/document/9050734) or the [code](https://github.com/ml4wireless/echo).

## Meta learning for interacting agents
I am currently exploring the impact of meta-learning (e.g. MAML) on the training process for Echo protocol agents. 
Along the way, I hope to achieve insight into how meta-learning works (or fails) when interacting with another learning agent.

# Publications
A. Sahai, **J. Sanz**, V. Subramanian, C. Tran and K. Vodrahalli, "Blind Interactive Learning of Modulation Schemes: Multi-Agent Cooperation Without Co-Design," in _IEEE Access_, vol. 8, pp. 63790-63820, 2020, doi: 10.1109/ACCESS.2020.2984218.




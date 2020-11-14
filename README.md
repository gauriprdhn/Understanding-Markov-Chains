# Understanding-Markov-Chains
Diving into the use and logic behind Markov Chains in Text Generation/ Pattern Recognition

## What are Markov Chains??
A Markov Chain is a probabilistic system that provides a way to capture the probability transitions in a system among different states.

Easier way to say this, consider a simple weather tracking system where we have 2 weather patterns only- "R" for Rainy and "S" for Sunny. We have a state space of size = 2, which we will refer to as D = {R,S}. A markob chain for this state space will be a mathematical model that will tell us the probability associated with transition from one state to the other. For a 2-state system, we will observe 4 transitions, R >> R, R >> S, S >> R, and S >> S.

Markov chains provide excellent ground for modelling real-world conditions. If independent of the actual phenomena, we would simply assign equal probabilities to each of the transitions. But we know that seldom will a Sunny (S) day be followed by a Rainy (R) only, Sunny weather or any weather pattern tends to prevail for a period before it transitions to the next (lest there be a natural disaster).

We can minic this "stickyness" with a two-state Markov chain. When the Markov chain is in state "R", it has a 0.9 probability of staying put and a 0.1 chance of leaving for the "S" state. Likewise, "S" state has 0.9 probability of staying put and a 0.1 chance of transitioning to the "R" state.
We will study the Markov Chains in context of an NLP problem where we often need to construct text sequences which involve predicting the next word given the current word in the sequence. For simplicity all the transitions will be treated as having equal probability of occurance for a given state. For example, if A is a state that can be followed by B,C,D, or E then each transition, A >> B, A >> C, A >> D or A >> E will have equal chance of occuring.

A great source to learn in detail would be https://setosa.io/ev/markov-chains/. The blog will explain visually how Markov Chains could be helpful in understanding real-world events.

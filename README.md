# Optimization-Markov-Decision-Process
Optimizing Service Delivery Action for Lenovo using Markov Decision Process

Background: For a technology company like Lenovo, early and efficient issue resolution plays a key role in reducing costs and driving customer satisfaction. On several occasions, the immediate service action chosen does not lead to an issue resolution resulting in increased costs and loss of customer goodwill

Objective: 

Devise a decision support system to help Lenovo identify the optimal service action to resolve a customer issue.

Solution: 

A solution to the problem was achieved in three steps

Step 1: Using historical data, developed a stochastic model(Markov Chain) to understand the following
a. Likelihood of each service action resolving an issue.
b. Common paths that customer issues take in terms of service actions.

Step 2: Incorporated the learnings from the Markov Chain to build a Markov Decision Process which helped identify optimal rules for service action selection.

The five components of the Markov Decision Process (State space, Action space, Epoch, Transition probabilities and Cost matrix) were defined carefully to capture the relevant information about an issue. After the costs and probabilities for each transition were accounted for, the optimal decision policy was generated using linear programming(LINDO). The linear program accounted for all potential transitions, in terms of costs and their likelihoods, and then decided which service action was the most optimal choice in terms of cost. 

Step 3: Sensitivity Analysis - A range of sensitivity analysis was conducted to ensure the robustness of the optimal policy.

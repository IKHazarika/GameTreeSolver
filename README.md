# GameTreeSolver
A tool to solve extended form games in Python

Developed in Python by IKHazarika

This program can find the pure Subgame Perfect Equilibrium for several categories of games.

The games can be described by entering the nodes in the list titled 'nodes', in the order that if the index of node 'a' is less than the index of node 'b', then the distance from the initial node to 'a' is less than or equal to the distance between the initial node and node 'b'.

Each node is of the form [parent node, player or payoff, label, probability (optional)]. For the parent node of the initial node, enter any negative integer as a place holder, otherwise enter the parent. Enter the player number after that. If the node is terminal and there is no associated player, enter the vector of payoffs as a list, such as [1, -10, 30]. If the player is nature, enter 'N'. Then add the label of the node, the "name" of the associated action (such as "cooperate" or "defect"). Finally, if the parent node's player is 'N', enter the probability associated with this node. The sum of the probabilities of all the children nodes of a node with player 'N' must be 1.

Currently, it works with finite perfect information games of arbitrary length and arbitrary number of players. If there are multiple SPNEs, the one including actions listed the lefmost are reported.
 
Newer versions would soon include:

1. Listing of all pure strategy SPNEs
2. Games with imperfect information
3. An HTML-CSS-JavaScript based graphical user interface to make entering the game details easy and the output easy to read

For more details, send a mail to kpishanh@gmail.com

Visit https://sites.google.com/view/ishankhazarika

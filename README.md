# PHSX815_Project3_Help

Thanks for the help!

This is the same setup from project 1 and 2. It's a simulated card game. Below is the description used for that game:

**************

We simulate a card game and analyze the results with a density plot and log-likelihood ratio.

The game works like this: Two players a distributed cards randomly from a deck of N_cards. The players "play" them against each other in the order they were distributed. The player with the higher valued card wins the round. Continue until all of the cards have been played. N_cards/2 rounds. This would constitute one game. You can select a number of games to play in a set and a number of sets to play.

You can cheat for your alternative hypothesis. This is done by giving yourself artificially high valued cards that will always win against the other players cards. This is called "gimme"

Begin with CardgameSim.py

-h gives options for user input. You can input numbers of cards, games, and sets. You can also set the gimme value for an alternative hypothesis. You should input the name of a file to save it as. Two sample distributions have been shared, named "fair.txt" and "cheat.txt"

When you run this, you'll generate another text file as rules_userinput. This is used by the analysis program to read data you inserted into the simulation.

Next, you'll analyze the data with CardgameAnalysis.py

-h gives options for user input. You can input the null and alternative hypotheses as input0 and input1. I've also added a method for setting confidence level with -conf, but this has not been tested extensively.

You'll generate plots of density and LLR with this.

Best starting place:

-Ncards 16 -Ngames 15 -Nsets 500 -gimme 2 -output cheat.txt

-Ncards 16 -Ngames 15 -Nsets 500 -output fair.txt

*****************

What I would like help with is determining how to setup a function to determine how many cheater cards were used (which is the whole point of this project). As the gimme value is increased, the distribution moves to the right. Unfortunately, I don't believe the probability distribution is very straightfoward. I build my log-likelihood from experimental values of probability, not theoretical.

I've added two images which are samples from 5 games and 25 games per set.

Feel free to contact me with questions. I'll be happy to discuss. rjscott@ku.edu

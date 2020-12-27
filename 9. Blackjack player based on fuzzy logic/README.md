# Blackjack player based on fuzzy logic

This project is meant to make use of the fuzzy logic in order to make a driver for Blackjack player. It was designed with a specific objective in mind - to make it easy to manipulate with the parameters, in order to make it learn the right rules and parameters.

Due to high complexity of the task, the rather easy way was finally chosen:
* generate a large number of random tuples of rules and parameters in the optimized Monte Carlo process - the possible tuples are repeatedly shorlisted, so that the computing power is not wasted on the ones that do poorly.

Then the following two possibilities are considered:
* the basic drivers being ensembled into complex one, i.e. the predictions of the top shortlisted drivers (say 10) are weighted by their scores, to make a single prediction with hopefully lower variability (although most likely biased),
* the basic drivers being feed into an evolutionary algorithm to make a single more accurate one.

Mind that, although you can mix the above approaches, it might not be a good idea, since the evolutionary algorithm heavily declines the independence of the shortlisted drivers, which is needed for ensembling.
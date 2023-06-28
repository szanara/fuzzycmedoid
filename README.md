# fuzzycmedoid
this repository corresponds to a reproduction of the code of the paper https://www.sciencedirect.com/science/article/abs/pii/S0925231215003720 for a course work using the Avila Dataset (https://archive.ics.uci.edu/ ml/datasets/Avila)


Using the Avila dataset, I produced 3 disililarity matrices using the Euclidean distance (L2), the city-block distance (L1) and the distance from Chebyshev (Linf).
I implemented and ran the "VFCMddV" algorithm from Francisco de A.T. de Carvalho, Filipe M de Melo, Yves Lechevallier, A multi-view relational fuzzy c-medoid vectors clustering algorithm.
Neurocomputing, v. 163, p. 115-123, 2015".(https://www.sciencedirect.com/science/article/abs/pii/S0925231215003720) 50 times to get a fuzzy partition in 12
groups and selected the best result according to the objective function.
Then I calculated the Modified partition coefficient and the Partition entropy. This generated a crisp partition into 12 groups and then it was possible to calculate the corrected Rand index, and the F-measure
(adapted for grouping).

The dissimilarity matrices were normalized as described in the article describing the VFCMddV algorithm (page 119, column 1, third paragraph) and the parameters: k = 12; T = 150; = 10−10;

These steps and parameters followed were based on the request of the professor of the discipline, Co-author of the article, Prof. doctor Francis.

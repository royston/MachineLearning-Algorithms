Notes:
Problem we are trying to solve with this recommender system for recommending movies for each user based on their ratings for other movies and how much they say they like different types of movies(action / romance etc)
A) What we know- 
1) How each user rates a bunch of movies they may have watched (Y)
2) How much each user rates different types of movies (action / comedy / romance etc) (Theta)

B) What we evaluate:
1) A crowd sourced rating of how much of each movie type each movie has - How romantic / comedic / action packed a given movie is. (X)
2) How much a user is expected to rate a movie he / she hasn't watched / rated.
3) Recommend movies to a user based on 2) that a user is likely to enjoy.

Algorithm:
Crude algo :
	1) Given Theta(for each user, what their liking for each movie type is), learn X for every movie
	2) Given X, learn Theta

	Inititialize X and Theta
	Iteratively, 
		using X), find Theta),
		using Theta) find X)
		
Collaborative algo:
DO the crude algo above simultaneously:
Initialize X, Theta
Using gradient descent(Or an advanced optimization algo): arrive at an optimal value of X, Theta

Finally, find B)2) and B)3) based on the above algo:
Theta * X

Nu - number of users, indexed by j
Nm - number of movies, indexed by i



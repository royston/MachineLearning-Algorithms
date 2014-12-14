##Stochasitic Gradient Descent
For Linear example, computing the derivative term can be expensive if the number of training exmaples is huge(because for every "step", sum has to be calculated over all training examples - also called Batch Gradient Descent)

In stochastic gradient descent, we instead use 1 example in each iteration. Scales much better. 
Look up wikipedia for the exact algo. Too much notation to put into a .md file.

Another way to overcome the issues with traditional Batch gradient descent is to use b examples( b < m) in each iteration. Reduce the number of training examples in each iteration.


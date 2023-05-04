Download Link: https://assignmentchef.com/product/solved-cs546-assignment-1-k-means-and-gmm
<br>
Implement the standard version of the K-Means algorithm as described in lecture. The initial starting points for the K cluster means can be K randomly selected data points. You should have an option to run the algorithm <em>r</em> times from <em>r</em> different randomly chosen initializations (e.g., <em>r</em> = 10), where you then select the solution that gives the lowest sum of squares error over the <em>r </em>runs. Run the algorithm for several different values of K and report the sum of squares error for each of these models. Please include a 2-d plot of several different iterations of your algorithm with the data points and clusters.

<h1>Assignment #2: GMM</h1>

Use the following general outline to execute the EM algorithm for GMM (please refer to lecture slides as needed for details of the EM algorithm for GMMs)

<ul>

 <li>Initialize the parameters randomly</li>

</ul>

Execute E and M steps as long as the convergence condition is not satisfied:

<ul>

 <li>E-step: compute membership probabilities using the current θ current values.</li>

 <li>M-step: compute new parameters θ<sub>new</sub> using the membership probabilities from the E-step</li>

 <li>After each EM iteration compute the log-likelihood of the data using θ<sub>new</sub> (see lecture notes). This will allow you to print out the log-likelihood values from each EM iteration, as the algorithm is running, to monitor its convergence.</li>

 <li>Check for convergence by computing the value of the log-likelihood after each iteration and halting when it appears not to be changing in a significant manner from one iteration to the next. If the convergence criterion is not satisfied, then execute another EM iteration.</li>

</ul>

You should run your algorithm multiple times from <em>r </em>different randomly-chosen starting conditions (e.g. r = 10) and pick the solution that results in the highest log-likelihood (since EM in general only finds local maxima).

<strong>*Note that The EM algorithm for Gaussian mixtures is a non-trivial algorithm to get working properly: please try and debug it carefully</strong>. Check that the likelihood is nondecreasing at each step (if the log-likelihood ever decreases you have a bug in your code).

Please print out your final parameters for the Gaussians in your GMM and check that the estimated parameters are roughly equal to the true parameters (obtained using the labels). For these data sets you could also impose a maximum number of iterations to halt the algorithm (e.g., 500) if it gets that far and still has not converged. Report your results for each and include a 2-d plot.

<strong>Report: </strong>Your report should include a short description of your experiments, along with the plots and discussion paragraphs requested above and any other relevant information to help shed light on your approach and results.  <strong> </strong>

<strong>Here is what you need to turn in: </strong>

<ul>

 <li>Your report.</li>

 <li>Readable code</li>

</ul>



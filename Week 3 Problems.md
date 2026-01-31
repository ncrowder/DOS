---


---

<h1 id="dos-problem-set-4-monte-carlo">DOS Problem Set 4 (Monte Carlo)</h1>
<ol>
<li>
<p>Simulate rolling an 8-sided die five times and store the values in a list called sample.  Find the mean, using <em>np.mean()</em> and standard deviation, using <em>np.std()</em>.  Make sure you use the appropriate ddof value.</p>
</li>
<li>
<p>Suppose that Tom plays a game that has him roll an 8-sided die five times on each turn.  Write a loop to calculate the simulated mean from 10000 turns.  Plot a histogram.</p>
</li>
<li>
<p>Find the 95% confidence interval 2 ways by using np.quantile with the appropriate cut-off percentages on the sampling distribution.</p>
</li>
<li>
<p>Calculate the theoretical confidence interval by applying the CLT and using the values from your initial sample in #1.  Note we need to use 2.776 in the formula instead of 2 or 1.96 since because the sample size (n = 5) is so small the distribution is more spread out.</p>
</li>
</ol>
<p><span class="katex--display"><span class="katex-display"><span class="katex"><span class="katex-mathml"><math xmlns="http://www.w3.org/1998/Math/MathML" display="block"><semantics><mrow><mtext>(lower,&nbsp;upper)</mtext><mo>=</mo><mover accent="true"><mi>x</mi><mo>ˉ</mo></mover><mo>±</mo><mn>2.776</mn><mo>∗</mo><mfrac><mi>s</mi><msqrt><mi>n</mi></msqrt></mfrac></mrow><annotation encoding="application/x-tex"> \text{(lower, upper)} = \bar{x} \pm 2.776 * \frac{s}{\sqrt{n}} </annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="base"><span class="strut" style="height: 1em; vertical-align: -0.25em;"></span><span class="mord text"><span class="mord">(lower,&nbsp;upper)</span></span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">=</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 0.66666em; vertical-align: -0.08333em;"></span><span class="mord accent"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height: 0.56778em;"><span class="" style="top: -3em;"><span class="pstrut" style="height: 3em;"></span><span class="mord mathnormal">x</span></span><span class="" style="top: -3em;"><span class="pstrut" style="height: 3em;"></span><span class="accent-body" style="left: -0.22222em;"><span class="mord">ˉ</span></span></span></span></span></span></span><span class="mspace" style="margin-right: 0.222222em;"></span><span class="mbin">±</span><span class="mspace" style="margin-right: 0.222222em;"></span></span><span class="base"><span class="strut" style="height: 0.64444em; vertical-align: 0em;"></span><span class="mord">2.776</span><span class="mspace" style="margin-right: 0.222222em;"></span><span class="mbin">∗</span><span class="mspace" style="margin-right: 0.222222em;"></span></span><span class="base"><span class="strut" style="height: 2.03756em; vertical-align: -0.93em;"></span><span class="mord"><span class="mopen nulldelimiter"></span><span class="mfrac"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 1.10756em;"><span class="" style="top: -2.30972em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mord sqrt"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 0.80028em;"><span class="svg-align" style="top: -3em;"><span class="pstrut" style="height: 3em;"></span><span class="mord" style="padding-left: 0.833em;"><span class="mord mathnormal">n</span></span></span><span class="" style="top: -2.76028em;"><span class="pstrut" style="height: 3em;"></span><span class="hide-tail" style="min-width: 0.853em; height: 1.08em;"><svg width="400em" height="1.08em" viewBox="0 0 400000 1080" preserveAspectRatio="xMinYMin slice"><path d="M95,702
c-2.7,0,-7.17,-2.7,-13.5,-8c-5.8,-5.3,-9.5,-10,-9.5,-14
c0,-2,0.3,-3.3,1,-4c1.3,-2.7,23.83,-20.7,67.5,-54
c44.2,-33.3,65.8,-50.3,66.5,-51c1.3,-1.3,3,-2,5,-2c4.7,0,8.7,3.3,12,10
s173,378,173,378c0.7,0,35.3,-71,104,-213c68.7,-142,137.5,-285,206.5,-429
c69,-144,104.5,-217.7,106.5,-221
l0 -0
c5.3,-9.3,12,-14,20,-14
H400000v40H845.2724
s-225.272,467,-225.272,467s-235,486,-235,486c-2.7,4.7,-9,7,-19,7
c-6,0,-10,-1,-12,-3s-194,-422,-194,-422s-65,47,-65,47z
M834 80h400000v40h-400000z"></path></svg></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 0.23972em;"><span class=""></span></span></span></span></span></span></span><span class="" style="top: -3.23em;"><span class="pstrut" style="height: 3em;"></span><span class="frac-line" style="border-bottom-width: 0.04em;"></span></span><span class="" style="top: -3.677em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mord mathnormal">s</span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 0.93em;"><span class=""></span></span></span></span></span><span class="mclose nulldelimiter"></span></span></span></span></span></span></span></p>
<ol start="5">
<li>
<p>Suppose that if Tom’s average on a turn is over over 5.5 he wins a bonus turn.  Use np.quantile to calculate the probability that on any turn he will get a bonus.</p>
</li>
<li>
<p>As discussed above, due to the small sample size the distribution is more spread out, and we need to use the t-distribution instead of the normal distribution.  This is generally always the case, but when the sample size is large enough we can use the normal instead.  Recalculate the probability Tom rolls an average over 5.5 using the theoretical t-distribution with either stats.t.cdf or stats.t.sf.  The arguments for both functions are the same (xbar, df, loc, scale).  xbar is the average you want to use in your calculation (i.e., 5.5), and df is the number of degrees of freedom.  In this case, we will use df=4, since the degrees of freedom for the t-dist is n-1.  For loc and scale, we will again use the mean and sd from our initial sample calculated at the top.</p>
</li>
<li>
<p>Using the csv of a random sample of 10 adult heights and 10 jockey heights, simulate 500 sample difference in means using either the permutation method shown in the slides or bootstrapping under the assumption that there is no difference in the two populations’ heights (adults vs. jockeys).  Store the sample differences in a list called sim_diffs.  You should use pd.read_csv and not manually copy the heights into your notebook.</p>
</li>
<li>
<p>Plot a histogram of the simulated differences as well as vertical lines for the 95% CI.  Plot another vertical line showing the sample mean.  Explain your conclusion (is it justifiable to assume that the heights or the same or no?) based on whether the sample mean is inside or outside the CI.</p>
</li>
<li>
<p>Suppose we have three bags with 2 die, 3 die, and 2 die as shown.<br>
bag1 = [ [1,2,3,4,4,-4], [1,-2,3,4,5,-6] ]<br>
bag2 = [ [1,2,3,4,5,5], [1,-2,3,4,5,6], [1,1,1,-5,5,6] ]<br>
bag3 =  [ [1,2,3,-3,4,-4], [1,2,3,4,5,-6] ]<br>
Greg picks one die from each bag randomly and rolls.  If the sum off three die is negative he wins a gajillion dollars.  Using 5000 samples, calculate using np.quantile the chance that Great wins a gajillion dollars.</p>
</li>
<li>
<p>Suppose that a busy intersection sees on average 3 accidents a month and accidents occur independently.  Using a sample size of 10 years, what’s the probability that a month will go by that has either no accidents or more than 4 accidents.  Use the appropriate <em>rvs</em> function.</p>
</li>
<li>
<p>Using the diabetes dataset, choose the two predictors with the largest correlation to y.  Fit a linear regression model to y using these two predictors and save it to the variable model_dia.</p>
</li>
<li>
<p>Calculate the mean of the two predictors as well as the covariance.  Save these in mean_dia and cov_dia.</p>
</li>
<li>
<p>Since we already know all predictors are roughly normal in our sample, we will use the multivariate normal to simulate 5000 new patients.  Save the results into a dataframe called df_sim.  Use slide 79 if you need help.</p>
</li>
<li>
<p>Using the model you built in problem 11, calculate the predicted y-value from the simulated patients and add it as a column to your dataframe.  Show a histogram of the predicted y-values.</p>
</li>
<li>
<p>Suppose we would like to know the expected difference in outcomes from those in the bottom 20% for both predictors vs. those in the top 20% for both predictors.  Simulate 500 samples of size 500 and calculate the mean difference in outcomes and the range of mean difference in outcomes would fall between <strong>98%</strong> of the time (assuming all our modeling assumptions were valid and the initial sample of patients (the real one) was representative and unbiased).</p>
</li>
<li>
<p>Pick either the exponential, laplace, or triangular distribution with the default parameters and ADD a little noise using a normal distibution with loc (mean) = 0 and scale (sd) = .1.  Generate 1000 samples from this distribution.  Calculate the negative log-likelihood (nnlf) for the exponential, laplace, triangular, and normal distributions after fitting each of these to the simulated data and identify the best fitting distribution.</p>
</li>
<li>
<p>Slowly “turn up the noise” by increasing the standard deviation of the normal distribution component until the best fitting distribution of the combination is normal.  Try writing a loop that slowly increments the standard deviation by .01 each time you fit and test for the nnlf and stop the loop when the distribution with the lowest nnlf is normal.  Print out the minimal standard deviation.  <em>Note: if you aren’t able to solve this completely, manually increment  the scale by .05 until you get the same result.</em></p>
</li>
</ol>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>


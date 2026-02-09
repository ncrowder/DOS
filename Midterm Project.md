---


---

<h1 id="dos-midterm-project">DOS Midterm Project</h1>
<ol>
<li>
<p>If the average bank transaction time takes 5 minutes on average to finish and times are independent from one another, what is the probability a person getting service has their transaction completed:</p>
<p>a) within the next 7 minutes</p>
<p>b) not for at least 4 minutes</p>
<p>c) in the next 6 minutes, if they’ve already had their transaction worked on for 4 minutes? (Hint: the key distribution you are using is “memoryless” - what does that mean?)</p>
</li>
<li>
<p>Earthquakes happen very seldom, but occurrences are assumed to be independent and a particular country experiences 1.3 earthquakes on average every decade.  What is the probability that a more than 12 earthquakes happen in the next 100 years?  No earthquakes in the next decade?</p>
</li>
<li>
<p>Simulate 100 samples from a binomial distribution with p = .25 and n = 100 called samp100 and 100 samples with p = .25 and n = 1000 called samp1000 using st.binom.rvs().</p>
<p>a) What’s the mean and standard deviation of samp100 and samp1000?</p>
<p>b) What’s the percentage error in the samp100 and samp1000 sample mean and standard deviation from the <a href="https://statisticsbyjim.com/probability/binomial-distribution-formula">true mean and standard deviation</a>?</p>
<p>c) Calculate the 95% CI based off the the sample mean and standard deviation from samp100:  (upper, lower) = <span class="katex--inline"><span class="katex"><span class="katex-mathml"><math xmlns="http://www.w3.org/1998/Math/MathML"><semantics><mrow><mover accent="true"><mi>x</mi><mo>ˉ</mo></mover><mo>±</mo><mn>1.96</mn><mo stretchy="false">(</mo><mfrac><mi>s</mi><msqrt><mi>n</mi></msqrt></mfrac><mo stretchy="false">)</mo></mrow><annotation encoding="application/x-tex">\bar{x} \pm 1.96(\frac{s}{\sqrt{n}})</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="base"><span class="strut" style="height: 0.66666em; vertical-align: -0.08333em;"></span><span class="mord accent"><span class="vlist-t"><span class="vlist-r"><span class="vlist" style="height: 0.56778em;"><span class="" style="top: -3em;"><span class="pstrut" style="height: 3em;"></span><span class="mord mathnormal">x</span></span><span class="" style="top: -3em;"><span class="pstrut" style="height: 3em;"></span><span class="accent-body" style="left: -0.22222em;"><span class="mord">ˉ</span></span></span></span></span></span></span><span class="mspace" style="margin-right: 0.222222em;"></span><span class="mbin">±</span><span class="mspace" style="margin-right: 0.222222em;"></span></span><span class="base"><span class="strut" style="height: 1.288em; vertical-align: -0.538em;"></span><span class="mord">1.96</span><span class="mopen">(</span><span class="mord"><span class="mopen nulldelimiter"></span><span class="mfrac"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 0.695392em;"><span class="" style="top: -2.62587em;"><span class="pstrut" style="height: 3em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord sqrt mtight"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 0.805905em;"><span class="svg-align" style="top: -3em;"><span class="pstrut" style="height: 3em;"></span><span class="mord mtight" style="padding-left: 0.833em;"><span class="mord mathnormal mtight">n</span></span></span><span class="" style="top: -2.76591em;"><span class="pstrut" style="height: 3em;"></span><span class="hide-tail mtight" style="min-width: 0.853em; height: 1.08em;"><svg width="400em" height="1.08em" viewBox="0 0 400000 1080" preserveAspectRatio="xMinYMin slice"><path d="M95,702
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
M834 80h400000v40h-400000z"></path></svg></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 0.234095em;"><span class=""></span></span></span></span></span></span></span></span><span class="" style="top: -3.23em;"><span class="pstrut" style="height: 3em;"></span><span class="frac-line" style="border-bottom-width: 0.04em;"></span></span><span class="" style="top: -3.394em;"><span class="pstrut" style="height: 3em;"></span><span class="sizing reset-size6 size3 mtight"><span class="mord mtight"><span class="mord mathnormal mtight">s</span></span></span></span></span><span class="vlist-s">​</span></span><span class="vlist-r"><span class="vlist" style="height: 0.538em;"><span class=""></span></span></span></span></span><span class="mclose nulldelimiter"></span></span><span class="mclose">)</span></span></span></span></span></p>
<p>d) Using the formulas for mean and standard deviation from a binomial, calculate the upper and lower bounds again.</p>
<p>e) Calculate what proportion of the samples within samp100 and samp1000 fall within the confidence interval constructed in part d.</p>
</li>
</ol>
<ol start="4">
<li>
<p>Suppose we have a starting inventory of 500 in the warehouse.  The units received each week is random: 10% of the time we get sent 50, but the other 90% of the time only 40 get sent.  The weekly demand (number sold) is approximately normally distributed with 50 as the average units sold and a standard deviation of 5 units.  Round the demand to the nearest unit.  Demand and units received are independent and uncorrelated.</p>
<p>To simulate the units received the following works:<br>
<em>demand = np.random.choice([40,50], size = num_weeks, p=[.9,.1])</em></p>
<p>Simulate the inventory after 52 weeks 100 times.  What appears to be the probability we will:</p>
<p>a) Run out of inventory anytime in the next year (52 weeks)?<br>
b) Our inventory will be at least 100 at the end of the year?<br>
c) Create a histogram with bin width of 10 for the inventory at the 2 month mark (8 weeks).<br>
e) What is the lowest 10% case for stock at 2 months?<br>
f) What is the median amount at 2 months?<br>
g) How much starting stock do I need so that I run out no more than 5% of the time?  (THIS IS A BONUS QUESTION.)</p>
</li>
<li>
<p>Test to see if the <a href="https://www.lock5stat.com/datasets4e/BMI.csv">sample data</a> suggests it is reasonable to assume that there is no difference in BMI between the group that exercised in the last 30 days vs. those that did not.  Use the permutation method as suggested in #7 of Problem Set 3.  Do this by generating 500 simulated differences, plotting a histogram, calculating the 95% CI, and seeing if the sample mean is outside of these bounds.</p>
</li>
<li>
<p>This exercise uses the <a href="https://www.lock5stat.com/datasets4e/BodyFat.txt">sample data</a> here.  We will consider bodyfat to be the response variable.<br>
a) Find the mean, median, max, min for all the variables using the df.agg method.<br>
b) Use seaborn to create a pairplot for the data as well as a correlation matrix.  Note any strong correlations between variables.  What variable(s) seem to be most correlated with bodyfat?  Which seems to be the least?<br>
c) Describe the histograms of each variable in terms of symmetry and/or skew.<br>
d) Test each of the variables to see if the best fitting distribution is the exponential, normal, triangular, or laplace using the nnlf after fitting each distribution first.</p>
</li>
</ol>
<p>Code snippet (indent where needed):</p>
<pre><code>from scipy import stats as st

dists = [st.expon, st.norm, st.laplace, st.triang]
winners = {}

for col in x.columns: 
#x is a dataframe with the bodyfat column dropped

nlls = []
	for dist in dists:
		params = dist.fit(x[col].values)
		nll = dist.nnlf(params, x[col])
		nlls.append(nll)
	lowestindex = np.argmin(nlls)
	winners[col] = dists[lowestindex].name
winners
</code></pre>
<p>e) Identify the two predictors for which the normal distribution is the best.<br>
f) Fit a linear regression model to the data (use bodyfat as your response and the two variables that are normally distributed as your predictors).<br>
g) Calculate the means and covariance matrix for the predictors.<br>
h) Simulate 5000 additional patients using st.multivariate_normal() and store it in x_sim.<br>
i) What the expected bodyfat for someone in the upper 25% for each of the predictors using the results from x_sim?<br>
j) What is the expected bodyfat for someone in the bottom 33% for one predictor and upper 33% for the other using x_sim?</p>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>


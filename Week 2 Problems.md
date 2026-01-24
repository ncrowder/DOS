---


---

<h1 id="dos-problem-set-3">DOS Problem Set 3</h1>
<p>You should complete the “Sampling in Python DataCamp” and watch the class recording from 1/22 before attempting these problems.  Note that the slide deck is also available in BB.  In addition, all problem sets from that course can be <a href="https://github.com/ncrowder/datacamp/tree/main/sampling_in_python">found here</a>.</p>
<blockquote>
<p>These datasets are in ‘feather’ format so you’ll need to import pyarrow in order to work with them.  You can use <em>read_feather</em> to load the datasets into a dataframe.</p>
</blockquote>
<pre><code>df_spot = pd.read_feather('https://raw.githubusercontent.com/ncrowder/datacamp/main/sampling_in_python/spotify_2000_2020.feather')
</code></pre>
<ol>
<li>
<p>Generate a samp20 dataframe from a random sample of 20 rows.</p>
</li>
<li>
<p>Generate a samp2per dataframe from a random sample of 2% of the rows.</p>
</li>
<li>
<p>Generate a random sample of 1% of the ‘duration_ms’ column and compute the mean of the sample and the mean of the full dataset.  What is the difference in milliseconds and as a percentage error?</p>
</li>
<li>
<p>Sort the dataframe by ‘duration_ms’ using the <em>sort_values</em> method and then find the mean ‘energy’ of the top 50 rows.  Compare this with the mean ‘energy’ of the full dataset.  What is the difference?</p>
</li>
<li>
<p>Generate a histogram of the ‘energy’ from the top 50 rows after sorting as well as histogram of the full dataset’s ‘energy’ level.  Comment on any perceived differences.</p>
</li>
<li>
<p>Using the original dataset, find the standard deviation of the ‘tempo’ of every 4th row.</p>
</li>
<li>
<p>What proportion of the dataset do the top 5 artists in the dataset represent?  Use the <em>value_counts</em> method with the normalize argument.  Then find the proportion of each of the top 5 artists if only looking at the rows representing one of these artists.  <strong>Hint: The proportions should add to 1 in the latter case, but not the former case.</strong></p>
</li>
<li>
<p>Generate a random sample of 5% of the artists from the dataset 2 ways: one that allows for repeated artists to show up and a second way where it is only possible that an artist shows up once in the sample.  For the first way you can simply use the sample method off of the dataframe.  For the second way you can use use the sample method off of the random package and pass a list of unique artists.</p>
</li>
<li>
<p>Using a dataset that only includes artists that show up at least 10 times, apply the <em>groupby</em> method on the ‘artists’ to take a sample of 10% of the rows from each artist.  Use a random_state of 2026.<br>
Helper code to start (make sure you understand it):</p>
</li>
</ol>
<pre><code>counts = df_spot.value_counts('artists')

top_artists = counts[counts&gt;=10].index
</code></pre>
<ol start="10">
<li>
<p>Using the result from #9, find the mean, min and max of the ‘loudness’ both for the total dataset, and then grouped by artist.</p>
</li>
<li>
<p>Generate a plot of sample_size vs. relative_error in the mean of ‘duration_ms’ for sample sizes ranging from 10 to 500.  The relative_error is computed against the the true mean from the entire population.</p>
</li>
<li>
<p>Plot a sampling distribution of the mean of ‘duration_ms’ using 5000 samples of size 25 and of size 100.</p>
</li>
<li>
<p>Find the margin of error corresponding to a 95% CI for both sampling distributions in #12 (n=25 and n=100) using np.quantile.</p>
</li>
<li>
<p>Generate a histogram of the ‘loudness’ for the entire dataset.  Does it appear normally distributed?  Explain the shape in terms of symmetry and skewness.</p>
</li>
<li>
<p>Select a single sample of size 100 and estimate the standard error of the mean ‘loudness’ using the formula:</p>
</li>
</ol>
<p><span class="katex--display"><span class="katex-display"><span class="katex"><span class="katex-mathml"><math xmlns="http://www.w3.org/1998/Math/MathML" display="block"><semantics><mrow><mtext>SE</mtext><mo>≈</mo><mfrac><mi>s</mi><msqrt><mi>n</mi></msqrt></mfrac></mrow><annotation encoding="application/x-tex">
\text{SE} \approx \frac{s}{\sqrt{n}}
</annotation></semantics></math></span><span class="katex-html" aria-hidden="true"><span class="base"><span class="strut" style="height: 0.68333em; vertical-align: 0em;"></span><span class="mord text"><span class="mord">SE</span></span><span class="mspace" style="margin-right: 0.277778em;"></span><span class="mrel">≈</span><span class="mspace" style="margin-right: 0.277778em;"></span></span><span class="base"><span class="strut" style="height: 2.03756em; vertical-align: -0.93em;"></span><span class="mord"><span class="mopen nulldelimiter"></span><span class="mfrac"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 1.10756em;"><span class="" style="top: -2.30972em;"><span class="pstrut" style="height: 3em;"></span><span class="mord"><span class="mord sqrt"><span class="vlist-t vlist-t2"><span class="vlist-r"><span class="vlist" style="height: 0.80028em;"><span class="svg-align" style="top: -3em;"><span class="pstrut" style="height: 3em;"></span><span class="mord" style="padding-left: 0.833em;"><span class="mord mathnormal">n</span></span></span><span class="" style="top: -2.76028em;"><span class="pstrut" style="height: 3em;"></span><span class="hide-tail" style="min-width: 0.853em; height: 1.08em;"><svg width="400em" height="1.08em" viewBox="0 0 400000 1080" preserveAspectRatio="xMinYMin slice"><path d="M95,702
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
<ol start="16">
<li>
<p>Generate 5000 bootstrap samples using your sample from #14 and compute the mean for each one.  The bootstrap standard error is the sample standard deviation of the 5000 bootstrap statistics.  Since the mean of this distribution is estimated from the data, use <strong>ddof = 1</strong>.</p>
</li>
<li>
<p>Calculate the difference between the theoretical SE from #14 (a result of the CLT) and the bootstrap SE from #15.  <strong>Hint: They should be very close.</strong></p>
</li>
<li>
<p>Instead of using the mean, let’s use the median or maximum (your choice) instead.  Reproduce parts 14-16, bearing in mind that the difference should be much more dramatic, at least in terms of percent difference.</p>
</li>
<li>
<p>The reason the results are different is because the CLT  formula for estimating SE can only be applied to means.  Generate a histogram of the bootstrap from the median/max statistic (whichever you chose in #17).  Does the result appear normal?  Explain how this factors in to the difference observed when comparing the means SE vs the median/max SE.</p>
</li>
<li>
<p>Suppose we roll an 8-sided die that has the following sides = [1,2,2,3,3,4,7,9] five times and take the average of the rolls.  Simulate doing this 10000 times and plot a sampling distribution that corresponds to this result.</p>
</li>
<li>
<p>Suppose now we roll the above 8-sided die along with a normal 6 sided fair die and take the average.  Simulate doing this 10000 times and plot a sampling distribution that corresponds to this result.</p>
</li>
<li>
<p>Generate one single sample from #21 and find the margin of error (MOE) corresponding to a 95% confidence interval using the ppf function (thus using the fact that the sampling distribution will be normally distributed under the CLT) with loc equal to the mean of your single sample and standard error using the above formula for SE.  A similar approach, but one using the bootstrap is shown on one of the final slides in the slide deck if you get stuck.</p>
</li>
</ol>
<blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>


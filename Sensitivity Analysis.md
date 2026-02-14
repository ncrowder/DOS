---


---

<h1 id="reduced-cost--shadow-prices">Reduced Cost &amp; Shadow Prices</h1>
<p><strong>Reduced price</strong> is how much the decision variable coefficient would have change to become part of the solution make-up, or equivalently how much the profit/cost would change if you forced one of the items into the solution mix and adjusted the other variables to still meet requirements. It is only non-zero for variables at zero in the optimal solution.</p>
<p><strong>Shadow price</strong> on the other hand tells you how much the objective would change (e.g. Profit, Cost) by increasing that particular constraint’s RHS by 1 unit. This only applies to constraints that are binding (have zero slack).</p>
<h2 id="shadow-price-break-out">Shadow Price Break-Out</h2>

<table>
<thead>
<tr>
<th>Problem Type</th>
<th>Constraint Type</th>
<th>Increasing RHS Does What?</th>
<th>Shadow Price Sign</th>
</tr>
</thead>
<tbody>
<tr>
<td>Min</td>
<td>≥ (minimum requirement)</td>
<td>Raises cost</td>
<td>Positive</td>
</tr>
<tr>
<td>Min</td>
<td>≤ (resource limit)</td>
<td>Lowers cost</td>
<td>Negative</td>
</tr>
<tr>
<td>Max</td>
<td>≤ (resource limit)</td>
<td>Raises profit</td>
<td>Positive</td>
</tr>
<tr>
<td>Max</td>
<td>≥ (minimum production)</td>
<td>Lowers profit</td>
<td>Negative</td>
</tr>
</tbody>
</table><h2 id="reduced-cost-break-out">Reduced Cost Break-Out</h2>

<table>
<thead>
<tr>
<th>Problem Type</th>
<th>Variable Status</th>
<th>What Must Happen for Variable to Enter?</th>
<th>Reduced Cost Sign</th>
</tr>
</thead>
<tbody>
<tr>
<td>Max</td>
<td>At 0 (nonbasic)</td>
<td>Coefficient must increase</td>
<td>Negative or Zero</td>
</tr>
<tr>
<td>Min</td>
<td>At 0 (nonbasic)</td>
<td>Coefficient must decrease</td>
<td>Positive or Zero</td>
</tr>
<tr>
<td>Max</td>
<td>Positive</td>
<td>Already in solution</td>
<td>Zero</td>
</tr>
<tr>
<td>Min</td>
<td>Positive</td>
<td>Already in solution</td>
<td>Zero</td>
</tr>
</tbody>
</table><h2 id="allowable-ranges-break-out">Allowable Ranges Break-Out</h2>

<table>
<thead>
<tr>
<th>What You Change</th>
<th>Does Mix Change?</th>
<th>Does Objective Change?</th>
<th>What Stays Valid within Allowable Range?</th>
</tr>
</thead>
<tbody>
<tr>
<td>Objective coefficient</td>
<td>No</td>
<td>Yes</td>
<td>Reduced costs &amp; shadow prices</td>
</tr>
<tr>
<td>RHS of constraint</td>
<td>Yes (usually)</td>
<td>Yes</td>
<td>Shadow prices</td>
</tr>
</tbody>
</table><blockquote>
<p>Written with <a href="https://stackedit.io/">StackEdit</a>.</p>
</blockquote>


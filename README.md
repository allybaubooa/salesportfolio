<h1 align="center">📊 Sales Dashboard – Power BI</h1>

<p align="center">
  <em>A modern, interactive sales analytics dashboard built with Power BI and DAX.</em>
</p>

<br/>

<p align="center">
  <!-- Replace the src with your actual image path -->
  <img src="screenshots/dashboard.jpg" alt="Sales Dashboard Preview" width="900">
</p>

<br/>

<hr/>

<h2>🚀 Overview</h2>

<p>
This project showcases a complete <strong>Sales Analytics Dashboard</strong> developed in <strong>Power BI</strong>.  
The goal was to combine <strong>clean UI/UX</strong>, <strong>advanced DAX</strong>, and <strong>business-focused KPIs</strong> into a dashboard that feels like a modern SaaS analytics product.
</p>

<ul>
  <li>End-to-end report design (data model → DAX → visuals → layout)</li>
  <li>Year-over-year performance analysis (CY vs LY vs LLY)</li>
  <li>Sales, Quantity, Discount and Return Rate KPIs</li>
  <li>Clear storytelling across products, regions and time</li>
</ul>

<hr/>

<h2>🎯 Key Features</h2>

<h3>1️⃣ Dynamic KPI Cards</h3>

<p>
Each KPI card includes:
</p>

<ul>
  <li><strong>Current Year</strong> value</li>
  <li><strong>ΔCY</strong> – change vs same period last year</li>
  <li><strong>ΔLY</strong> – change vs the previous year’s LY</li>
  <li>Mini <strong>sparkline</strong> to show trend</li>
  <li>Conditional <strong>▲ / ▼</strong> indicators based on performance</li>
</ul>

<p>The main KPIs are:</p>

<ul>
  <li><strong>Sales</strong></li>
  <li><strong>Quantity Sold</strong></li>
  <li><strong>Average Discount</strong></li>
  <li><strong>Return Rate</strong></li>
</ul>

<h3>2️⃣ Sales vs Last Year Trend</h3>

<p>
A dual-line chart compares:
</p>

<ul>
  <li><strong>P</strong> – current year sales</li>
  <li><strong>P-1</strong> – previous year sales for the same period</li>
</ul>

<p>
This view highlights seasonality, monthly spikes and drops, and year-over-year changes in a single visual.
</p>

<h3>3️⃣ Regional Performance</h3>

<ul>
  <li><strong>Sales by Region</strong> – North, Central, East, West, South</li>
  <li><strong>Toggle</strong> between <em>Sales</em> and <em>Quantity</em> using a custom button selector</li>
</ul>

<h3>4️⃣ Top Product Rankings</h3>

<p>
A dedicated panel shows:
</p>

<ul>
  <li><strong>Top 5 Products by Sales</strong></li>
  <li><strong>Top 5 Products by Quantity</strong></li>
</ul>

<p>
Each bar is labeled with a formatted value such as:
</p>

<pre>
Chair  $168K
Laptop 534 units
</pre>

<hr/>

<h2>🧠 DAX Highlights</h2>

<p>
The dashboard relies heavily on DAX for time intelligence, growth calculations, and ranking logic.
Below are a few core measures:
</p>

<h3>Total Sales</h3>

<pre>
Total Sales =
SUM ( 'Product Sales Region'[TotalPrice] )
</pre>

<h3>Sales LY (Last Year)</h3>
<pre>
Sales LY =
CALCULATE (
    [Total Sales],
    SAMEPERIODLASTYEAR ( 'Calendar'[Date] )
)
</pre>

<h3>Sales CY Growth % (CY vs LY)</h3>

<pre>
Sales CY Growth % =
DIVIDE (
    [Sales CY] - [Sales LY],
    [Sales LY]
)
</pre>

<h3>Return Rate</h3>
<pre>
Return Rate =
DIVIDE (
    SUM ( 'Product Sales Region'[Returned] ),
    COUNTROWS ( 'Product Sales Region' )
)
</pre>
<h2>🎯 Purpose</h2> <p> This dashboard was built as part of a personal analytics portfolio to demonstrate: </p> <ul> <li>Strong <strong>Power BI</strong> skills</li> <li>Practical <strong>DAX</strong> for business reporting</li> <li>Modern <strong>dashboard design</strong> and layout</li> <li>Ability to translate raw data into meaningful insights</li> </ul> <hr/> 
<hr/>

<h2>🤝 Connect With Me</h2>

<p>
If you'd like to connect, collaborate, or discuss opportunities related to data analytics, Power BI, or dashboard design, feel free to reach out through the links below:
</p>

<ul>
  <li>
    <strong>LinkedIn:</strong>
    <a href="https://www.linkedin.com/in/ally-hussein-baubooa" target="_blank">
      https://www.linkedin.com/in/ally-hussein-baubooa
    </a>
  </li>

  <li>
    <strong>Portfolio Website:</strong>
    <a href="https://ally-devportfolio.vercel.app" target="_blank">
      https://ally-devportfolio.vercel.app
    </a>
  </li>

  <li>
    <strong>GitHub Profile:</strong>
    <a href="https://github.com/allybaubooa" target="_blank">
      https://github.com/allybaubooa
    </a>
  </li>

  <li>
    <strong>Email:</strong>
    <a href="mailto:allyhusseinbaubooa@gmail.com">
      allyhusseinbaubooa@gmail.com
    </a>
  </li>
</ul>

<p>Always happy to connect with fellow developers, analysts, and data enthusiasts!</p>

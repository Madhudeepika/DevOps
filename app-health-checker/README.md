<h2>What is this project?</h2>
<p><b>This is a simple app checking program.</b></p>
<p>It checks: <br>
<b>"Is my application working or not?"</b></p>

<hr>

<h2> Why I did this?</h2>
<p>In real companies:</p>
<ul>
  <li>Apps should not go down</li>
  <li>Systems should always run</li>
  <li>So we need <b>monitoring</b></li>
</ul>
<p>This project helps me understand that.</p>

<hr>

<h2> What my code is doing (step by step)</h2>

<h3>1️. I gave one URL</h3>
<pre><code>url = "https://jsonplaceholder.typicode.com/posts/1"</code></pre>
<p> This is like my <b>"application"</b></p>

<h3>2️. I check it multiple times</h3>
<pre><code>for attempt in range(1, 4):</code></pre>
<p> Means:</p>
<ul>
  <li>Checking again and again</li>
  <li>Like real systems monitor continuously</li>
</ul>

<h3>3️. Sending request</h3>
<pre><code>response = requests.get(url)</code></pre>
<p> Asking: <b>"Hey app, are you working?"</b></p>

<h3>4️.Checking response</h3>
<pre><code>if response.status_code == 200:</code></pre>
<p> <b>200 means:</b> App is working ✔</p>
<p>Else: Something is wrong </p>

<h3>5️.Waiting between checks</h3>
<pre><code>time.sleep(2)</code></pre>
<p>Like real monitoring tools (not checking every second)</p>

<h3>6️.Final alert</h3>
<pre><code>if response.status_code != 200:</code></pre>
<p> If not working → <b>ALERT</b></p>

<hr>

<h2>What I learned</h2>
<ul>
  <li>How apps are monitored</li>
  <li>What is status code</li>
  <li>Basic DevOps thinking</li>
  <li>Automation idea</li>
</ul>

<hr>

<h2>Real world connection</h2>
<p>In companies they use tools like:</p>
<ul>
  <li><b>Prometheus</b></li>
  <li><b>Grafana</b></li>
</ul>
<p>My project is a <b>basic version of this</b></p>


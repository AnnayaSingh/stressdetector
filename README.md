<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
</head>

<body>

<h1>🧠 NeuroWell – Stress Monitoring Dashboard</h1>

<p align="center">
<img src="NeuroWell DashBoard.png" width="800">
</p>


<p>
NeuroWell is a <strong>web-based mental wellness dashboard</strong> that connects to a 
BLE-enabled wearable device to monitor physiological signals such as 
<strong>❤️ Heart Rate, 🩸 SpO₂, and ⚡ Galvanic Skin Response (GSR)</strong>.
</p>

<p>
The system analyzes these signals to estimate a user's <span class="highlight">📊 stress level</span>
and provides calming suggestions, 🧘 breathing exercises, and 🤖 AI-assisted insights.
</p>

<section>
<h2>✨ Features</h2>

<div class="card">
<h3>📡 Real-Time Sensor Monitoring</h3>
<ul>
<li>❤️ Heart Rate (BPM)</li>
<li>🩸 Blood Oxygen Level (SpO₂)</li>
<li>⚡ Galvanic Skin Response (GSR)</li>
<li>📈 Real-time charts powered by Chart.js</li>
</ul>
</div>

<div class="card">
<h3>🧠 Stress Level Detection</h3>
<p>The system analyzes sensor data and classifies stress into:</p>
<ul>
<li class="highlight">😌 LOW</li>
<li class="highlight">⚠️ MODERATE</li>
<li class="highlight">🚨 HIGH</li>
</ul>
</div>

<div class="card">
<h3>🤖 AI Wellness Assistant</h3>
<p>
The dashboard integrates with Google's <strong>Gemini API</strong> to provide
personalized suggestions based on sensor readings.
</p>
</div>

<div class="card">
<h3>🧘 Guided Breathing Exercise</h3>
<ul>
<li>🌬 Animated inhale / exhale guide</li>
<li>⏱ Multiple breathing speeds</li>
<li>🎧 Ambient calming audio</li>
</ul>
</div>

<div class="card">
<h3>📜 Session History</h3>
<p>
The dashboard stores the <strong>last 10 sessions</strong> in local browser storage,
allowing users to track their stress patterns over time.
</p>
</div>

</section>

<section>
<h2>🛠 Technologies Used</h2>

<div class="card">
<ul>
<li>🌐 HTML5</li>
<li>🎨 CSS3</li>
<li>⚙️ JavaScript (Vanilla)</li>
<li>📊 Chart.js</li>
<li>📶 Web Bluetooth API</li>
<li>🤖 Google Gemini API</li>
<li>🌤 Open Meteo Weather API</li>
</ul>
</div>

</section>

<section>
<h2>🔌 Hardware Compatibility</h2>

<div class="card">
<ul>
<li>📡 ESP32 (BLE enabled)</li>
<li>❤️ MAX30102 Pulse Oximeter</li>
<li>⚡ GSR Sensor</li>
<li>🌡 Temperature sensor (optional)</li>
</ul>
</div>

</section>

<section>
<h2>⚙️ How It Works</h2>

<div class="card">

<ol>
<li>🔗 User connects the wearable device using Bluetooth.</li>
<li>📡 Dashboard receives live sensor readings.</li>
<li>📊 Data is visualized using real-time graphs.</li>
<li>⏱ After a 40 second test, the system calculates stress level.</li>
<li>💡 Suggestions and relaxation techniques are provided.</li>
</ol>

</div>

</section>

<section>
<h2>📊 Stress Calculation Logic</h2>

<div class="card">

<p>
Stress is calculated using a weighted combination of heart rate and skin conductance.
</p>

<pre>
Final Score =
(Heart Rate Score × 0.6)
+
(GSR Score × 0.4)
</pre>

<p>Stress categories:</p>

<ul>
<li>😌 0 – 45 : LOW</li>
<li>⚠️ 45 – 75 : MODERATE</li>
<li>🚨 75+ : HIGH</li>
</ul>

</div>

</section>

<section>
<h2>🚑 Emergency Support</h2>

<div class="card">

<p>If the user feels overwhelmed, emergency helplines are available:</p>

<ul>
<li>🚑 Ambulance: 102 / 108</li>
<li>👮 Police: 100 / 112</li>
<li>🧠 National Mental Health Helpline: 1800-599-0019</li>
</ul>

</div>

</section>

<section>
<h2>⚡ Setup Instructions</h2>

<div class="card">

<p>1️⃣ Download the project files.</p>

<p>2️⃣ Add your Gemini API key inside the JavaScript file:</p>

<code>const GEMINI_API_KEY = "YOUR_API_KEY";</code>

<p>3️⃣ Open the dashboard:</p>

<code>index.html</code>

<p>Recommended browsers:</p>
<ul>
<li>🌐 Google Chrome</li>
<li>🌐 Microsoft Edge</li>
</ul>

</div>

</section>

<section>
<h2 class="warning">⚠️ Disclaimer</h2>

<div class="card">

<p>
NeuroWell is a wellness monitoring tool and should not be considered
a medical diagnostic system.
</p>

</div>

</section>

<footer>
<p>© NeuroWell Project 🚀</p>
</footer>

</body>
</html>

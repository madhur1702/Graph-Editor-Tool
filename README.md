<h1 align="center">Graph Editor Tool</h1>

<p align="center">
An interactive <b>Graph Visualization & Algorithm Animation Tool</b><br>
Built using <b>Python</b> and <b>Pygame</b>, designed to run inside a <b>Jupyter Notebook.</b>.
</p>

<hr>

<h2>📌 Overview</h2>

<p>
Graph Editor Tool helps students and developers understand graph theory concepts visually.
</p>

<ul>
<li>Build graphs interactively</li>
<li>Toggle between Directed & Undirected modes</li>
<li>Run multiple graph algorithms</li>
<li>Watch smooth animated execution</li>
<li>No external assets required — everything is drawn using Pygame</li>
</ul>

<hr>

<h2>📂 Project Structure</h2>

<pre>
Graph Editor Tool/
│
└── GraphAlgo.ipynb      # Complete project implementation
</pre>

<p>The entire project is contained inside the notebook file.</p>

<hr>

<h2>🚀 Features</h2>

<h3>🏗 Graph Building</h3>
<ul>
<li>Add nodes by clicking on the canvas</li>
<li>Connect nodes by clicking two nodes consecutively</li>
<li>Delete nodes or edges individually</li>
<li>Toggle between <b>Directed</b> and <b>Undirected</b> graph mode</li>
<li>Undo / Redo support (<b>Ctrl + Z</b>, <b>Ctrl + Y</b>)</li>
<li>Clear the entire canvas instantly</li>
<li>Reset graph coloring anytime</li>
</ul>

<hr>

<h2>⚡ Algorithms with Real-Time Animation</h2>

<table border="1" cellpadding="8" cellspacing="0">
<tr>
<th>Algorithm</th>
<th>Description</th>
</tr>
<tr>
<td><b>DFS (Depth First Search)</b></td>
<td>Explores deeply before backtracking</td>
</tr>
<tr>
<td><b>BFS (Breadth First Search)</b></td>
<td>Explores level-by-level from source</td>
</tr>
<tr>
<td><b>Dijkstra (SSSP)</b></td>
<td>Finds shortest path between two nodes</td>
</tr>
<tr>
<td><b>Prim's MST</b></td>
<td>Finds Minimum Spanning Tree (Undirected only)</td>
</tr>
<tr>
<td><b>Bridges & Articulation Points</b></td>
<td>Detects critical nodes and edges</td>
</tr>
<tr>
<td><b>Cycle Detection</b></td>
<td>Detects cycles in both graph types</td>
</tr>
</table>

<hr>

<h2>🎨 Visual Indicators</h2>

<table border="1" cellpadding="8" cellspacing="0">
<tr>
<th>Color</th>
<th>Meaning</th>
</tr>
<tr>
<td>🟢 Green Node</td>
<td>Visited</td>
</tr>
<tr>
<td>🟠 Orange Node</td>
<td>Source</td>
</tr>
<tr>
<td>🔴 Red Node</td>
<td>Destination</td>
</tr>
<tr>
<td>🟡 Yellow Node</td>
<td>Articulation Point</td>
</tr>
<tr>
<td>🟢 Green Edge</td>
<td>Tree Edge</td>
</tr>
<tr>
<td>🔴 Red Edge</td>
<td>Back/Cross Edge</td>
</tr>
<tr>
<td>🔵 Blue Edge</td>
<td>Bridge</td>
</tr>
<tr>
<td>🟣 Purple Edge</td>
<td>MST Edge</td>
</tr>
<tr>
<td>🟡 Yellow Edge</td>
<td>Shortest Path</td>
</tr>
</table>

<hr>

<h2>🎮 Controls</h2>

<table border="1" cellpadding="8" cellspacing="0">
<tr>
<th>Action</th>
<th>Shortcut</th>
</tr>
<tr>
<td>Add Node</td>
<td><b>N</b></td>
</tr>
<tr>
<td>Add Edge</td>
<td><b>E</b></td>
</tr>
<tr>
<td>Toggle Directed Mode</td>
<td><b>D</b></td>
</tr>
<tr>
<td>Reset Colors</td>
<td><b>R</b></td>
</tr>
<tr>
<td>Undo</td>
<td><b>Ctrl + Z</b></td>
</tr>
<tr>
<td>Redo</td>
<td><b>Ctrl + Y</b></td>
</tr>
<tr>
<td>Cancel Current Action</td>
<td><b>ESC</b></td>
</tr>
</table>

<hr>

<h2>🖥 Installation & Setup</h2>

<h3>1️⃣ Install Requirements</h3>

<pre>
pip install pygame notebook
</pre>

<h3>2️⃣ Run the Project</h3>

<pre>
jupyter notebook
</pre>

<p>
Open:
</p>

<pre>
Graph Editor Tool/GraphAlgo.ipynb
</pre>

<p>
Click <b>Run All Cells</b> to start the application.
</p>

<hr>

<h2>🧵 Why Threading is Used</h2>

<p>
Using <code>pygame.time.delay()</code> freezes the entire window during animation.
</p>

<p>This project uses <b>Python threading</b> to:</p>

<ul>
<li>Keep the UI responsive</li>
<li>Run algorithms in the background</li>
<li>Provide smooth animation</li>
<li>Prevent window freezing</li>
</ul>

<hr>

<h2>🧠 Algorithm Implementation Details</h2>

<h3>DFS & BFS</h3>
<ul>
<li>DFS → Recursive traversal</li>
<li>BFS → Queue-based traversal</li>
<li>Live coloring during exploration</li>
</ul>

<h3>Dijkstra’s Algorithm</h3>
<ul>
<li>Uses Min-Heap (Priority Queue)</li>
<li>Tracks shortest distances</li>
<li>Highlights final shortest path</li>
</ul>

<h3>Prim’s Minimum Spanning Tree</h3>
<ul>
<li>Greedy approach</li>
<li>Uses Min-Heap</li>
<li>Works only on Undirected Graphs</li>
</ul>

<h3>Bridges & Articulation Points</h3>
<ul>
<li>Implemented using Tarjan’s Algorithm</li>
<li>Uses discovery time & low values</li>
</ul>

<h3>Cycle Detection</h3>
<ul>
<li>Directed → DFS with node coloring</li>
<li>Undirected → DFS with parent tracking</li>
</ul>

<hr>

<h2>🎯 Use Cases</h2>

<ul>
<li>Data Structures & Algorithms learning</li>
<li>Classroom demonstrations</li>
<li>Competitive programming preparation</li>
<li>Interview revision</li>
<li>Visual understanding of graph theory</li>
</ul>

<hr>

<h2>🤝 Contributing</h2>

<p>
Contributions are welcome!
</p>

<ul>
<li>Add new algorithms</li>
<li>Improve animation</li>
<li>Enhance UI</li>
<li>Optimize performance</li>
</ul>

<p>
Fork the repository and open a Pull Request.
</p>

<hr>

<h2>👨‍💻 Developed By</h2>

<p>
<b>Madhur Bhandarkar</b><br>
</p>

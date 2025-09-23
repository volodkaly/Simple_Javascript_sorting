<body style="font-family: Arial, sans-serif; line-height:1.6; margin: 20px;">

  <h1>📌 JavaScript Natural Sorting Example</h1>
 <a href="https://volodkaly.github.io/Simple_Javascript_sorting/" 
   target="_blank"
   style="
      display:inline-block;
      padding: 10px 20px;
      font-size: 16px;
      font-weight: 600;
      color: #fff;
      background-color: #198754;
      border: none;
      border-radius: 6px;
      text-decoration: none;
      text-align: center;
      transition: background-color 0.2s;
   "
   onmouseover="this.style.backgroundColor='#157347'" 
   onmouseout="this.style.backgroundColor='#198754'">
   <button>CLICK HERE TO TEST</button>
 </a>

  <h2>🚀 Problem</h2>
  <p>
    Normally, using JavaScript’s default <code>.sort()</code> gives wrong results:  
    <br><code>Version 10</code> appears before <code>Version 2</code>.
  </p>

  <h2>💡 Solution</h2>
  <pre><code>
numbers.sort((a, b) =>
  a.localeCompare(b, undefined, { numeric: true, sensitivity: 'base' })
);
  </code></pre>
  <ul>
    <li>✅ Case-insensitive</li>
    <li>✅ Correct numeric order</li>
  </ul>

  <h2>🖥️ Usage</h2>
  <ol>
    <li>Open <strong>index.html</strong> in your browser.</li>
    <li>Enter items separated by commas (e.g. <code>Version 100, version 1, Version 9.999, version 3.4</code>).</li>
    <li>Click <strong>Submit</strong> to see the sorted result.</li>
  </ol>

 
  <p style="font-size:0.9em; color:gray;">Made with ❤️ using vanilla JavaScript</p>

</body>
</html>

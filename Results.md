
<h1>SRAM Startup Randomness Analysis</h1>

<h2>Experiment 1: SRAM Random Bit Generation </h2>
<hr>

<h2>Statistical Analysis</h2>

<table>
    <tr>
        <th>Metric</th>
        <th>Value</th>
    </tr>
    <tr>
        <td>Total Bits</td>
        <td>1024</td>
    </tr>
    <tr>
        <td>Ones</td>
        <td>407</td>
    </tr>
    <tr>
        <td>Zeros</td>
        <td>617</td>
    </tr>
    <tr>
        <td>P(1)</td>
        <td>0.397461</td>
    </tr>
    <tr>
        <td>P(0)</td>
        <td>0.602539</td>
    </tr>
    <tr>
        <td>Shannon Entropy</td>
        <td>0.969446</td>
    </tr>
</table>

<hr>

<h2>Interpretation</h2>
<ul>
    <li>The bit distribution shows a bias toward 0.</li>
    <li>Entropy is close to 1, indicating strong randomness.</li>
    <li>SRAM startup behavior demonstrates high statistical unpredictability despite bias.</li>
</ul>

<hr>

<h2>Observations</h2>

<ul>
    <li>Output remains consistent across boots (indicating stable SRAM regions).</li>
    <li>Some spatial bias is visible in memory.</li>
    <li>Suitable for entropy-based applications with statistical post-processing.</li>
</ul>

<hr>

<h2>SRAM XOR Folding Experimental Results</h2>



<h3>SRAM XOR Folding Experimental Results</h3>

<hr>

<h2>Experiment 2: XOR Folding (Block Size = 8)</h2>

<table>
<tr>
    <th>Metric</th>
    <th>Value</th>
</tr>
<tr>
    <td>Total Bits</td>
    <td>128</td>
</tr>
<tr>
    <td>Ones</td>
    <td>42</td>
</tr>
<tr>
    <td>Zeros</td>
    <td>86</td>
</tr>
<tr>
    <td>P(1)</td>
    <td>0.328125</td>
</tr>
<tr>
    <td>P(0)</td>
    <td>0.671875</td>
</tr>
<tr class="highlight">
    <td>Shannon Entropy</td>
    <td>0.912999</td>
</tr>
</table>

<hr>

<h2>Experiment 3: XOR Folding (Block Size = 2)</h2>

<table>
<tr>
    <th>Metric</th>
    <th>Value</th>
</tr>
<tr>
    <td>Total Bits</td>
    <td>512</td>
</tr>
<tr>
    <td>Ones</td>
    <td>151</td>
</tr>
<tr>
    <td>Zeros</td>
    <td>361</td>
</tr>
<tr>
    <td>P(1)</td>
    <td>0.294922</td>
</tr>
<tr>
    <td>P(0)</td>
    <td>0.705078</td>
</tr>
<tr class="highlight">
    <td>Shannon Entropy</td>
    <td>0.874995</td>
</tr>
</table>

<hr>

<h2>Comparative Summary</h2>

<table>
<tr>
    <th>Stage</th>
    <th>Total Bits</th>
    <th>P(1)</th>
    <th>Entropy</th>
</tr>
<tr>
    <td>XOR Block = 8</td>
    <td>128</td>
    <td>0.328125</td>
    <td>0.912999</td>
</tr>
<tr>
    <td>XOR Block = 2</td>
    <td>512</td>
    <td>0.294922</td>
    <td>0.874995</td>
</tr>
</table>

<hr>

<h2>Analysis</h2>
<ul>
    <li>Reducing block size from 8 to 2 increased output bit count.</li>
    <li>However, bias toward zero increased.</li>
    <li>Entropy decreased as block size reduced.</li>
    <li>XOR folding alone did not eliminate spatial bias in SRAM startup data.</li>
</ul>


# CorLevelPlot
<h1>Visualise correlation results, e.g., clinical parameter correlations</h1>
<img src="https://github.com/kevinblighe/CorLevelPlot/blob/master/CorLevelPlot1.png">
<img src="https://github.com/kevinblighe/CorLevelPlot/blob/master/CorLevelPlot2.png"><br>
<h2>Requires</h2>
<ul>
  <li>lattice</li>
  <li>latticeExtra</li>
  <li>RColorBrewer</li>
  </ul>
<h2>Execution</h2>
<code>CorLevelPlot(df, x, y, labcex, strCorMethod, strPalette, iNumColours, boolReverse, boolPlotRSquared, strTitle)</code>
<br>
<h2>Parameters</h2>
<ul>
  <li>df, data-frame/matrix</li>
  <li>x, vector of column names in df</li>
  <li>y, vector of column names in df to be correlated to x</li>
  <li>labCex, size of the labels inside the plot area</li>
  <li>strCorMethod, one of "pearson", "kendall", "spearman"</li>
  <li>strPalette, one of RColorBrewer's palettes (see http://www.r-graph-gallery.com/38-rcolorbrewers-palettes/)</li>
  <li>iNumColours, number of colours to use in the palette (if too many chosen, the max will automatically be chosen)</li>
  <li>boolReverse, Reverse the palette? (TRUE/FALSE)</li>
  <li>boolPlotRSquared, plot R^2 values? (TRUE/FALSE)</li>
  <li>strTitle, plot title</li>
</ul>
<br>
<h2>Example</h2>
<code>CorLevelPlot(Mydata, c("PC1","PC2","PC3","PC4"), c("Batch","CaseControl","Gender"), 0.8, "spearman", "RdBu", 9, FALSE, FALSE, "PC correlation")</code>
<br>
<h2>Credits</h2>
<ul>
  <li>Kevin Blighe (Queen Mary University of London)</li>
  <li>Myles Lewis (Queen Mary University of London)</li>
</ul>

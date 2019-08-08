# Introduction to Gephi

This tutorial was written by <a href="https://www.grinnell.edu/users/waldenka">Katherine Walden</a>, Digital Liberal Arts Specialist at Grinnell College.

This tutorial was reviewed by <a href="https://www.grinnell.edu/users/purcelsj">Sarah Purcell</a> (L.F. Parker Professor of History) and <a href="https://www.grinnell.edu/users/donovang">Gina Donovan</a> (Instructional Technologist) at Grinnell College, and edited by Papa Ampim-Darko, a student research assistant at Grinnell College.

<a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license"><img style="border-width: 0;" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" alt="Creative Commons License" /></a>
Network Analysis-Part III (Gephi) is licensed under a <a href="http://creativecommons.org/licenses/by-nc/4.0/" rel="license">Creative Commons Attribution-NonCommercial 4.0 International License</a>.

<hr />

In the last tutorial, we used a browser-based tool to visualize and briefly analyze networks in the Quaker data. While Palladio is useful for preliminary visualization of network data, it offers limited options for calculating or analyzing more advanced network metrics. <a href="https://github.com/gephi/gephi">Gephi</a> is an open-source network analysis and visualization software created by students at the University of Technology of Compiègne in 2008. The Gephi Consortium, which supports the ongoing development and documentation for Gephi, is a non-profit corporation supported by members that include SciencesPo, Linfluence, WebAtlas, and Quid. Gephi runs on Linux, Windows, and macOS operating systems and is available in 9 different languages.

<hr />

## Installing Gephi

To download Gephi on your own computer, go to Gephi’s <a href="https://gephi.org/users/download/">download page</a> and select the correct version for your operating system.

<hr />

## Data

1-In this tutorial, we will be working with data about Grinnell faculty, the subject of their terminal degree, where they received their terminal degree, and when they were hired by the College.

2-Download the <strong>GC_faculty_nodesheet</strong> and <strong>GC_faculty_edgesheet</strong> CSV files to your Desktop. Open the files in Microsoft Excel to explore the data structure.
<ul>
 	<li>What types of institutions and College instructors are represented?</li>
 	<li>How are they described in the nodelist data?</li>
 	<li>What additional questions do you have about the individuals and degree-granting institutions that will be represented as nodes?</li>
 	<li>How is the edgelist data structured?</li>
 	<li>Based on a preliminary scan of the nodelist and edgelist CSV data, what types of networks do you think this data might illuminate?</li>
 	<li>Are there gaps, silences, or alternative networks that are not accounted for in the data?</li>
</ul>
3-Save these files to your desktop as “<strong>Grinnell_nodelist</strong>” and “<strong>Grinnell_edgelist</strong>” or another descriptive file name.

<hr />

## Loading Data into Gephi

4-Open <strong>Gephi</strong> by selecting it from <strong>Start-&gt;All Programs-&gt;Gephi</strong> or the <strong>Desktop icon</strong>.

5-Click the <strong>X</strong> in the top right-hand corner of the <strong>Welcome</strong> popup window.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture.PNG?raw=true" alt="" width="840" height="473" /></a></p>

6-Click <strong>File-&gt;Import Spreadsheet</strong> and navigate to the <strong>Desktop</strong> where the <strong>nodelist and edgelist CSV files</strong> are saved on your computer.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture2.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture2.PNG?raw=true" alt="" width="843" height="500" /></a></p>

7-Select the <strong>nodelist</strong> file, make sure <strong>Comma</strong> is selected as <strong>Separator</strong>, <strong>Nodes</strong> table is selected under <strong>Import as</strong>, and <strong>UTF-8 </strong>under <strong>Charset</strong>.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture3.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture3.PNG?raw=true" alt="" width="845" height="498" /></a></p>

8-Click <strong>Next</strong>. Leave the default settings on the <strong>Import settings (2 of 2)</strong> popup, and click <strong>Finish</strong>.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture4.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture4.PNG?raw=true" alt="" width="662" height="460" /></a></p>

9-Select <strong>Undirected</strong> for <strong>Graph Type</strong>, and switch the default selection from <strong>New workspace</strong> to <strong>Append to existing workspace</strong>.

10-Click <strong>OK</strong>.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture5.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture5.PNG?raw=true" alt="" width="840" height="475" /></a></p>

11-Your node data is now loaded in the <strong>Data Laboratory tab</strong> in Gephi.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture7.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture7.PNG?raw=true" alt="" width="763" height="114" /></a></p>

12-Click <strong>Import Spreadsheet</strong>, and select the CSV with your edgelist data.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture8.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture8.PNG?raw=true" alt="" width="824" height="493" /></a></p>

13-Make sure <strong>Comma</strong> is selected as <strong>Separator</strong>, <strong>Edges</strong> table under <strong>Import as</strong>, and <strong>UTF-8</strong> under <strong>Charset</strong>.

14-Click <strong>Next</strong>.

15-Leave the default settings on the <strong>Import settings (2 of 2)</strong> window and click <strong>Finish</strong>.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture9.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture9.PNG?raw=true" alt="" width="663" height="457" /></a></p>

16-Make sure <strong>Undirected</strong> is selected as <strong>Graph Type</strong>, and switch the default selection from <strong>New workspace</strong> to <strong>Append to existing workspace</strong>.

17-Click <strong>OK</strong>.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture10.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture10.PNG?raw=true" alt="" width="840" height="472" /></a></p>

18-Now our nodes and edges data has been imported in Gephi.

19-Click <strong>File-&gt;Save</strong> to save your project. Label the Gephi file “<strong>Network_Tutorial</strong>” or another descriptive name.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture11.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture11.PNG?raw=true" alt="" width="511" height="105" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture12.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture12.PNG?raw=true" alt="" width="840" height="472" /></a></p>

20-Click on the <strong>Overview</strong> tab to see Gephi’s default visualization of your network data.

21-As you probably noticed, the default visualization is an interesting connection of nodes and edges, but doesn’t do much to help us more fully understand and analyze our data.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture14.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture14.PNG?raw=true" alt="" width="366" height="141" /></a></p>

22-Click on <strong>Choose a layout</strong> under the <strong>Layout panel</strong> to select how Gephi displays your nodes and edges.

23-Gephi uses a variety of layout algorithms to determine the shape of network graphs. These different layouts algorithms highlight different aspects or features of your data.

<table>
<tbody>
<tr>
<td width="312">Divisions</td>
<td width="312">OpenOrd</td>
</tr>
<tr>
<td width="312">Complementarities</td>
<td width="312">ForceAtlas, Yifan Hu, Frushterman-Reingold</td>
</tr>
<tr>
<td width="312">Ranking</td>
<td width="312">Circular, Radial Axis</td>
</tr>
<tr>
<td width="312">Geographic Repartition</td>
<td width="312">GeoLayout</td>
</tr>
</tbody>
</table>

24-<strong>Label Adjust, Noverlap, Expansion, and Contraction</strong> make graphic adjustments to how your data displays, rather than using an underlying algorithm to change the structure of the network visualization.

25-<strong>Select different Layout options</strong> and click the <strong>Run</strong> icon to see how the different algorithms and settings change the visualization of your data. Click the <strong>Stop</strong> icon to stop the layout operation.

26-What Layout option(s) do you prefer, and why? How do different Layout options impact the visualization of your data? How could different Layout options be useful to answer different types of research questions?

<hr />

## Calculating Network Metrics in Gephi

27- As a GUI interface, Gephi allows us to calculate a variety of statistics without having to run the back-end code or use a library like NetworkX (which we will try next time).

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture15.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture15.PNG?raw=true" alt="" width="324" height="617" /></a></p>

28-The <strong>Statistics panel</strong> gives you the option to run a number of different calculations on your network data.

29-While Gephi allows us to easily perform these calculations, the program doesn’t automatically tell us what these measures mean or how they are calculated.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture16.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture16.PNG?raw=true" alt="" width="701" height="603" /></a></p>

30-The HTML report in the pop-up window that displays after you run a <strong>Statistics calculation</strong> gives you a graph of the data calculation, and sometimes the source for the algorithm used to calculate the statistic.

31-Consult <a href="https://github.com/gephi/gephi/wiki/Statistics">Gephi’s GitHub repository</a> for more information on these statistics.

32-Click <strong>Run</strong> for each of the options under <strong>Statistics</strong>.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture19.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture19.PNG?raw=true" alt="" width="840" height="473" /></a></p>

33-If you click on the <strong>Data Laboratory tab</strong>, you will see these calculated statistics have been added to your network data.

34-What do these statistics tell you about your network? How do these statistics help you understand your network data more deeply? What questions do you have about the network data or these calculations?

<hr />

## Customizing a Network Visualization in Gephi

35-Select <strong>Noverlap</strong> for your <strong>Layout</strong> so your nodes and edges don’t overlap as you are exploring display customization options.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture21.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture21.PNG?raw=true" alt="" width="840" height="655" /></a></p>

36-The <strong>border icons in the Graph panel</strong> allow you to customize the display of your network visualization.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture22.PNG?raw=true"><img class="size-full wp-image-196 alignright" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture22.PNG?raw=true" alt="" width="28" height="24" /></a></p>

37-Click on the <strong>Show Node Labels icon</strong> to display the node labels. You can change the size of text for your labels by using the slider to the right of “Arial Bold, 32.”

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture24.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture24.PNG?raw=true" alt="" width="359" height="362" /></a></p>

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture23.PNG?raw=true"><img class="alignright" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture23.PNG?raw=true" alt="" width="22" height="29" /></a></p>

38-You can also click on the <strong>Attributes icon</strong> to customize what data fields display as part of your labels.

39-While your nodes now have labels, the large number of nodes and edges makes it difficult to differentiate or discern various attributes about our network data.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture20.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture20.PNG?raw=true" alt="" width="347" height="110" /></a></p>

40-The <strong>Appearance panel</strong> allows you to customize the color, size or weight, and labels for your nodes and edges. Changing the coloring or sizing of nodes in the Appearance panel can help make our network visualization more meaningful.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture26.PNG?raw=true"><img class="alignright" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture26.PNG?raw=true" alt="" width="24" height="25" /></a></p>

41-Select the <strong>Size icon  </strong>to change the default size of your nodes. You can explore different sizes, but 3 works well with this dataset. Click the <strong>Apply icon</strong> to change the setting for your network visualization.

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture27.PNG?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Capture27.PNG?raw=true" alt="" width="349" height="330" /></a></p>

42-You can also rank the size of nodes based on one of the network metrics you calculated in the Statistics panel.

43-Click the <strong>Ranking icon</strong> in the Appearance panel, and select <strong>Degree</strong> from the dropdown menu. Click <strong>Apply</strong>.

44-Ranking our node size by degree determines the size of a node based on its degree of centrality (or connectedness). Nodes with higher numbers of connections appear larger, and nodes with lower numbers of connections are smaller.

45-What changes did you notice in your network visualization after sizing nodes by degree? How does changing the size of nodes impact your understanding of the network data? What do you see in the network data after this change that you weren’t able to see before?

46-You can change the minimum and maximum node size, and also select different statistics to use for determining node size.

47-Explore these different settings and options to see how different node size calculations shape your understanding of the network data.

48-Save your project.

<hr />

## Exporting Networks

<p align="center"><a href="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Picx.png?raw=true"><img class="aligncenter" src="https://github.com/kwaldenphd/Gephi-tutorial/blob/master/screenshots/Picx.png?raw=true" alt="" width="244" height="264" /></a></p>

49-Click <strong>File-&gt;Export</strong> to save your project as a static image (SVG, PNG, PDF) or network file (CSV, GDF, GEXF, GraphML, Pajek Net).

50-You can learn more about the different export options on <a href="https://gephi.org/users/supported-graph-formats/">Gephi’s website documentation</a>.

51-Step 47 in this tutorial had you experiment with display customization settings.

52-Return to the visualizations you explored in that step, and export those you find useful or interesting as PNG files.

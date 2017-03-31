chart-tools
===========

Open source reusable charting tools workshop for the Hacks/ Hackers Buenos Aires Media Party, 2014

*To clone all submodules (charting tools and their docs), run:
`git clone --recursive https://github.com/bchartoff/chart-tools.git`*

This is far from a comprehensive list of chart creation tools, instead it focusses on a few tools that meet the followsing criteria:
- Open Source projects
- Able to create at least the two basic chart types: bar charts and line/ scatter plots (a few of these tools don't yet offer scatter plots)
- Focussed on creating basic chart types, rather than more niche charts (Sankey diagrams, Tree maps, etc.)

Any of these tools could be used out-of-the-box in your newsroom, or modified to create a custom tool.

## GUI based tools

#### Chartbuilder
- [github repo](https://github.com/Quartz/Chartbuilder)
- [project page](http://quartz.github.io/Chartbuilder/)

One of the easier tools to use, builds bar and line charts in browser. Needs only means to run local server (e.g.[python simpleHTTPServer](https://docs.python.org/2/library/simplehttpserver.html) or [node http-server](https://github.com/nodeapps/http-server)). Built in D3, static output. See also [NPR's fork](https://github.com/nprapps/Chartbuilder).

#### Datamatic.io
- [gui](http://datamatic.io/)
- [tutorial](https://medium.com/@DatamaticIO/how-to-make-an-interactive-d3-js-visualization-using-datamatic-io-3c0663040eff)

Datamatic is a visualization generator based on the d3.js library and ported from google sheets data.

#### Datawrapper
- [github repo](https://github.com/datawrapper/datawrapper)
- [project page](https://datawrapper.de/)

An in-browswer tool that handles a few steps such as user accounts, saving graphs, etc. Live version is free (for now) and account based, but is possible to host on your own servers (mySQL, Apache, PHP). Javascript plugin based. [The Washington Post's fork](https://github.com/washingtonpost/datawrapper) is here.

#### Lyra
- [github repo](https://github.com/uwdata/lyra)

A full pipeline of data manipulation/ graph creation/ export without needing to write code. The goal is to be extremely customizable by marking arbitrary marks/ visual elements to data, but it means that there's a steep learning curve. Jim Vallandingham's [let's make a bar chart in Lyra](http://vallandingham.me/make_a_barchart_with_lyra.html) is a great place to start.

#### Charted
- [github repo](https://github.com/mikesall/charted)
- [project page](http://www.charted.co/)

Charted is a tool that automatically visualizes data, created by the Product Science team at Medium. Give it the link to a data file and Charted returns a beautiful, shareable visualization of that data.

#### TinyChart
- [project page](http://tinychart.co/)
Tiny Chart allows you to load data as a table or json and visualize/export as a quick and simple chart. It's an anomaly on this page as it's not (yet) open source, but it is free to use in the in-browser gui.

## Code based tools

#### d3.chart
- [github repo](https://github.com/misoproject/d3.chart)
- [project page](http://misoproject.com/d3-chart/)

A charting framework that is in a sense a refactor of d3, with the specific goal of creating reusable charts. Reusable is defined by miso as: **repeatable, configurable, extensible, and composable**.

#### nvd3 
- [github repo](https://github.com/novus/nvd3)
- [project page](http://nvd3.org/)

While nvd3 requires writing code to build graphics, it's a pretty minimal amount of code to produce a basic chart. Uses d3 syntax for setting options, but handles much of the charting framework. [A bar chart example](https://github.com/novus/nvd3/blob/master/examples/discreteBarChart.html) *Note: currently in the middle of a major refactor.*

#### dc.js
- [github repo](https://github.com/dc-js/dc.js)
- [project page](http://dc-js.github.io/dc.js/)

Browser/mobile friendly  multi-dimensional charting library with native [crossfilter](http://square.github.io/crossfilter/) support; allowing exploration on large multi-dimensional datasets (inspired by crossfilter's demo). dc.js leverages d3 engine to render charts in css-friendly svg format.

#### cola.js
- [github repo](https://github.com/tgdwyer/WebCola)
- [project page](http://marvl.infotech.monash.edu/webcola/)

Cola advertises as a "constraint based layout in the browser," or an open source javascript library that handles force layouts (from D3 or other), more elegantly accommodating constraing optimizations.

#### rickshaw
- [github repo](https://github.com/shutterstock/rickshaw)
- [project page](http://code.shutterstock.com/rickshaw/)

Similar to nvd3 in that it requires a small amount of code to build complex graphics. Less tightly tied to d3 syntax than nvd3, and more of a focus on interactive graphics. Various features such as streaming data supported via plugins.

#### tau 
- [github repo](https://github.com/TargetProcess/tauCharts)
- [project page](http://blog.taucharts.com/taucharts-data-focused-charting-library/)

A free, open source, "data friendly" library for charting. Similar to Vega's Visual grammar, they describe the API simply as such: "Taucharts DSL describes composition of graphical components and mapping of data variables (columns) to the scales and components properties." They also have a package of plugins to make it easier to process.

#### vega
- [github repo](https://github.com/trifacta/vega)
- [project page](http://trifacta.github.io/vega/)

Ambitious library that includes large number of chart types, both standard and d3-esque. Simple charts are again straightforward to construct (data object plus config object). Editor "tool" is not quite a chartbuilding tool, but allows easy side by side code/ graph comparisons.

#### Highcharts 
- [github repo](https://github.com/highslide-software/highcharts.com/)
- [project page](http://www.highcharts.com/)

Built in native JS (not d3), but similar to above projects, in that it requires only simple code. Very well supported, excellent documentation, stable product.

## Command line based tool

#### NPR's daily graphics rig
- [github repo](https://github.com/nprapps/dailygraphics)

An interesting example of a charting tool implemented within a newsroom, start to finish (pulling data from google spreadsheets, deploy to s3, embed in responsive iframe). Included not because of the charts themselves, but the context surrounding them. Run from the command line, using fabric.

## Other resources

[Sitepoint round-up](http://www.sitepoint.com/15-best-javascript-charting-libraries/)






<!DOCTYPE html>

<html xmlns="http://www.w3.org/1999/xhtml">

<head>

<meta charset="utf-8" />
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<meta name="generator" content="pandoc" />


<meta name="author" content="Author:MUSA T GANIYU" />


<title>|IS 608 KNOWLEDGE AND VISUAL ANALYTICS - PROJECT PROPOSAL | Data Analytics</title>

<style type="text/css">code{white-space: pre;}</style>
<style type="text/css">
div.sourceCode { overflow-x: auto; }
table.sourceCode, tr.sourceCode, td.lineNumbers, td.sourceCode {
  margin: 0; padding: 0; vertical-align: baseline; border: none; }
table.sourceCode { width: 100%; line-height: 100%; background-color: #f8f8f8; }
td.lineNumbers { text-align: right; padding-right: 4px; padding-left: 4px; color: #aaaaaa; border-right: 1px solid #aaaaaa; }
td.sourceCode { padding-left: 5px; }
pre, code { background-color: #f8f8f8; }
code > span.kw { color: #204a87; font-weight: bold; } /* Keyword */
code > span.dt { color: #204a87; } /* DataType */
code > span.dv { color: #0000cf; } /* DecVal */
code > span.bn { color: #0000cf; } /* BaseN */
code > span.fl { color: #0000cf; } /* Float */
code > span.ch { color: #4e9a06; } /* Char */
code > span.st { color: #4e9a06; } /* String */
code > span.co { color: #8f5902; font-style: italic; } /* Comment */
code > span.ot { color: #8f5902; } /* Other */
code > span.al { color: #ef2929; } /* Alert */
code > span.fu { color: #000000; } /* Function */
code > span.er { color: #a40000; font-weight: bold; } /* Error */
code > span.wa { color: #8f5902; font-weight: bold; font-style: italic; } /* Warning */
code > span.cn { color: #000000; } /* Constant */
code > span.sc { color: #000000; } /* SpecialChar */
code > span.vs { color: #4e9a06; } /* VerbatimString */
code > span.ss { color: #4e9a06; } /* SpecialString */
code > span.im { } /* Import */
code > span.va { color: #000000; } /* Variable */
code > span.cf { color: #204a87; font-weight: bold; } /* ControlFlow */
code > span.op { color: #ce5c00; font-weight: bold; } /* Operator */
code > span.pp { color: #8f5902; font-style: italic; } /* Preprocessor */
code > span.ex { } /* Extension */
code > span.at { color: #c4a000; } /* Attribute */
code > span.do { color: #8f5902; font-weight: bold; font-style: italic; } /* Documentation */
code > span.an { color: #8f5902; font-weight: bold; font-style: italic; } /* Annotation */
code > span.cv { color: #8f5902; font-weight: bold; font-style: italic; } /* CommentVar */
code > span.in { color: #8f5902; font-weight: bold; font-style: italic; } /* Information */
</style>
<style type="text/css">
  pre:not([class]) {
    background-color: white;
  }
</style>


<style type="text/css">
h1 {
  font-size: 34px;
}
h1.title {
  font-size: 38px;
}
h2 {
  font-size: 30px;
}
h3 {
  font-size: 24px;
}
h4 {
  font-size: 18px;
}
h5 {
  font-size: 16px;
}
h6 {
  font-size: 12px;
}
.table th:not([align]) {
  text-align: left;
}
</style>


</head>

<body>

<style type="text/css">
.main-container {
  max-width: 940px;
  margin-left: auto;
  margin-right: auto;
}
code {
  color: inherit;
  background-color: rgba(0, 0, 0, 0.04);
}
img {
  max-width:100%;
  height: auto;
}
.tabbed-pane {
  padding-top: 12px;
}
button.code-folding-btn:focus {
  outline: none;
}
</style>



<div class="container-fluid main-container">

<!-- tabsets -->
<script>
$(document).ready(function () {
  window.buildTabsets("TOC");
});
</script>

<!-- code folding -->




<script>
$(document).ready(function ()  {

    // move toc-ignore selectors from section div to header
    $('div.section.toc-ignore')
        .removeClass('toc-ignore')
        .children('h1,h2,h3,h4,h5').addClass('toc-ignore');

    // establish options
    var options = {
      selectors: "h1,h2",
      theme: "bootstrap3",
      context: '.toc-content',
      hashGenerator: function (text) {
        return text.replace(/[.\\/?&!#<>]/g, '').replace(/\s/g, '_').toLowerCase();
      },
      ignoreSelector: ".toc-ignore",
      scrollTo: 0
    };
    options.showAndHide = true;
    options.smoothScroll = false;

    // tocify
    var toc = $("#TOC").tocify(options).data("toc-tocify");
});
</script>

<style type="text/css">

#TOC {
  margin: 25px 0px 20px 0px;
}
@media (max-width: 768px) {
#TOC {
  position: relative;
  width: 100%;
}
}


.toc-content {
  padding-left: 30px;
  padding-right: 40px;
}

div.main-container {
  max-width: 1200px;
}

div.tocify {
  width: 20%;
  max-width: 260px;
  max-height: 85%;
}

@media (min-width: 768px) and (max-width: 991px) {
  div.tocify {
    width: 25%;
  }
}

@media (max-width: 767px) {
  div.tocify {
    width: 100%;
    max-width: none;
  }
}

.tocify ul, .tocify li {
  line-height: 20px;
}

.tocify-subheader .tocify-item {
  font-size: 0.90em;
  padding-left: 25px;
  text-indent: 0;
}

.tocify .list-group-item {
  border-radius: 0px;
}


</style>

<!-- setup 3col/9col grid for toc_float and main content  -->
<div class="row-fluid">
<div class="col-xs-12 col-sm-4 col-md-3">
<div id="TOC" class="tocify">
</div>
</div>

<div class="toc-content col-xs-12 col-sm-8 col-md-9">




<div class="fluid-row" id="header">



<h1 class="title toc-ignore"><p>|IS 608 KNOWLEDGE AND VISUAL ANALYTICS - PROJECT PROPOSAL | Data Analytics</p></h1>
<h4 class="author"><em>Author:MUSA T GANIYU</em></h4>
<h4 class="date"><em>OCT. 20th, 2017</em></h4>

</div>


<div id="aim" class="section level2">
<h2>Aim:</h2>
<p>The goal of this project is to:</p>
<ul>
<li>Show the merit and demerit of visual analytics on data analysis, and how to improve it.</li>
<li>Provide answer to the question, “Does demographics like Age, Sex, Location have impact on types of death, economic status?”</li>
<li>Make the visualized image(s) tells the story in an unambiguous way, understandable, even to a layman!</li>
</ul>
</div>
<div id="methodology" class="section level2">
<h2>Methodology:</h2>
<p>The project would lay more emphasis on the explanatory techniques. It will be used in making data presentation to the viewers in a more succinct way. I therefore plan to use the R programing language to explore and analysis the dataset.</p>
<p>The dataset to be used is the World Health Nutrition and Population Statistics from year 2010 to 2016 . This can be obtained from <a href="http://databank.worldbank.org/data/reports.aspx?source=health-nutrition-and-population-statistics#advancedDownloadOptions" class="uri">http://databank.worldbank.org/data/reports.aspx?source=health-nutrition-and-population-statistics#advancedDownloadOptions</a> .</p>
<p>Load this libraries and dataset and lets get to work!</p>
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r"><span class="kw">suppressMessages</span>(<span class="kw">library</span>(knitr))
<span class="kw">suppressMessages</span>(<span class="kw">library</span>(dplyr))
<span class="kw">suppressMessages</span>(<span class="kw">library</span>(ggplot2))
<span class="kw">suppressMessages</span>(<span class="kw">library</span>(plotly))
<span class="kw">suppressMessages</span>(<span class="kw">library</span>(sqldf))
<span class="kw">suppressPackageStartupMessages</span>(<span class="kw">library</span>(googleVis))</code></pre></div>
<pre><code>## Creating a generic function for 'toJSON' from package 'jsonlite' in package 'googleVis'</code></pre>
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r">df &lt;-<span class="st"> </span><span class="kw">read.csv</span>(<span class="st">&quot;World_Health_2.csv&quot;</span>, <span class="dt">header =</span> <span class="ot">TRUE</span>, <span class="dt">sep =</span> <span class="st">&quot;,&quot;</span>, <span class="dt">stringsAsFactors =</span> <span class="ot">FALSE</span>)
<span class="kw">kable</span>(<span class="kw">head</span>(df[<span class="dv">200</span>:<span class="dv">206</span>, ]))</code></pre></div>
<table>
<thead>
<tr class="header">
<th></th>
<th align="left">Series_Name</th>
<th align="left">Series_Code</th>
<th align="left">Country_Name</th>
<th align="left">Country_Code</th>
<th align="left">YR1960</th>
<th align="left">YR1970</th>
<th align="left">YR1980</th>
<th align="left">YR1990</th>
<th align="left">YR2000</th>
<th align="left">YR2010</th>
<th align="left">YR2015</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>200</td>
<td align="left">Children (ages 0-14) newly infected with HIV</td>
<td align="left">SH.HIV.INCD.14</td>
<td align="left">Saudi Arabia</td>
<td align="left">SAU</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">100</td>
<td align="left">100</td>
<td align="left">100</td>
<td align="left">100</td>
</tr>
<tr class="even">
<td>201</td>
<td align="left">Children (ages 0-14) newly infected with HIV</td>
<td align="left">SH.HIV.INCD.14</td>
<td align="left">Senegal</td>
<td align="left">SEN</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">200</td>
<td align="left">1000</td>
<td align="left">1000</td>
<td align="left">500</td>
</tr>
<tr class="odd">
<td>202</td>
<td align="left">Children (ages 0-14) newly infected with HIV</td>
<td align="left">SH.HIV.INCD.14</td>
<td align="left">Serbia</td>
<td align="left">SRB</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
</tr>
<tr class="even">
<td>203</td>
<td align="left">Children (ages 0-14) newly infected with HIV</td>
<td align="left">SH.HIV.INCD.14</td>
<td align="left">Seychelles</td>
<td align="left">SYC</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
</tr>
<tr class="odd">
<td>204</td>
<td align="left">Children (ages 0-14) newly infected with HIV</td>
<td align="left">SH.HIV.INCD.14</td>
<td align="left">Sierra Leone</td>
<td align="left">SLE</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">200</td>
<td align="left">500</td>
<td align="left">1000</td>
<td align="left">500</td>
</tr>
<tr class="even">
<td>205</td>
<td align="left">Children (ages 0-14) newly infected with HIV</td>
<td align="left">SH.HIV.INCD.14</td>
<td align="left">Singapore</td>
<td align="left">SGP</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
<td align="left">..</td>
</tr>
</tbody>
</table>
<ul>
<li>World longitudes and latitudes</li>
</ul>
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r">lat_long &lt;-<span class="st"> </span><span class="kw">read.csv</span>(<span class="st">&quot;Countries_long_lat2.csv&quot;</span>, <span class="dt">header =</span> <span class="ot">TRUE</span>, <span class="dt">sep =</span> <span class="st">&quot;,&quot;</span>)
<span class="kw">colnames</span>(lat_long) &lt;-<span class="st"> </span><span class="kw">c</span>(<span class="st">&quot;Country&quot;</span>, <span class="st">&quot;Country_Code&quot;</span>, <span class="st">&quot;Latitude&quot;</span>, <span class="st">&quot;Longtitude&quot;</span>)
<span class="kw">kable</span>(<span class="kw">head</span>(lat_long))</code></pre></div>
<table>
<thead>
<tr class="header">
<th align="left">Country</th>
<th align="left">Country_Code</th>
<th align="right">Latitude</th>
<th align="right">Longtitude</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left">Albania</td>
<td align="left">ALB</td>
<td align="right">41.0000</td>
<td align="right">20.0000</td>
</tr>
<tr class="even">
<td align="left">Algeria</td>
<td align="left">DZA</td>
<td align="right">28.0000</td>
<td align="right">3.0000</td>
</tr>
<tr class="odd">
<td align="left">American Samoa</td>
<td align="left">ASM</td>
<td align="right">-14.3333</td>
<td align="right">-170.0000</td>
</tr>
<tr class="even">
<td align="left">Andorra</td>
<td align="left">AND</td>
<td align="right">42.5000</td>
<td align="right">1.6000</td>
</tr>
<tr class="odd">
<td align="left">Angola</td>
<td align="left">AGO</td>
<td align="right">-12.5000</td>
<td align="right">18.5000</td>
</tr>
<tr class="even">
<td align="left">Anguilla</td>
<td align="left">AIA</td>
<td align="right">18.2500</td>
<td align="right">-63.1667</td>
</tr>
</tbody>
</table>
<p>Cleaning and renaming of dataset and column respectively.</p>
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r"><span class="kw">options</span>(<span class="dt">warn =</span> -<span class="dv">1</span>)
df2 &lt;-<span class="st"> </span><span class="kw">merge</span>(df, lat_long, <span class="dt">by.x =</span> <span class="st">&quot;Country_Code&quot;</span>, <span class="dt">by.y =</span> <span class="st">&quot;Country_Code&quot;</span>, <span class="dt">all =</span> <span class="ot">FALSE</span>)
df2[, <span class="dv">5</span>:<span class="dv">11</span>] &lt;-<span class="st"> </span><span class="kw">sapply</span>(df2[, <span class="dv">5</span>:<span class="dv">11</span>], as.numeric)</code></pre></div>
<p>Merging column lonitude and Latitude together for a better coordinate to be in maps (googlevis)</p>
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r">df2$Lat_Long =<span class="st"> </span><span class="kw">paste</span>(df2$Latitude, df2$Longtitude, <span class="dt">sep=</span><span class="st">&quot;:&quot;</span>)</code></pre></div>
<blockquote>
<p>we are now to goint make use of sql to subset(query) columns so as to diffentiate between year 2000 and 2010 where the number children orphaned by HIV/AIDS more than 50000.</p>
</blockquote>
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r">sq &lt;-<span class="st"> </span><span class="kw">sqldf</span>(<span class="st">&quot;select Lat_Long, Country_Name, YR2000, YR2010 from df2 </span>
<span class="st">            where YR2010 &gt;= 50000 and YR2000 &gt;= 50000 and Series_Name ='Children orphaned by HIV/AIDS'</span>
<span class="st">            order by YR2010, YR2000 limit 20&quot;</span>)
<span class="kw">head</span>(sq)</code></pre></div>
<pre><code>##      Lat_Long Country_Name YR2000 YR2010
## 1     -10:-76         Peru  61000  54000
## 2       -1:15  Congo, Rep.  52000  70000
## 3     23:-102       Mexico  66000  71000
## 4       17:-4         Mali  51000  91000
## 5   2.5:112.5     Malaysia  51000  96000
## 6 19:-72.4167        Haiti 110000 100000</code></pre>
<ul>
<li>The world map showing the countries where children are orphaned by HIV?AIDS (2000, 2010)</li>
</ul>
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r">Show_map &lt;-<span class="st"> </span><span class="kw">gvisMap</span>(sq, <span class="st">&quot;Lat_Long&quot;</span> , <span class="st">&quot;Country_Name&quot;</span>,
              <span class="dt">options=</span><span class="kw">list</span>(<span class="dt">showTip=</span><span class="ot">TRUE</span>, <span class="dt">mapType=</span><span class="st">'normal'</span>,
              <span class="dt">enableScrollWheel=</span><span class="ot">TRUE</span>,
              <span class="dt">icons=</span><span class="kw">paste0</span>(<span class="st">&quot;{&quot;</span>,
              <span class="st">&quot;'default': {'normal': 'http://icons.iconarchive.com/&quot;</span>,
              <span class="st">&quot;icons/icons-land/vista-map-markers/48/&quot;</span>,
              <span class="st">&quot;Map-Marker-Ball-Azure-icon.png',</span><span class="ch">\n</span><span class="st">&quot;</span>,
              <span class="st">&quot;'selected': 'http://icons.iconarchive.com/&quot;</span>,
              <span class="st">&quot;icons/icons-land/vista-map-markers/48/&quot;</span>,
              <span class="st">&quot;Map-Marker-Ball-Right-Azure-icon.png'&quot;</span>,
              <span class="st">&quot;}}&quot;</span>)))
<span class="kw">print</span>(Show_map, <span class="dt">file=</span><span class="st">&quot;gvis1.html&quot;</span>)                        
<span class="kw">plot</span>(Show_map)</code></pre></div>
<pre><code>## starting httpd help server ... done</code></pre>
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r"><span class="kw">browseURL</span>(<span class="st">&quot;gvis1.html&quot;</span>)</code></pre></div>
<div class="sourceCode"><pre class="sourceCode r"><code class="sourceCode r">g &lt;-<span class="st"> </span><span class="kw">ggplot</span>(sq, <span class="kw">aes</span>(YR2010, YR2000)) +
<span class="st">  </span><span class="kw">geom_line</span>(<span class="kw">aes</span>(<span class="dt">colour =</span> Country_Name)) +
<span class="st">  </span><span class="kw">labs</span>(<span class="dt">title =</span> <span class="st">&quot;Top 20 Countries Where Children Orphaned by HIV/AIDS For YRS 2000 &amp; 2010 &quot;</span>) +
<span class="st">  </span><span class="kw">geom_smooth</span>(<span class="dt">se =</span> <span class="ot">TRUE</span>)

<span class="kw">ggplotly</span>(g)</code></pre></div>
<pre><code>## `geom_smooth()` using method = 'loess' and formula 'y ~ x'</code></pre>
<div id="421c62a46c6e" style="width:864px;height:864px;" class="plotly html-widget"></div>
<script type="application/json" data-for="421c62a46c6e">{"x":{"data":[{"x":[110000],"y":[82000],"text":"Country_Name: Botswana<br />YR2010:  110000<br />YR2000:  82000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(248,118,109,1)","dash":"solid"},"hoveron":"points","name":"Botswana","legendgroup":"Botswana","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[130000],"y":[170000],"text":"Country_Name: Brazil<br />YR2010:  130000<br />YR2000: 170000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(234,131,49,1)","dash":"solid"},"hoveron":"points","name":"Brazil","legendgroup":"Brazil","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[130000],"y":[120000],"text":"Country_Name: Burkina Faso<br />YR2010:  130000<br />YR2000: 120000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(216,144,0,1)","dash":"solid"},"hoveron":"points","name":"Burkina Faso","legendgroup":"Burkina Faso","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[290000],"y":[87000],"text":"Country_Name: Cameroon<br />YR2010:  290000<br />YR2000:  87000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(192,155,0,1)","dash":"solid"},"hoveron":"points","name":"Cameroon","legendgroup":"Cameroon","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[130000],"y":[68000],"text":"Country_Name: Central African Republic<br />YR2010:  130000<br />YR2000:  68000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(163,165,0,1)","dash":"solid"},"hoveron":"points","name":"Central African Republic","legendgroup":"Central African Republic","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[630000],"y":[430000],"text":"Country_Name: Congo, Dem. Rep.<br />YR2010:  630000<br />YR2000: 430000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(124,174,0,1)","dash":"solid"},"hoveron":"points","name":"Congo, Dem. Rep.","legendgroup":"Congo, Dem. Rep.","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[70000],"y":[52000],"text":"Country_Name: Congo, Rep.<br />YR2010:   70000<br />YR2000:  52000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(57,182,0,1)","dash":"solid"},"hoveron":"points","name":"Congo, Rep.","legendgroup":"Congo, Rep.","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[370000],"y":[250000],"text":"Country_Name: Cote d'Ivoire<br />YR2010:  370000<br />YR2000: 250000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(0,187,78,1)","dash":"solid"},"hoveron":"points","name":"Cote d'Ivoire","legendgroup":"Cote d'Ivoire","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[870000],"y":[490000],"text":"Country_Name: Ethiopia<br />YR2010:  870000<br />YR2000: 490000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(0,191,125,1)","dash":"solid"},"hoveron":"points","name":"Ethiopia","legendgroup":"Ethiopia","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[360000],"y":[190000],"text":"Country_Name: Ghana<br />YR2010:  360000<br />YR2000: 190000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(0,193,163,1)","dash":"solid"},"hoveron":"points","name":"Ghana","legendgroup":"Ghana","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[100000],"y":[110000],"text":"Country_Name: Haiti<br />YR2010:  100000<br />YR2000: 110000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(0,191,196,1)","dash":"solid"},"hoveron":"points","name":"Haiti","legendgroup":"Haiti","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[910000],"y":[550000],"text":"Country_Name: Malawi<br />YR2010:  910000<br />YR2000: 550000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(0,186,224,1)","dash":"solid"},"hoveron":"points","name":"Malawi","legendgroup":"Malawi","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[96000],"y":[51000],"text":"Country_Name: Malaysia<br />YR2010:   96000<br />YR2000:  51000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(0,176,246,1)","dash":"solid"},"hoveron":"points","name":"Malaysia","legendgroup":"Malaysia","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[91000],"y":[51000],"text":"Country_Name: Mali<br />YR2010:   91000<br />YR2000:  51000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(53,162,255,1)","dash":"solid"},"hoveron":"points","name":"Mali","legendgroup":"Mali","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[71000],"y":[66000],"text":"Country_Name: Mexico<br />YR2010:   71000<br />YR2000:  66000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(149,144,255,1)","dash":"solid"},"hoveron":"points","name":"Mexico","legendgroup":"Mexico","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[1000000],"y":[260000],"text":"Country_Name: Mozambique<br />YR2010: 1000000<br />YR2000: 260000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(199,124,255,1)","dash":"solid"},"hoveron":"points","name":"Mozambique","legendgroup":"Mozambique","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[54000],"y":[61000],"text":"Country_Name: Peru<br />YR2010:   54000<br />YR2000:  61000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(231,107,243,1)","dash":"solid"},"hoveron":"points","name":"Peru","legendgroup":"Peru","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[130000],"y":[70000],"text":"Country_Name: Rwanda<br />YR2010:  130000<br />YR2000:  70000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(250,98,219,1)","dash":"solid"},"hoveron":"points","name":"Rwanda","legendgroup":"Rwanda","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[300000],"y":[170000],"text":"Country_Name: Thailand<br />YR2010:  300000<br />YR2000: 170000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(255,98,188,1)","dash":"solid"},"hoveron":"points","name":"Thailand","legendgroup":"Thailand","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[670000],"y":[400000],"text":"Country_Name: Zambia<br />YR2010:  670000<br />YR2000: 400000","type":"scatter","mode":"lines","line":{"width":1.88976377952756,"color":"rgba(255,106,152,1)","dash":"solid"},"hoveron":"points","name":"Zambia","legendgroup":"Zambia","showlegend":true,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[54000,65974.6835443038,77949.3670886076,89924.0506329114,101898.734177215,113873.417721519,125848.101265823,137822.784810127,149797.46835443,161772.151898734,173746.835443038,185721.518987342,197696.202531646,209670.886075949,221645.569620253,233620.253164557,245594.936708861,257569.620253165,269544.303797468,281518.987341772,293493.670886076,305468.35443038,317443.037974684,329417.721518987,341392.405063291,353367.088607595,365341.772151899,377316.455696203,389291.139240506,401265.82278481,413240.506329114,425215.189873418,437189.873417722,449164.556962025,461139.240506329,473113.924050633,485088.607594937,497063.291139241,509037.974683544,521012.658227848,532987.341772152,544962.025316456,556936.70886076,568911.392405063,580886.075949367,592860.759493671,604835.443037975,616810.126582279,628784.810126582,640759.493670886,652734.17721519,664708.860759494,676683.544303798,688658.227848101,700632.911392405,712607.594936709,724582.278481013,736556.962025316,748531.64556962,760506.329113924,772481.012658228,784455.696202532,796430.379746835,808405.063291139,820379.746835443,832354.430379747,844329.113924051,856303.797468354,868278.481012658,880253.164556962,892227.848101266,904202.53164557,916177.215189873,928151.898734177,940126.582278481,952101.265822785,964075.949367089,976050.632911392,988025.316455696,1000000],"y":[45840.0892240449,56341.1915644422,66181.6224528322,75352.7935874278,83850.7657716175,91674.7041990587,98833.8462255915,105229.843127999,110571.008178909,114991.213949256,118658.455767356,121740.728961528,124406.028860089,126822.350791358,129157.690083651,131580.042065288,134257.402064585,137357.765409861,141049.127429432,145499.483451618,150876.828804736,157349.158817103,165084.468817038,174250.754132859,185016.010092882,197548.232025426,211764.291229061,225890.135011262,239552.901008377,252758.637082457,265513.391095554,277823.21090972,289694.144387006,301132.239389463,312143.543779143,322734.105418098,332909.972168378,342677.191892036,352041.812451123,361009.88170769,369587.447523789,377780.557761471,385595.260282788,393037.602949792,400113.633624533,406829.400169064,413190.950445435,419204.332315699,424875.593641907,430251.788366923,435376.583405447,440219.267221192,444748.541115999,448933.106391707,452741.664350157,456142.916293188,459105.56352264,461598.307340355,463589.849048171,465048.889947929,465944.13134147,466244.274530632,465918.020817257,464934.071503184,463261.127890254,460867.891280306,457723.062975182,453795.34427672,449053.436486761,443570.171406674,437509.665006288,430875.508911631,423668.469677452,415889.313858502,407538.808009531,398617.71868529,389126.812440529,379066.855829999,368438.61540845,357242.857730632],"text":["YR2010:   54000.00<br />YR2000:  45840.09","YR2010:   65974.68<br />YR2000:  56341.19","YR2010:   77949.37<br />YR2000:  66181.62","YR2010:   89924.05<br />YR2000:  75352.79","YR2010:  101898.73<br />YR2000:  83850.77","YR2010:  113873.42<br />YR2000:  91674.70","YR2010:  125848.10<br />YR2000:  98833.85","YR2010:  137822.78<br />YR2000: 105229.84","YR2010:  149797.47<br />YR2000: 110571.01","YR2010:  161772.15<br />YR2000: 114991.21","YR2010:  173746.84<br />YR2000: 118658.46","YR2010:  185721.52<br />YR2000: 121740.73","YR2010:  197696.20<br />YR2000: 124406.03","YR2010:  209670.89<br />YR2000: 126822.35","YR2010:  221645.57<br />YR2000: 129157.69","YR2010:  233620.25<br />YR2000: 131580.04","YR2010:  245594.94<br />YR2000: 134257.40","YR2010:  257569.62<br />YR2000: 137357.77","YR2010:  269544.30<br />YR2000: 141049.13","YR2010:  281518.99<br />YR2000: 145499.48","YR2010:  293493.67<br />YR2000: 150876.83","YR2010:  305468.35<br />YR2000: 157349.16","YR2010:  317443.04<br />YR2000: 165084.47","YR2010:  329417.72<br />YR2000: 174250.75","YR2010:  341392.41<br />YR2000: 185016.01","YR2010:  353367.09<br />YR2000: 197548.23","YR2010:  365341.77<br />YR2000: 211764.29","YR2010:  377316.46<br />YR2000: 225890.14","YR2010:  389291.14<br />YR2000: 239552.90","YR2010:  401265.82<br />YR2000: 252758.64","YR2010:  413240.51<br />YR2000: 265513.39","YR2010:  425215.19<br />YR2000: 277823.21","YR2010:  437189.87<br />YR2000: 289694.14","YR2010:  449164.56<br />YR2000: 301132.24","YR2010:  461139.24<br />YR2000: 312143.54","YR2010:  473113.92<br />YR2000: 322734.11","YR2010:  485088.61<br />YR2000: 332909.97","YR2010:  497063.29<br />YR2000: 342677.19","YR2010:  509037.97<br />YR2000: 352041.81","YR2010:  521012.66<br />YR2000: 361009.88","YR2010:  532987.34<br />YR2000: 369587.45","YR2010:  544962.03<br />YR2000: 377780.56","YR2010:  556936.71<br />YR2000: 385595.26","YR2010:  568911.39<br />YR2000: 393037.60","YR2010:  580886.08<br />YR2000: 400113.63","YR2010:  592860.76<br />YR2000: 406829.40","YR2010:  604835.44<br />YR2000: 413190.95","YR2010:  616810.13<br />YR2000: 419204.33","YR2010:  628784.81<br />YR2000: 424875.59","YR2010:  640759.49<br />YR2000: 430251.79","YR2010:  652734.18<br />YR2000: 435376.58","YR2010:  664708.86<br />YR2000: 440219.27","YR2010:  676683.54<br />YR2000: 444748.54","YR2010:  688658.23<br />YR2000: 448933.11","YR2010:  700632.91<br />YR2000: 452741.66","YR2010:  712607.59<br />YR2000: 456142.92","YR2010:  724582.28<br />YR2000: 459105.56","YR2010:  736556.96<br />YR2000: 461598.31","YR2010:  748531.65<br />YR2000: 463589.85","YR2010:  760506.33<br />YR2000: 465048.89","YR2010:  772481.01<br />YR2000: 465944.13","YR2010:  784455.70<br />YR2000: 466244.27","YR2010:  796430.38<br />YR2000: 465918.02","YR2010:  808405.06<br />YR2000: 464934.07","YR2010:  820379.75<br />YR2000: 463261.13","YR2010:  832354.43<br />YR2000: 460867.89","YR2010:  844329.11<br />YR2000: 457723.06","YR2010:  856303.80<br />YR2000: 453795.34","YR2010:  868278.48<br />YR2000: 449053.44","YR2010:  880253.16<br />YR2000: 443570.17","YR2010:  892227.85<br />YR2000: 437509.67","YR2010:  904202.53<br />YR2000: 430875.51","YR2010:  916177.22<br />YR2000: 423668.47","YR2010:  928151.90<br />YR2000: 415889.31","YR2010:  940126.58<br />YR2000: 407538.81","YR2010:  952101.27<br />YR2000: 398617.72","YR2010:  964075.95<br />YR2000: 389126.81","YR2010:  976050.63<br />YR2000: 379066.86","YR2010:  988025.32<br />YR2000: 368438.62","YR2010: 1000000.00<br />YR2000: 357242.86"],"type":"scatter","mode":"lines","name":"fitted values","line":{"width":3.77952755905512,"color":"rgba(51,102,255,1)","dash":"solid"},"hoveron":"points","showlegend":false,"xaxis":"x","yaxis":"y","hoverinfo":"text","frame":null},{"x":[54000,65974.6835443038,77949.3670886076,89924.0506329114,101898.734177215,113873.417721519,125848.101265823,137822.784810127,149797.46835443,161772.151898734,173746.835443038,185721.518987342,197696.202531646,209670.886075949,221645.569620253,233620.253164557,245594.936708861,257569.620253165,269544.303797468,281518.987341772,293493.670886076,305468.35443038,317443.037974684,329417.721518987,341392.405063291,353367.088607595,365341.772151899,377316.455696203,389291.139240506,401265.82278481,413240.506329114,425215.189873418,437189.873417722,449164.556962025,461139.240506329,473113.924050633,485088.607594937,497063.291139241,509037.974683544,521012.658227848,532987.341772152,544962.025316456,556936.70886076,568911.392405063,580886.075949367,592860.759493671,604835.443037975,616810.126582279,628784.810126582,640759.493670886,652734.17721519,664708.860759494,676683.544303798,688658.227848101,700632.911392405,712607.594936709,724582.278481013,736556.962025316,748531.64556962,760506.329113924,772481.012658228,784455.696202532,796430.379746835,808405.063291139,820379.746835443,832354.430379747,844329.113924051,856303.797468354,868278.481012658,880253.164556962,892227.848101266,904202.53164557,916177.215189873,928151.898734177,940126.582278481,952101.265822785,964075.949367089,976050.632911392,988025.316455696,1000000,1000000,1000000,988025.316455696,976050.632911392,964075.949367089,952101.265822785,940126.582278481,928151.898734177,916177.215189873,904202.53164557,892227.848101266,880253.164556962,868278.481012658,856303.797468354,844329.113924051,832354.430379747,820379.746835443,808405.063291139,796430.379746835,784455.696202532,772481.012658228,760506.329113924,748531.64556962,736556.962025316,724582.278481013,712607.594936709,700632.911392405,688658.227848101,676683.544303798,664708.860759494,652734.17721519,640759.493670886,628784.810126582,616810.126582279,604835.443037975,592860.759493671,580886.075949367,568911.392405063,556936.70886076,544962.025316456,532987.341772152,521012.658227848,509037.974683544,497063.291139241,485088.607594937,473113.924050633,461139.240506329,449164.556962025,437189.873417722,425215.189873418,413240.506329114,401265.82278481,389291.139240506,377316.455696203,365341.772151899,353367.088607595,341392.405063291,329417.721518987,317443.037974684,305468.35443038,293493.670886076,281518.987341772,269544.303797468,257569.620253165,245594.936708861,233620.253164557,221645.569620253,209670.886075949,197696.202531646,185721.518987342,173746.835443038,161772.151898734,149797.46835443,137822.784810127,125848.101265823,113873.417721519,101898.734177215,89924.0506329114,77949.3670886076,65974.6835443038,54000,54000],"y":[-33286.0640447155,-4164.03784523915,19987.4949230153,37434.2852505911,47004.0523915084,50400.0884309582,50746.8109064757,50185.6744758026,49900.3449325382,50310.159357077,51521.3147340384,53511.7470196874,56200.4740173505,59480.3364481576,63238.1486492295,67371.6707690225,71806.9124148526,76515.4427650727,81527.7814184793,86936.1767495773,92879.9152701149,99509.574785132,106931.893706791,115142.596954709,123962.484623567,133005.412885348,141673.784219073,149728.594806244,158000.845818618,166956.242170462,176758.715444036,187409.304373022,198816.704035971,210833.507345099,223275.704396274,235934.308576591,248584.024331956,260992.200625641,272930.523775506,284191.024269955,294606.226409125,304070.434008152,312556.278856581,320120.043989022,326892.444397901,333056.928950509,338821.290543304,344388.039203727,349925.569428647,355475.234958995,360944.206058238,366291.562078236,371476.050377837,376455.446843908,381186.509779216,385624.845022067,389724.6765343,393438.513837232,396716.706150085,399506.873844899,401753.212547506,403395.676524226,404369.069623734,404602.108431499,404016.5770068,402526.764459328,400039.452949236,396454.771723201,391668.1968797,385672.445030582,378557.255369566,370277.965748436,360804.600123638,350125.173926847,338243.926769008,325177.857596802,310952.5956048,295598.506517017,279147.566676082,261631.167925948,261631.167925948,452854.547535316,457729.664140817,462535.205142981,467301.029276259,472057.579773779,476833.689250054,481653.453790157,486532.339231266,491473.052074825,496462.07464301,501467.897782766,506438.676093822,511135.916830238,515406.673001127,519209.018101285,522505.678773708,525266.03457487,527466.97201078,529092.872537038,530135.050135433,530590.906050959,530462.991946257,529758.100843478,528486.45051098,526660.987564308,524296.818921097,521410.765939506,518021.031854161,514146.972364149,509808.960752656,505028.34177485,499825.617855166,494020.625427671,487560.610347567,480601.871387618,473334.822851165,465955.161910561,458634.241708995,451490.68151479,444568.668638452,437828.739145425,431153.101126739,424362.18315843,417235.9200048,409533.902259604,401011.383162012,391430.971433827,380571.58473804,368237.117446418,354268.066747073,338561.031994452,321104.956198136,302051.675216279,281854.798239049,262091.051165504,246069.535562196,233358.911311008,223237.043927286,215188.742849075,208873.742339357,204062.790153659,200570.473440386,198200.088054648,196707.891714317,195788.413361553,195077.231518073,194164.365134558,192611.583702828,189969.710903369,185795.596800674,179672.268541435,171241.671425281,160274.011780195,146920.881544707,132949.319967159,120697.479151727,113271.301924265,112375.749982649,116846.420974124,124966.242492805,-33286.0640447155],"text":["YR2010:   54000.00<br />YR2000:  45840.09","YR2010:   65974.68<br />YR2000:  56341.19","YR2010:   77949.37<br />YR2000:  66181.62","YR2010:   89924.05<br />YR2000:  75352.79","YR2010:  101898.73<br />YR2000:  83850.77","YR2010:  113873.42<br />YR2000:  91674.70","YR2010:  125848.10<br />YR2000:  98833.85","YR2010:  137822.78<br />YR2000: 105229.84","YR2010:  149797.47<br />YR2000: 110571.01","YR2010:  161772.15<br />YR2000: 114991.21","YR2010:  173746.84<br />YR2000: 118658.46","YR2010:  185721.52<br />YR2000: 121740.73","YR2010:  197696.20<br />YR2000: 124406.03","YR2010:  209670.89<br />YR2000: 126822.35","YR2010:  221645.57<br />YR2000: 129157.69","YR2010:  233620.25<br />YR2000: 131580.04","YR2010:  245594.94<br />YR2000: 134257.40","YR2010:  257569.62<br />YR2000: 137357.77","YR2010:  269544.30<br />YR2000: 141049.13","YR2010:  281518.99<br />YR2000: 145499.48","YR2010:  293493.67<br />YR2000: 150876.83","YR2010:  305468.35<br />YR2000: 157349.16","YR2010:  317443.04<br />YR2000: 165084.47","YR2010:  329417.72<br />YR2000: 174250.75","YR2010:  341392.41<br />YR2000: 185016.01","YR2010:  353367.09<br />YR2000: 197548.23","YR2010:  365341.77<br />YR2000: 211764.29","YR2010:  377316.46<br />YR2000: 225890.14","YR2010:  389291.14<br />YR2000: 239552.90","YR2010:  401265.82<br />YR2000: 252758.64","YR2010:  413240.51<br />YR2000: 265513.39","YR2010:  425215.19<br />YR2000: 277823.21","YR2010:  437189.87<br />YR2000: 289694.14","YR2010:  449164.56<br />YR2000: 301132.24","YR2010:  461139.24<br />YR2000: 312143.54","YR2010:  473113.92<br />YR2000: 322734.11","YR2010:  485088.61<br />YR2000: 332909.97","YR2010:  497063.29<br />YR2000: 342677.19","YR2010:  509037.97<br />YR2000: 352041.81","YR2010:  521012.66<br />YR2000: 361009.88","YR2010:  532987.34<br />YR2000: 369587.45","YR2010:  544962.03<br />YR2000: 377780.56","YR2010:  556936.71<br />YR2000: 385595.26","YR2010:  568911.39<br />YR2000: 393037.60","YR2010:  580886.08<br />YR2000: 400113.63","YR2010:  592860.76<br />YR2000: 406829.40","YR2010:  604835.44<br />YR2000: 413190.95","YR2010:  616810.13<br />YR2000: 419204.33","YR2010:  628784.81<br />YR2000: 424875.59","YR2010:  640759.49<br />YR2000: 430251.79","YR2010:  652734.18<br />YR2000: 435376.58","YR2010:  664708.86<br />YR2000: 440219.27","YR2010:  676683.54<br />YR2000: 444748.54","YR2010:  688658.23<br />YR2000: 448933.11","YR2010:  700632.91<br />YR2000: 452741.66","YR2010:  712607.59<br />YR2000: 456142.92","YR2010:  724582.28<br />YR2000: 459105.56","YR2010:  736556.96<br />YR2000: 461598.31","YR2010:  748531.65<br />YR2000: 463589.85","YR2010:  760506.33<br />YR2000: 465048.89","YR2010:  772481.01<br />YR2000: 465944.13","YR2010:  784455.70<br />YR2000: 466244.27","YR2010:  796430.38<br />YR2000: 465918.02","YR2010:  808405.06<br />YR2000: 464934.07","YR2010:  820379.75<br />YR2000: 463261.13","YR2010:  832354.43<br />YR2000: 460867.89","YR2010:  844329.11<br />YR2000: 457723.06","YR2010:  856303.80<br />YR2000: 453795.34","YR2010:  868278.48<br />YR2000: 449053.44","YR2010:  880253.16<br />YR2000: 443570.17","YR2010:  892227.85<br />YR2000: 437509.67","YR2010:  904202.53<br />YR2000: 430875.51","YR2010:  916177.22<br />YR2000: 423668.47","YR2010:  928151.90<br />YR2000: 415889.31","YR2010:  940126.58<br />YR2000: 407538.81","YR2010:  952101.27<br />YR2000: 398617.72","YR2010:  964075.95<br />YR2000: 389126.81","YR2010:  976050.63<br />YR2000: 379066.86","YR2010:  988025.32<br />YR2000: 368438.62","YR2010: 1000000.00<br />YR2000: 357242.86","YR2010: 1000000.00<br />YR2000: 357242.86","YR2010: 1000000.00<br />YR2000: 357242.86","YR2010:  988025.32<br />YR2000: 368438.62","YR2010:  976050.63<br />YR2000: 379066.86","YR2010:  964075.95<br />YR2000: 389126.81","YR2010:  952101.27<br />YR2000: 398617.72","YR2010:  940126.58<br />YR2000: 407538.81","YR2010:  928151.90<br />YR2000: 415889.31","YR2010:  916177.22<br />YR2000: 423668.47","YR2010:  904202.53<br />YR2000: 430875.51","YR2010:  892227.85<br />YR2000: 437509.67","YR2010:  880253.16<br />YR2000: 443570.17","YR2010:  868278.48<br />YR2000: 449053.44","YR2010:  856303.80<br />YR2000: 453795.34","YR2010:  844329.11<br />YR2000: 457723.06","YR2010:  832354.43<br />YR2000: 460867.89","YR2010:  820379.75<br />YR2000: 463261.13","YR2010:  808405.06<br />YR2000: 464934.07","YR2010:  796430.38<br />YR2000: 465918.02","YR2010:  784455.70<br />YR2000: 466244.27","YR2010:  772481.01<br />YR2000: 465944.13","YR2010:  760506.33<br />YR2000: 465048.89","YR2010:  748531.65<br />YR2000: 463589.85","YR2010:  736556.96<br />YR2000: 461598.31","YR2010:  724582.28<br />YR2000: 459105.56","YR2010:  712607.59<br />YR2000: 456142.92","YR2010:  700632.91<br />YR2000: 452741.66","YR2010:  688658.23<br />YR2000: 448933.11","YR2010:  676683.54<br />YR2000: 444748.54","YR2010:  664708.86<br />YR2000: 440219.27","YR2010:  652734.18<br />YR2000: 435376.58","YR2010:  640759.49<br />YR2000: 430251.79","YR2010:  628784.81<br />YR2000: 424875.59","YR2010:  616810.13<br />YR2000: 419204.33","YR2010:  604835.44<br />YR2000: 413190.95","YR2010:  592860.76<br />YR2000: 406829.40","YR2010:  580886.08<br />YR2000: 400113.63","YR2010:  568911.39<br />YR2000: 393037.60","YR2010:  556936.71<br />YR2000: 385595.26","YR2010:  544962.03<br />YR2000: 377780.56","YR2010:  532987.34<br />YR2000: 369587.45","YR2010:  521012.66<br />YR2000: 361009.88","YR2010:  509037.97<br />YR2000: 352041.81","YR2010:  497063.29<br />YR2000: 342677.19","YR2010:  485088.61<br />YR2000: 332909.97","YR2010:  473113.92<br />YR2000: 322734.11","YR2010:  461139.24<br />YR2000: 312143.54","YR2010:  449164.56<br />YR2000: 301132.24","YR2010:  437189.87<br />YR2000: 289694.14","YR2010:  425215.19<br />YR2000: 277823.21","YR2010:  413240.51<br />YR2000: 265513.39","YR2010:  401265.82<br />YR2000: 252758.64","YR2010:  389291.14<br />YR2000: 239552.90","YR2010:  377316.46<br />YR2000: 225890.14","YR2010:  365341.77<br />YR2000: 211764.29","YR2010:  353367.09<br />YR2000: 197548.23","YR2010:  341392.41<br />YR2000: 185016.01","YR2010:  329417.72<br />YR2000: 174250.75","YR2010:  317443.04<br />YR2000: 165084.47","YR2010:  305468.35<br />YR2000: 157349.16","YR2010:  293493.67<br />YR2000: 150876.83","YR2010:  281518.99<br />YR2000: 145499.48","YR2010:  269544.30<br />YR2000: 141049.13","YR2010:  257569.62<br />YR2000: 137357.77","YR2010:  245594.94<br />YR2000: 134257.40","YR2010:  233620.25<br />YR2000: 131580.04","YR2010:  221645.57<br />YR2000: 129157.69","YR2010:  209670.89<br />YR2000: 126822.35","YR2010:  197696.20<br />YR2000: 124406.03","YR2010:  185721.52<br />YR2000: 121740.73","YR2010:  173746.84<br />YR2000: 118658.46","YR2010:  161772.15<br />YR2000: 114991.21","YR2010:  149797.47<br />YR2000: 110571.01","YR2010:  137822.78<br />YR2000: 105229.84","YR2010:  125848.10<br />YR2000:  98833.85","YR2010:  113873.42<br />YR2000:  91674.70","YR2010:  101898.73<br />YR2000:  83850.77","YR2010:   89924.05<br />YR2000:  75352.79","YR2010:   77949.37<br />YR2000:  66181.62","YR2010:   65974.68<br />YR2000:  56341.19","YR2010:   54000.00<br />YR2000:  45840.09","YR2010:   54000.00<br />YR2000:  45840.09"],"type":"scatter","mode":"lines","line":{"width":3.77952755905512,"color":"transparent","dash":"solid"},"fill":"toself","fillcolor":"rgba(153,153,153,0.4)","hoveron":"points","hoverinfo":"x+y","showlegend":false,"xaxis":"x","yaxis":"y","frame":null}],"layout":{"margin":{"t":40.8401826484018,"r":7.30593607305936,"b":37.2602739726027,"l":54.7945205479452},"plot_bgcolor":"rgba(235,235,235,1)","paper_bgcolor":"rgba(255,255,255,1)","font":{"color":"rgba(0,0,0,1)","family":"","size":14.6118721461187},"title":"Top 20 Countries Where Children Orphaned by HIV/AIDS For YRS 2000 & 2010 ","titlefont":{"color":"rgba(0,0,0,1)","family":"","size":17.5342465753425},"xaxis":{"domain":[0,1],"type":"linear","autorange":false,"range":[6700,1047300],"tickmode":"array","ticktext":["250000","500000","750000","1000000"],"tickvals":[250000,500000,750000,1000000],"categoryorder":"array","categoryarray":["250000","500000","750000","1000000"],"nticks":null,"ticks":"outside","tickcolor":"rgba(51,51,51,1)","ticklen":3.65296803652968,"tickwidth":0.66417600664176,"showticklabels":true,"tickfont":{"color":"rgba(77,77,77,1)","family":"","size":11.689497716895},"tickangle":-0,"showline":false,"linecolor":null,"linewidth":0,"showgrid":true,"gridcolor":"rgba(255,255,255,1)","gridwidth":0.66417600664176,"zeroline":false,"anchor":"y","title":"YR2010","titlefont":{"color":"rgba(0,0,0,1)","family":"","size":14.6118721461187},"hoverformat":".2f"},"yaxis":{"domain":[0,1],"type":"linear","autorange":false,"range":[-62450.3672469513,579164.303202236],"tickmode":"array","ticktext":["0e+00","2e+05","4e+05"],"tickvals":[0,200000,400000],"categoryorder":"array","categoryarray":["0e+00","2e+05","4e+05"],"nticks":null,"ticks":"outside","tickcolor":"rgba(51,51,51,1)","ticklen":3.65296803652968,"tickwidth":0.66417600664176,"showticklabels":true,"tickfont":{"color":"rgba(77,77,77,1)","family":"","size":11.689497716895},"tickangle":-0,"showline":false,"linecolor":null,"linewidth":0,"showgrid":true,"gridcolor":"rgba(255,255,255,1)","gridwidth":0.66417600664176,"zeroline":false,"anchor":"x","title":"YR2000","titlefont":{"color":"rgba(0,0,0,1)","family":"","size":14.6118721461187},"hoverformat":".2f"},"shapes":[{"type":"rect","fillcolor":null,"line":{"color":null,"width":0,"linetype":[]},"yref":"paper","xref":"paper","x0":0,"x1":1,"y0":0,"y1":1}],"showlegend":true,"legend":{"bgcolor":"rgba(255,255,255,1)","bordercolor":"transparent","borderwidth":1.88976377952756,"font":{"color":"rgba(0,0,0,1)","family":"","size":11.689497716895},"y":0.951881014873141},"annotations":[{"text":"Country_Name","x":1.02,"y":1,"showarrow":false,"ax":0,"ay":0,"font":{"color":"rgba(0,0,0,1)","family":"","size":14.6118721461187},"xref":"paper","yref":"paper","textangle":-0,"xanchor":"left","yanchor":"bottom","legendTitle":true}],"hovermode":"closest","barmode":"relative"},"config":{"doubleClick":"reset","modeBarButtonsToAdd":[{"name":"Collaborate","icon":{"width":1000,"ascent":500,"descent":-50,"path":"M487 375c7-10 9-23 5-36l-79-259c-3-12-11-23-22-31-11-8-22-12-35-12l-263 0c-15 0-29 5-43 15-13 10-23 23-28 37-5 13-5 25-1 37 0 0 0 3 1 7 1 5 1 8 1 11 0 2 0 4-1 6 0 3-1 5-1 6 1 2 2 4 3 6 1 2 2 4 4 6 2 3 4 5 5 7 5 7 9 16 13 26 4 10 7 19 9 26 0 2 0 5 0 9-1 4-1 6 0 8 0 2 2 5 4 8 3 3 5 5 5 7 4 6 8 15 12 26 4 11 7 19 7 26 1 1 0 4 0 9-1 4-1 7 0 8 1 2 3 5 6 8 4 4 6 6 6 7 4 5 8 13 13 24 4 11 7 20 7 28 1 1 0 4 0 7-1 3-1 6-1 7 0 2 1 4 3 6 1 1 3 4 5 6 2 3 3 5 5 6 1 2 3 5 4 9 2 3 3 7 5 10 1 3 2 6 4 10 2 4 4 7 6 9 2 3 4 5 7 7 3 2 7 3 11 3 3 0 8 0 13-1l0-1c7 2 12 2 14 2l218 0c14 0 25-5 32-16 8-10 10-23 6-37l-79-259c-7-22-13-37-20-43-7-7-19-10-37-10l-248 0c-5 0-9-2-11-5-2-3-2-7 0-12 4-13 18-20 41-20l264 0c5 0 10 2 16 5 5 3 8 6 10 11l85 282c2 5 2 10 2 17 7-3 13-7 17-13z m-304 0c-1-3-1-5 0-7 1-1 3-2 6-2l174 0c2 0 4 1 7 2 2 2 4 4 5 7l6 18c0 3 0 5-1 7-1 1-3 2-6 2l-173 0c-3 0-5-1-8-2-2-2-4-4-4-7z m-24-73c-1-3-1-5 0-7 2-2 3-2 6-2l174 0c2 0 5 0 7 2 3 2 4 4 5 7l6 18c1 2 0 5-1 6-1 2-3 3-5 3l-174 0c-3 0-5-1-7-3-3-1-4-4-5-6z"},"click":"function(gd) { \n        // is this being viewed in RStudio?\n        if (location.search == '?viewer_pane=1') {\n          alert('To learn about plotly for collaboration, visit:\\n https://cpsievert.github.io/plotly_book/plot-ly-for-collaboration.html');\n        } else {\n          window.open('https://cpsievert.github.io/plotly_book/plot-ly-for-collaboration.html', '_blank');\n        }\n      }"}],"cloud":false},"source":"A","attrs":{"421c24eeafa":{"colour":{},"x":{},"y":{},"type":"scatter"},"421c370e7588":{"x":{},"y":{}}},"cur_data":"421c24eeafa","visdat":{"421c24eeafa":["function (y) ","x"],"421c370e7588":["function (y) ","x"]},"highlight":{"on":"plotly_click","persistent":false,"dynamic":false,"selectize":false,"opacityDim":0.2,"selected":{"opacity":1}},"base_url":"https://plot.ly"},"evals":["config.modeBarButtonsToAdd.0.click"],"jsHooks":{"render":[{"code":"function(el, x) { var ctConfig = crosstalk.var('plotlyCrosstalkOpts').set({\"on\":\"plotly_click\",\"persistent\":false,\"dynamic\":false,\"selectize\":false,\"opacityDim\":0.2,\"selected\":{\"opacity\":1}}); }","data":null}]}}</script>
</div>
<div id="tools-to-be-used" class="section level2">
<h2>Tools To Be Used:</h2>
<ul>
<li>GoogleVis</li>
<li>Plotly</li>
<li>GGplot2</li>
<li>Sqldf</li>
</ul>
</div>
<div id="packages-to-be-used" class="section level2">
<h2>Packages To Be Used:</h2>
<ul>
<li>Plotly</li>
<li>Knitr</li>
<li>Dplyr</li>
<li>Plyr</li>
<li>Reshape2</li>
<li>Ggplot2</li>
<li>Graphics</li>
<li>Ggthemes</li>
<li>GoogleVis</li>
</ul>
<p>etc</p>
</div>



</div>
</div>

</div>

<script>

// add bootstrap table styles to pandoc tables
function bootstrapStylePandocTables() {
  $('tr.header').parent('thead').parent('table').addClass('table table-condensed');
}
$(document).ready(function () {
  bootstrapStylePandocTables();
});


</script>

<!-- dynamically load mathjax for compatibility with self-contained -->
<script>
  (function () {
    var script = document.createElement("script");
    script.type = "text/javascript";
    script.src  = "https://mathjax.rstudio.com/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML";
    document.getElementsByTagName("head")[0].appendChild(script);
  })();
</script>

</body>
</html>

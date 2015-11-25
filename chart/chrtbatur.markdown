<head>
  <link rel="stylesheet" href="bower_components/angular-chart.js/dist/angular-chart.css" />
<head>
<body>


  <canvas id="bar" class="chart chart-bar"
  chart-data="data" chart-labels="labels">
</canvas
<code class="rainbow" data-language="javascript">angular.<span class="function call">module</span>(<span class="string">"app"</span>, [<span class="string">"chart.js"</span>]).<span class="function call">controller</span>(<span class="string">"BarCtrl"</span>, <span class="storage function">function</span> ($scope) {
  $scope.labels <span class="keyword operator">=</span> [<span class="string">'2006'</span>, <span class="string">'2007'</span>, <span class="string">'2008'</span>, <span class="string">'2009'</span>, <span class="string">'2010'</span>, <span class="string">'2011'</span>, <span class="string">'2012'</span>];
  $scope.series <span class="keyword operator">=</span> [<span class="string">'Series A'</span>, <span class="string">'Series B'</span>];

  $scope.data <span class="keyword operator">=</span> [
    [<span class="constant numeric">65</span>, <span class="constant numeric">59</span>, <span class="constant numeric">80</span>, <span class="constant numeric">81</span>, <span class="constant numeric">56</span>, <span class="constant numeric">55</span>, <span class="constant numeric">40</span>],
    [<span class="constant numeric">28</span>, <span class="constant numeric">48</span>, <span class="constant numeric">40</span>, <span class="constant numeric">19</span>, <span class="constant numeric">86</span>, <span class="constant numeric">27</span>, <span class="constant numeric">90</span>]
  ];
});
              </code>

</body>
  <script src="bower_components/angular/angular.min.js"></script>
  <script src="bower_components/Chart.js/Chart.min.js"></script>
  <script src="bower_components/angular-chart.js/dist/angular-chart.min.js"></script>


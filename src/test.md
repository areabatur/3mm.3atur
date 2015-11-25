<!DOCTYPE html>
<html ng-app="graf">
<head>
  <link rel="stylesheet" href="/angular-chart.css">
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.4/css/bootstrap.min.css" />
</head>
<body>
  <div class="col-lg-6 col-sm-12" id="bar-chart" ng-controller="BarCtrl">
    <div class="panel panel-default">
      <div class="panel-heading">Bar Chart</div>
      <div class="panel-body">
        <canvas id="bar" class="chart chart-bar" data="data" labels="labels" series="series"
                options="options"></canvas>
      </div>
    </div>
  </div>
 
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.4.3/angular.min.js"></script>
<script src="/js/Chart.min.js"></script>
<script src="/js/angular-chart.min.js"></script>
<script>
(function(){
var app = angular.module('graf', ['chart.js']);
app.controller("BarCtrl", function ($scope) {
  $scope.labels = ['2006', '2007', '2008', '2009', '2010', '2011', '2012'];
  $scope.series = ['Series A', 'Series B'];
 
  $scope.data = [
    [65, 59, 80, 81, 56, 55, 40],
    [28, 48, 40, 19, 86, 27, 90]
  ];
});
 
  })();
</script>
</body>
</html>

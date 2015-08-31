react-chartjs
============

rich interactive react charting components using [chart.js](http://www.chartjs.org/) including

* Line chart
* Bar chart
* Radar chart
* Polar area chart
* Pie chart
* Doughnut chart

[view chart examples](http://jhudson8.github.io/react-chartjs/index.html)

Installation
------------

This is a normal javascript file that you can include with a script tag

You must also include chartjs and react before this

Example Usage
-------------
```
var LineChart = ReactChartjs.Line;

var MyComponent = React.createClass({
  render: function() {
    return <LineChart data={chartData} options={chartOptions} width="600" height="250"/>
  }
});
```

* ```data``` represents the chart data (see [chart.js](http://www.chartjs.org/) for details)
* ```options``` represents the chart options (see [chart.js](http://www.chartjs.org/) for details)
* all other parameters will be passed through to the ```canvas``` element
* if data passed into the component changes, points will animate between values using chart.js' ```.update()```. If you want the chart destroyed and redrawn on every change, pass in ```redraw``` as a prop. For example ```<LineChart data={this.state.chartData} redraw />```

Chart References
----------------
The ```canvas``` element can be retrieved using ```getCanvas``` and the ```chartjs object``` can be retrieved using ```getChart```.


### Other React projects that may interest you

* [jhudson8/react-mixin-manager](https://github.com/jhudson8/react-mixin-manager)
* [jhudson8/react-backbone](https://github.com/jhudson8/react-backbone)
* [jhudson8/react-events](https://github.com/jhudson8/react-events)


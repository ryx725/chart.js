# chart.js

In my project, the tooltip show all the time not depend on the mouse evnet.

//my bar chart
var ctx = document.getElementById("canvas").getContext("2d");
		myBarChart = new Chart(ctx).Bar(barChartData, {
			responsive : true
		});
		
//get all bars
  var bars=myBarChart.datasets[0].bars;
	myBarChart.showTooltip(bars,false); 
	
//remove the mouse event
Chart.defaults = {
		global: {
		...
			// Array - Array of string names to attach tooltip events
			//tooltipEvents: ["mousemove", "touchstart", "touchmove", "mouseout"],
		...
		
		


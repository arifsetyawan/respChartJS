responsive Chart.js
=======
This distribution extending Chart.js capability by adding responsive feature.
Whole tribute and source of Chart.js can be download and update on its origin [repository](https://github.com/nnnick/Chart.js "Chart JS") + [documentation](http://www.chartjs.org/docs/ "Chart JS Documentation")


i'am wrap this feature in file chartjs-option.js through function 
	
	respChart(selector,data)
	
Setting
------
1. Import Chart.js source at the first place. i recomended the head.js power to doing this
2. Import chartjs-option.js after step 1 declaration and make sure that this part only be execute after Chart.js ready.
3. Create a canvas and make sure it has container.

		...
		<canvas class="myChart" width="800" ></canvas>
		...

4. Prepare your data  
		
		<script>
		...
		var data = {
			labels : ["January","February","March","April","May","June","July"],
			datasets : [
				{
					fillColor : "rgba(151,187,205,0.5)",
					strokeColor : "rgba(151,187,205,1)",
					pointColor : "rgba(151,187,205,1)",
					pointStrokeColor : "#fff",
					data : [28,48,40,19,96,27,100]
				}
			]
		};
		...

5. Call the extended function

		respChart($(".myChart"),data);
		
6. Enjoy your responsive chart



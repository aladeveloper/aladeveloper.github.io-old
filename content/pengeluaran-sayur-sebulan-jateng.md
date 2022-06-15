Title: Belanja Sayur Sebulan Warga Meningkat 1.19% Sejak 2019
Date: 2022-06-15 10:20
Category: Jawa Tengah
Slug: pengeluaran-sayur-sebulan
Tags: consumer behavoiur,spending,vegetables
Authors: Faris Priadi

<script src="https://cdn.jsdelivr.net/npm/chart.js@3.0.0/dist/chart.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-datalabels@2.0.0"></script>
<div id='chart-box' style="padding-top: 50px; padding-bottom: 100px;">
	<canvas id="myChart" width="400" height="100"></canvas>
</div>
<script>
Chart.register(ChartDataLabels);
const ctx = document.getElementById('myChart').getContext('2d');
const myChart = new Chart(ctx, {
    type: 'line',
    data: {
        labels: [
						"2018",
						
						"2019",
						
						"2020",
						
						"2021",
						],
        datasets: [{
            label: '',
            data: [
						3.55,
						
						3.32,
						
						3.72,
						
						4.51,
						],
            backgroundColor: [
                'grey',
                'rgba(54, 162, 235, 1)',
                'rgba(54, 162, 235, 1)',
                'rgba(54, 162, 235, 1)',
            ],
            datalabels: {
	        	color: 'blue',
	        	align: 'end',
    			anchor: 'end',
    			color: function(context) {
		          return context.dataset.backgroundColor;
		        },
		        font: function(context) {
		          var w = context.chart.width;
		          return {
		            size: 15,
		            weight: 'bold',
		          };
		        },
      		}
        }],
        
    },
    options: {
    	responsive: true,
    	plugins:  {
	      datalabels: {
	        color: 'optionsrange',
	        padding: 5
	      },
	      legend : {
	      	display: false,
	      }
	    },
	    // Core options
	    aspectRatio: 4 / 1,
	    layout: {
	      padding: {
	        top: 32,
	        right: 16,
	        bottom: 16,
	        left: 20
	      }
	    },
        scales: {
            y: {
                // beginAtZero: true,
                display : false,
                ticks : {
                	stepSize: 0.01

	            },
            },
            x: {
            	grid: {display: false, drawBorder: false},

            }

        }

    }
});
</script>
	    
# Map-Visualisation-of-Ghana-s-Energy-Sector
"This map shows the distribution of Ghana's energy sub-stations"

https://samysagoe.github.io/Map-Visualisation-of-Ghana-s-Energy-Sector/

<!DOCTYPE html>
<html>
  <head>
    <title>Energy-Map-of-Ghana</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    

  <script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>
  <script>
    google.charts.load('current', { 'packages': ['map'] });
    google.charts.setOnLoadCallback(drawMap);

    function drawMap() {
      var data = google.visualization.arrayToDataTable([
        ['Country', 'Population'],
        ['China', 'China: 1,363,800,000'],
        ['India', 'India: 1,242,620,000'],
        ['US', 'US: 317,842,000'],
        ['Indonesia', 'Indonesia: 247,424,598'],
        ['Brazil', 'Brazil: 201,032,714'],
        ['Pakistan', 'Pakistan: 186,134,000'],
        ['Nigeria', 'Nigeria: 173,615,000'],
        ['Bangladesh', 'Bangladesh: 152,518,015'],
        ['Russia', 'Russia: 146,019,512'],
        ['Japan', 'Japan: 127,120,000']
      ]);

    var options = {
      showTooltip: true,
      showInfoWindow: true
    };

    var map = new google.visualization.Map(document.getElementById('chart_div'));

    map.draw(data, options);
  };
  </script>
  </head>
  <body>
    <div id="chart_div"></div>
  </body>
</html>

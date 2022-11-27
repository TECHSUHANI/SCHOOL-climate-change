DOCTYPE html>
<html>
<head>
<style>
h1 {text-align: center;}
</style>
</head>
<body>

<h1 style="border:5px solid Teal;">CLIMATE CHANGE</h1>
<meta name="viewport" content="width=device-width, initial-scale=1">
<style>
* {box-sizing: border-box}

/* Set height of body and the document to 100% */
body, html {
  height: 100%;
  margin: 0;
  font-family: Arial;
}

/* Style tab links */
.tablink {
  background-color: #008080;
  color: white;
  float: left;
  border: none;
  outline: none;
  cursor: pointer;
  padding: 14px 16px;
  font-size: 17px;
  width: 25%;
}

.tablink:hover {
  background-color: #777;
}

/* Style the tab content (and add height:100% for full page content) */
.tabcontent {
  color: white;
  display: none;
  padding: 100px 20px;
  height: 100%;
}

#Intro {background-color: SteelBlue;}
#Consequences {background-color: MediumAquaMarine;}
#Solutions {background-color: SteelBlue;}
#Credits {background-color: MediumAquaMarine;}
</style>
</head>
<body>

<button class="tablink" onclick="openPage('Intro', this, 'SteelBlue')">Intro</button>
<button class="tablink" onclick="openPage('Consequences', this, 'MediumAquaMarine')" id="defaultOpen">Consequences</button>
<button class="tablink" onclick="openPage('Solutions', this, 'SteelBlue')">Solutions</button>
<button class="tablink" onclick="openPage('Credits', this, 'MediumAquaMarine')">Credits</button>

<div id="Intro" class="tabcontent">
  <h3>Climate change refers to long-term shifts in temperatures and weather patterns.
These shifts may be natural, but since the 1800s, human activities have been the main driver of climate change, primarily due to the burning of fossil fuels (like coal, oil, and gas), which produces heat-trapping gases.</h3>
  <p>....</p>
</div>

<div id="Consequences" class="tabcontent">
  <h3>consquences</h3>
  <p>.......</p> 
</div>

<div id="Solutions" class="tabcontent">
  <h3>solutions</h3>
  <p>.....</p>
</div>

<div id="Credits" class="tabcontent">
  <h3>Credits</h3>
  <p>........</p>
</div>

<script>
function openPage(pageName,elmnt,color) {
  var i, tabcontent, tablinks;
  tabcontent = document.getElementsByClassName("tabcontent");
  for (i = 0; i < tabcontent.length; i++) {
    tabcontent[i].style.display = "none";
  }
  tablinks = document.getElementsByClassName("tablink");
  for (i = 0; i < tablinks.length; i++) {
    tablinks[i].style.backgroundColor = "";
  }
  document.getElementById(pageName).style.display = "block";
  elmnt.style.backgroundColor = color;
}

// Get the element with id="defaultOpen" and click on it
document.getElementById("defaultOpen").click();
</script>
   
</body>
</html> 




# PetufoCZ.github.io
<!DOCTYPE html>
<html>
<body>

<div>
<input id="hrubamzdapole" type="text"><br>
<input id="vlozit" type="submit" value="Spočítat" onclick="spocitat()"><br>
<ul>
<li>Hrubá mzda: <span id="hrubamzdavysledek"></span></li>
<li>Superhrubá mzda: <span id="superhrubamzdavysledek"></span></li>
<li>Cista mzda: <span id="cistamzdavysledek"></span></li>
</ul>
</div>

<script>
function spocitat() {
var hrubamzda = document.getElementById("hrubamzdapole").value;
var superhrubamzda = hrubamzda*1.34;
var soczam = hrubamzda*0.09;
var zdravzam = hrubamzda*0.25;
var soc = hrubamzda*0.065;
var zdrav = hrubamzda*0.045;
var dan = superhrubamzda*0.15;
var poplatnik = 2070;
var cistamzda = hrubamzda-(dan+soc+zdrav)+poplatnik;
document.getElementById("hrubamzdavysledek").innerHTML = hrubamzda;
document.getElementById("superhrubamzdavysledek").innerHTML = superhrubamzda;
document.getElementById("cistamzdavysledek").innerHTML = cistamzda;
};
</script>

</body>
</html>

# Danipower27.github.io
<!DOCTYPE html>
<html lang="en-US">
<head>
   <title> Práctica 3-1</title>
   <meta charset="UTF-8">
</head>
<body style="background: #C0C0C0" align = "center" onload="startTime()">
	<div id="clockdate">
  <div class="clockdate-wrapper">
    <div id="clock"></div>
    <div id="date"></div>
  </div>
</div>
<script type="text/javascript">
	function startTime() {
    var today = new Date();
    var hr = today.getHours();
    var min = today.getMinutes();
    var sec = today.getSeconds();
    ap = (hr < 12) ? "<span>AM</span>" : "<span>PM</span>";
    hr = (hr == 0) ? 12 : hr;
    hr = (hr > 12) ? hr - 12 : hr;
    //Add a zero in front of numbers<10
    hr = checkTime(hr);
    min = checkTime(min);
    sec = checkTime(sec);
    document.getElementById("clock").innerHTML = hr + ":" + min + ":" + sec + " " + ap;
    
    var months = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December'];
    var days = ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat'];
    var curWeekDay = days[today.getDay()];
    var curDay = today.getDate();
    var curMonth = months[today.getMonth()];
    var curYear = today.getFullYear();
    var date = curWeekDay+", "+curDay+" "+curMonth+" "+curYear;
    document.getElementById("date").innerHTML = date;
    
    var time = setTimeout(function(){ startTime() }, 500);
}
function checkTime(i) {
    if (i < 10) {
        i = "0" + i;
    }
    return i;

}
</script>
<link rel="stylesheet" type="text/css" href="MiCSS.css">
<table border="5px" align="center">
	<tr>
		<td colspan="6"><strong>Nombre:</strong> Daniel Pérez Luis <strong>Año Escolar:</strong> 2020/21 <strong>Curso:</strong> 2º CTA</td>
	</tr>
	<tr>
		<td colspan="6"><h1 align="center"><strong>HORARIO DE CLASE <br><img src="lapiz.png" ></br></h1></strong></td>
	</tr>
	<tr>
		<td align="center"><strong>Hora</strong></td>
		<td align="center"><strong>Lunes</strong></td>
		<td align="center"><strong>Martes</strong></td> 
		<td align="center"><strong>Miércoles</strong></td>
		<td align="center"><strong>Jueves</strong></td>
		<td align="center"><strong>Viernes</strong></td>
	</tr>
	<tr>
		<td align="center"><strong>14:00-14:45</strong></td>
		<td align="center" style="color: #B40404">Historia de España</td>
		<td align="center" style="color: #1531BE">Matemáticas</td>
		<td align="center" style="color: #1531BE">Matemáticas</td>
		<td align="center" style="color: #0A6A0F">Química</td>
		<td align="center" style="color: #A86617">Inglés</td>
	</tr>
    <tr>
    	<td align="center"><strong>14:45-15:30</strong></td>
    	<td align="center" style="color: #A86617">Inglés</td>
    	<td rowspan="2" align="center" style="color: #5A7100">Religión</td>
    	<td align="center"style="color: #0A6A0F">Química</td>
    	<td rowspan="2" align="center" style="color: #FA6A6A">TFL</td>
    	<td align="center"style="color: #0A6A0F">Química</td>
    </tr>
    <tr>
    	<td align="center"><strong>15:30-16:15</strong></td>
    	<td align="center" style="color: #FA6A6A">TFL</td>
    	<td align="center" style="color: #FF8000">Biología</td>
    	<td align="center" style="color: #6A0D74">Lengua</td>
    </tr>
    <tr>
    	<td align="center"><strong>16:15-16:45</strong></td>
    	<td colspan="5"align="center" style="color: #F8FBEF">Recreo</td>
    </tr>
    <tr>
    	<td align="center"><strong>16:45-17:30</strong></td>
    	<td align="center" style="color: #1531BE">Matemáticas</td>
    	<td align="center" style="color: #0A6A0F">Química</td>
    	<td align="center" style="color: #A86617">Inglés</td>
    	<td align="center" style="color: #FF8000">Biología</td>
    	<td align="center" style="color: #B40404">Historia de España</td>
    </tr>
    <tr>
    	<td align="center"><strong>17:30-18:15</strong></td>
    	<td align="center" style="color: #6A0D74">Lengua</td>
    	<td align="center" style="color: #FF8000">Biología</td>
    	<td align="center" style="color: #FE2EC8">Alemán</td>
    	<td align="center" style="color: #6A0D74">Lengua</td>
    	<td rowspan="2" align="center" style="color: #FE2EC8">Alemán</td>
    </tr>
    <tr>
    	<td align="center"><strong>18:15-19:00</strong></td>
    	<td align="center" style="color: #FF8000">Biología</td>
    	<td align="center" style="color: #088A68">Tutoría</td>
    	<td align="center" style="color: #B40404">Historia de España</td>
    	<td align="center" style="color: #1531BE">Matemáticas</td>
    </tr>
</table>
</body>
</html>

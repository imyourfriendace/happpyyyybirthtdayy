<!DOCTYPE html>
<html>
<style>
body, html {
  height: 100%;
  margin: 0;
}

.birthdayimg {
  background-image: url('https://wallpapercave.com/wp/wp2592008.jpg');
  height: 100%;
  background-position: center;
  background-size: cover;
  position: relative;
  color: red;
  font-size: 35px;
}

.topleft {
  position: absolute;
  color: green;
  top: 0;
  left: 12px;
}

.bottomleft {
  position: absolute;
  color: red;
  bottom:0;
  left: 18px;
}

.middle {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
}

hr {
  margin: auto;
  width: 40%;
}
</style>

<body>
<div class="birthdayimg">
  <div class="topleft">
    <p>HI CRUSHIECAKES</p>
  </div>
  <div class="middle">
    <h1>HAPPY BIRTHDAY</h1>
    <hr>
    <p id="amx" style="font-size:80px"></p>
  </div>
  <div class="bottomleft">
    <p>MABUHAY KA HANGGA'T GUSTO KO </p>
  </div>
</div>

<script>
var countDownDate = new Date("Jul 23, 2023 00:00:00").getTime();

var countdownfunction = setInterval(function() {

  var now = new Date().getTime();
var distance = countDownDate - now;

 var days = Math.floor(distance / (1000 * 60 * 60 * 24));
  var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
  var seconds = Math.floor((distance % (1000 * 60)) / 1000);

  document.getElementById("amx").innerHTML = days + "D " + hours + "H "
  + minutes + "M " + seconds + "S ";

 if (distance < 0) {
    clearInterval(countdownfunction);
    document.getElementById("amx").innerHTML = "HAPPY BIRTHDAY CRUSHICAKES";
    window.location = "https://youtu.be/tL6SQ2PGXV4";
}

}, 1000);
</script>

</body>
</html>







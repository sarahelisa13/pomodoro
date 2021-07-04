var minutos = 25;
var segundos = 0;

var minutos_interval;
var segundos_interval;

var click1 = new Audio("click1.mp3");
var bell1 = new Audio("bell1.mp3");

function template(minutos = 25, segundos='00'){
    document.getElementById("minutos").innerHTML = minutos;
    document.getElementById("segundos").innerHTML = segundos;
}
function minutostimer(){
    minutos = minutos -  1;
    document.getElementById("minutos").innerHTML = minutos;
}
function segundostimer(){
    segundos = segundos - 1;
    document.getElementById("segundos").innerHTML = segundos;
    if (segundos <= 0) {
        if (minutos <= 0) {
           bell1.play();
          clearInterval(minutos_interval);
          clearInterval(segundos_interval);
    
          document.getElementById("done").innerHTML = "Tarefa feita! Hora do Intervalo!"
          document.getElementById("done").classList.add('show_message');
    
         
        }
        segundos = 60;
      }
}
function iniciarDescanso() {
    click1.play();
  template(5, 0);

  minutos = 4;
  segundos = 59;

  document.getElementById("minutos").innerHTML  = minutos;
  document.getElementById("segundos").innerHTML = segundos;

  minutos_interval  = setInterval(minutostimer, 60000);
  segundos_interval = setInterval(segundostimer, 1000);
}

function start() {
    click1.play();
    
    minutos = 24;
    segundos = 59;
  
    document.getElementById("minutos").innerHTML  = minutos;
    document.getElementById("segundos").innerHTML = segundos;
  
    minutos_interval  = setInterval(minutostimer, 60000);
    segundos_interval = setInterval(segundostimer, 1000);
  }
let posCirculoX;
let posCirculoY;
let circuloDirH = true;
let circuloDirV = true;
let posRaqueteX;
let posRaqueteY;

function setup()
{
  createCanvas(665, 400);
  posCirculoX = 665/2;
  posCirculoY = 400/2;
}

function draw()
{
  background(25);
  circle(posCirculoX, posCirculoY, 50);
  circle(posRaqueteX, posRaqueteY, 75);
  posRaqueteX = 50;
  posRaqueteY = mouseY - 25;
  moverBola();
  bolaColidirRaquete();
}

function moverBola()
{
  if(posCirculoX > 640)
    {
      circuloDirH = false;
    }
  else if(posCirculoX < 25)
    {
      circuloDirH = true;
    }
 
  if(circuloDirH == true)
    {
      posCirculoX = posCirculoX + 5;
    }
  else
    {
      posCirculoX = posCirculoX - 5;
    }
 
  if(posCirculoY > 375)
    {
      circuloDirV = false;
    }
  else if(posCirculoY < 25)
    {
      circuloDirV = true;
    }
 
  if(circuloDirV == true)
    {
      posCirculoY = posCirculoY + 5;
    }
  else
    {
      posCirculoY = posCirculoY - 5;
    }
}
function bolaColidirRaquete()
{
  let distanciaX = posRaqueteX - posCirculoX;
  let distanciaY = posRaqueteY - posCirculoY;
  let distancia = sqrt((distanciaX*distanciaX) + (distanciaY*distanciaY));
 
  if(distancia <= 62.5)
    {
      circuloDirH = true;
    }
}

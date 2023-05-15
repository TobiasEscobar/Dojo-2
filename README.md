# Dojo-2 
(Primer entrega)

## Integrantes 
- Tobías Fabricio Escobar

## Proyecto: SUBTE
[Proyecto 1](![Dojo 2°-1° Entrega- Escobar Tobías Fabricio](https://github.com/TobiasEscobar/Dojo-2/assets/98720272/e4e17f84-cf9a-4446-a667-bc0609a640cc)

## Descripción
Implementar un sistema que permita al usuario saber a qué estación de subte está llegando, aparte el sistema muestra las estaciones que faltan hasta llegar a destino,
para ello debemos utilizar 4 LEDs y el display de 7 segmentos. Esta vez el buzzer deberá emitir un sonido diferente cada vez que se llegue a una estación.
El sistema deberá arrancar apagado, luego de presionar el botón empezará y hará lo pedido.

## Función principal
void loop()
{

  int encendido = digitalRead(BOTON);
  Serial.println("encendido");

//Si el boton es presionado, se cumple la condicion y se ejecuta su codigo
  if(encendido == 0)
  {
  Serial.println("Llego a constitucion");   			
  prenderDisplay(1, 1, 1, 1, 0, 0, 1, LED_ROJO, 1000);
    
  Serial.println("Llego a San Juan");
  prenderDisplay(1, 1, 0, 1, 1, 0, 1, LED_VERDE, 1000);
    
  Serial.println("Llego a Independencia");
  prenderDisplay(0, 1, 1, 0, 0, 0, 0, LED_AZUL, 1000);
    
  Serial.println("Llego a Moron");
  prenderDisplay(1, 1, 1, 1, 1, 1, 0, LED_AMARILLO, 1000);
  }
}

## :robot: Link al proyecto
- [proyecto](https://www.tinkercad.com/things/0RSGAV9Lyxk-dojo-2-1-entrega-escobar-tobias-fabricio/editel)
---

# UBICUA
Proyecto de UBICUA: Sistema de control inteligente de plantas con Alexa

- ESP32 DevKit (Microcontrolador):
  *VELOCIDAD DE RELOJ: 160-240 MHz
  *RAM: 520Kb
  *BLUETOOTH
  *TARJETA WIFI
  *36 GP10 PIN
  *16 ADC de 16 bits + 2 DAC de 8 bits
  *16 canales PWM
  *2 Puertos series (com3)
 
�� TENED ESTAS CARACTER�SITICAS MUY EN CUENTA A LA HORA DE CREAR C�DIGO QUE VAYA A CORRER SOBRE EL MICROCONTROLADOR!!

src/server --> servidor lanzado con JAVA Spring para tener un servicio WEB (estoy barajando el quitarlo por tiempo, y hacerlo directamente sobre HTML usando el IDE de ARDUINO, y que el servidor corra directamente sobre la IP de la microcontroladora como si fuera un LOCALHOST)

src/ESPAlexa --> c�digo para conectar el ESP32 con ALEXA, a�n est� muy b�sico. Alexa detecta el ESP como si fuera una LUZ (TODO: CAMBIAR ESO), adem�s arranca con "Alexa, enciende..." ver c�mo cambiar para que sea "Alexa, riega..." y reconfigurar para que arrance la bomba de agua (por ahora enciende una luz)

src\dsb18b20_to_WebServer --> Lectura del sensor DSB18b20 mostrando los datos en una web a la que nos conectamos usando la IP de red del ESP. Los datos en la web se muestran en Celsius y Farenhein y el dise�o es muy b�sico, es una prueba de concepto m�s bien.

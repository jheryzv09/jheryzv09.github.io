# jheryzv09.github.io

# PARKING AUTOMATIZADO CON COONTROL DE AFORO EN TIEMPO REAL

## RESUMEN

Mi maqueta del parking automatizado estará compuesta por un sistema de sensores colocados estratégicamente en la entrada. Al detectarse un vehículo en el acceso, el sistema activará de forma automática la subida de la barrera y mostrará en el panel un mensaje de **BIENVENIDO**. De igual modo, al detectar un vehículo en la salida, la barrera se abrirá y el panel mostrará un mensaje de **HASTA LUEGO, BUEN VIAJE**.

Cada plaza estará equipada con un sensor de ocupación que enviará información al controlador principal, que en nuestro caso usaremos Arduino. Según el estado de cada plaza, se encenderá una luz verde (libre) o roja (ocupada). Estos datos se reflejarán simultáneamente en el panel LED, donde se mostrará el número de plazas disponibles. 

Existirá otro panel superior donde solamente figure el estado del parking, es decir cuando el sistema detecte que quedan plazas libres dentro del parking lo indicará con un mensaje de **PARKING LIBRE** y cuando detecte que todas las plazas están ocupadas, el panel indicará claramente **PARKING COMPLETO**.

Además, el panel contará con un reloj digital que mostrará la hora en tiempo real, aportando un aspecto más completo y realista al conjunto.

## ABSTRACT

My automated parking project will consist of a system of sensors strategically placed at the entrance. When a vehicle is detected at the access point, the system will automatically raise the barrier and display a **WELCOME** message on the panel. Likewise, when a vehicle is detected at the exit, the barrier will open and the panel will show a **GOODBYE, HAVE A SAFE TRIP** message.

Each parking space will be equipped with an occupancy sensor that will send information to the main controller, which in our case will be an Arduino. Depending on the status of each space, a green light (free) or red light (occupied) will turn on. This data will be simultaneously reflected on the LED panel, where the number of available spaces will be displayed.

There will also be an upper panel that shows only the overall parking status. When the system detects that there are free spaces inside the parking lot, it will indicate this with a **PARKING AVAILABLE** message. When it detects that all spaces are occupied, the panel will clearly display **PARKING FULL**.

Additionally, the panel will include a digital clock showing the real-time hour, providing a more complete and realistic look to the system.

## ESTADO DEL ARTE
El crecimiento del parque automovilístico en entornos urbanos ha provocado un aumento de los problemas relacionados con la gestión del estacionamiento: congestión, pérdida de tiempo en la búsqueda de plazas libres, aumento de emisiones contaminantes y una experiencia de usuario poco eficiente. Como respuesta a esta problemática, en los últimos años han surgido los sistemas de aparcamiento inteligentes, integrados dentro del concepto de Smart Cities.
Un sistema de parking inteligente se basa en la detección automática de vehículos, la gestión del aforo y la comunicación de información en tiempo real al usuario. Estos sistemas combinan electrónica, sensórica, programación y automatización para optimizar el uso de las plazas disponibles.

**TECNOLOGÍAS EMPLEADAS ACTUALMENTE**

Los desarrollos existentes en el ámbito del parking automatizado suelen apoyarse en las siguientes tecnologías:

- **Sensores de detección de vehículos:**
  Se utilizan sensores ultrasónicos, infrarrojos (IR), magnéticos o cámaras con visión artificial para detectar la presencia de un vehículo en una plaza o en los accesos de entrada y salida.         Los sensores ultrasónicos (como el HC-SR04) son especialmente comunes en entornos educativos y prototipos por su bajo coste y facilidad de integración.

- **Controladores embebidos:**
  Muchos sistemas de pequeña y mediana escala se basan en plataformas como Arduino, ESP32 o Raspberry Pi. Estos dispositivos permiten la lectura de sensores, el procesamiento de datos y la           activación de actuadores en tiempo real.

- **Actuadores y sistemas de acceso:**
  Las barreras automáticas suelen funcionar mediante servomotores o motores paso a paso, controlados electrónicamente. Su activación puede depender de la disponibilidad de plazas o de la detección   de un vehículo autorizado.

- **Sistemas de señalización:**
  Es habitual el uso de LEDs rojo/verde por plaza para indicar ocupación, así como paneles informativos LED o LCD en la entrada que muestran el número de plazas libres.

- **Gestión del aforo:**
  El conteo de vehículos se realiza mediante sensores en la entrada y salida. El sistema mantiene una variable de ocupación que se incrementa o decrementa según el flujo de coches, bloqueando el     acceso cuando se alcanza la capacidad máxima.

**SOLUCIONES COMERCIALES Y ACADÉMICAS**


En el ámbito comercial, existen parkings que incorporan:

- Paneles informativos exteriores con número de plazas disponibles.

- Sensores individuales en cada plaza conectados a redes inalámbricas.

- Aplicaciones móviles para reservar plaza.

- Integración con sistemas de pago automático.

Sin embargo, estos sistemas suelen tener costes elevados, infraestructuras complejas y dependencia de redes de comunicación avanzadas.
En el ámbito educativo y de investigación, se desarrollan prototipos a escala que permiten estudiar:

- La automatización de accesos.

- La lógica de control de aforo.

- La integración de múltiples sensores.

- La simulación de situaciones reales (parking lleno, vacío, fallos de detección).

Estos proyectos suelen priorizar bajo coste, modularidad y facilidad de mantenimiento, utilizando componentes estándar y plataformas abiertas.

**ENFOQUE DE MI PROYECTO**


El proyecto de Parking Automatizado con Control de Aforo en Tiempo Real se sitúa dentro de esta línea de sistemas inteligentes, pero con un enfoque didáctico, modular y de bajo coste. A diferencia de las soluciones comerciales, se centra en:

- El uso de Arduino como núcleo de control.
  
- Sensores ultrasónicos e infrarrojos para la detección en accesos y plazas.
  
- Barreras automáticas accionadas por servomotores.
  
- Señalización visual por plaza mediante LEDs.

- Panel informativo que muestra el estado del parking.
  
- Lógica de conteo de vehículos y bloqueo automático cuando se alcanza el aforo máximo.


Este proyecto toma como base los principios de los sistemas de parking inteligentes actuales, pero los adapta a una maqueta funcional, permitiendo comprender de forma práctica la interacción entre hardware, software y automatización.






Shield: [![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

This work is licensed under a
[Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[![CC BY-SA 4.0][cc-by-sa-image]][cc-by-sa]

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg

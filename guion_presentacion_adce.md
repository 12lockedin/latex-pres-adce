Hola a todos, vamos a hablar de una tendencia y novedad tecnológica muy
interesante en el campo del control de tensión: Los Transformadores de
Estado Sólido (SST por sus siglas en inglés).
Para que entendáis mejor qué hacen estos transformadores de estado sólido,
me gustaría recordar dos aparatos que todos conocemos:
1. En primer lugar, el transformador convencional. Este es un dispositivo
que mediante los campos electromagnéticos de dos devanados consigue
transformar los niveles de tensión en corriente alterna. Es un
dispositivo importante, porque es una de las principales razones por las
que utilizamos corriente alterna.
2. En segundo lugar, el STATCOM. Lo vimos hace dos clases. Es un
dispositivo que ayuda a controlar la tensión de la red eléctrica y mejorar
la calidad del suministro. Su función es casi exclusivamente el
intercambio de potencia reactiva para regular la tensión local. Solo
consume la potencia activa necesaria para cubrir sus propias pérdidas
internas. Están basados en un convertidor electrónico, los VSC (Voltage
Source Converters).
Los SST o transformadores de estado sólido son equipos de paso, como los
trafos convencionales, se conectan en serie al flujo de potencia, a diferencia de
los STATCOM, que se conectan en paralelo (o derivación) para ayudar al nodo
local. En muchos casos, se comporta como un transformador convencional y
un compensador a la vez.
En esencia, las características de un SST son:
● transformar los niveles de tensión mientras transmite potencia activa.
● capacidad para modificar el factor de potencia.
● regulación de tensión dinámica (a diferencia del trafo convencional, si
la tensión de entrada baja un 10%, el SST puede mantener la salida
exactamente a 230V o el valor deseado).
● peso y volumen drásticamente inferior a un trafo convencional, esto es
debido a utilizar frecuencias mucho más altas en la transformación,
cerca de 20 000 Hz en comparación con los 50 Hz de la red. Esto se
consigue rectificando primeramente la rede de 50 Hz a DC y
posteriormente generando la señal a la frecuencia deseada.
● tiene un bus de corriente continua que permite conectar tanto consumo
(como carga de coches eléctricos) como generación (como placas
solares) de DC directamente sin necesidad de convertidores externos
adicionales.
● Eliminación de armónicos perjudiciales para la red.
● Es un elemento clave para las SmartGrids, ya que puede decidir cuánta
energía deja pasar y en qué dirección.
Se usa principalmente en redes de Media Tensión y Baja Tensión, debido a los
límites de tensión de los semiconductores actuales.
El esquema típico de un SST se divide en los siguientes bloques conectados en
serie:
1. Etapa de Entrada (Rectificador AC/DC):
○ Se conecta a la red de Media Tensión.
○ Convierte la señal alterna en continua.
○ Controla el factor de potencia y reduce armónicos (similar a la
función del STATCOM, pero transfiriendo energía).
2. Etapa Intermedia (Convertidor DC/DC de Alta Frecuencia):
○ Es el "corazón" del SST.
○ Incluye un Inversor, un Transformador de Alta Frecuencia (HFT)
y un Rectificador.
○ El HFT es mucho más pequeño y ligero que un transformador
convencional de 50/60 Hz debido a la alta frecuencia de operación.
○ Proporciona el aislamiento galvánico entre la alta y la baja
tensión.
3. Etapa de Salida (Inversor DC/AC):
○ Convierte la tensión del bus de continua a una señal alterna (AC)
de Baja Tensión.
○ Alimenta la carga o la red secundaria con tensión y frecuencia
controladas.
Es decir,
1. convertimos a DC →
2. convertimos a AC ALTA FRECUENCA →
3. transformamos la tensión en AC ALTA FRECUENCIA →
4. esa corriente en AC ALTA FRECUENCIA la volvemos a convertir a DC →
5. y una vez más, convertimos ese DC a AC a la frecuencia de red (50 Hz).
Aunque parece complejo, este sistema permite:
- Que el transformador físico sea mucho más pequeño y ligero.
- Controlar el voltaje de salida de forma instantánea si hay caídas en la
red.
- Eliminar armónicos y mejorar el factor de potencia (algo que el
STATCOM del libro también hace, pero el SST lo hace mientras
transfiere potencia a una carga).
Los Transformadores de Estado Sólido combinan transformación de tensión,
compensación reactiva y control dinámico en un equipo compacto, siendo
ideales para estaciones de recarga ultrarrápida, microredes con renovables y
SmartGrids donde su bidireccionalidad y conexión directa DC son clave.
Sin embargo, enfrentan barreras importantes: coste elevado, mayores
pérdidas que los trafos convencionales (>99% rendimiento), limitaciones de
tensión a Media/Baja, y contribuyen a la pérdida de inercia del sistema
eléctrico al sustituir equipos electromecánicos por electrónica de potencia,
reduciendo la estabilidad natural ante perturbaciones de frecuencia. Estas
limitaciones indican que aún queda un largo camino para su implantación
generalizada.
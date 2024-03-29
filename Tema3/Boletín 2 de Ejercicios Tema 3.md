# Boletín 2 de Ejercicios Tema 3

### Pasar a modelo relacional

1. ![image-20201203131202771](/home/user22/.config/Typora/typora-user-images/image-20201203131202771.png)

### Realizar el diagrama ER Ampliado y luego realizar el modelo relacional (a tablas)

2. El club de Ajedrez Master Chess, ha sido encargado por la Federación Internacional de Ajedrez de la organización de los próximos campeonatos mundiales que se celebrarán a finales de 2020. Por este motivo, desea llevar a una base de datos toda la gestión relativa a participantes, alojamientos y partidas. Teniendo en cuenta que:

- En el campeonato participan (participantes de los que se necesita saber nacionalidad) jugadores y árbitros, de ambos se requiere conocer el número de asociado, nombre, dirección y teléfono de contacto. De los jugadores se precisa además el nivel de juego en una escala de 1 a 10. Y de los árbitros guardaremos los años de experiencia.
- Ningún árbitro puede participar como jugador.
- Los países envían al campeonato un conjunto de jugadores y árbitros, aunque no todos los países envían participantes. Todo jugador y árbitro es enviado por un único país. Un país puede ser representado por otro país.
- Cada país se identifica por un número correlativo según su orden alfabético e interesa conocer además su nombre y el número de clubes de ajedrez existentes en el mismo.
- Cada partida se identifica por un número correlativo (CódigoPartida), la juegan dos jugadores y la arbitra un árbitro. Interesa registrar las partidas que juega cada jugador y el color (blancas o negras) con el que juega. Ha de tenerse en cuenta que un árbitro no puede arbitrar a jugadores enviados por el mismo país que ha enviado él.
- Todo participante participa en al menos una partida.
- Tanto jugadores como árbitros se alojan en uno de los hoteles en los que se desarrollan las partidas, se desea conocer en qué hotel y en qué fechas se ha alojado cada uno de los participantes. Los participantes pueden no permanecer en Huércal de Almería durante todo el campeonato, sino acudir cuando tienen que jugar alguna partida alojándose en el mismo o distinto hotel. De cada hotel, se desea conocer el nombre, la dirección y el número de teléfono.
- El campeonato se desarrolla a lo largo de una serie de jornadas (año, mes, día) y cada partida tiene lugar en una de las jornadas aunque no tengan lugar partidas todas las jornadas.
- Cada partida se celebra en una de las salas de las que pueden disponer los hoteles, se desea conocer el número de entradas vendidas en la sala para cada partida. De cada sala, se desea conocer la capacidad y medios de que dispone (radio, televisión, vídeo,…) para facilitar la retransmisión de los encuentros. Una sala puede disponer de varios medios distintos.
- De cada partida se pretende registrar todos los movimientos que la componen, la identificación de movimiento se establece en base a un número de orden dentro de cada partida, para cada movimiento se guardan la jugada (5 posiciones) y un breve comentario realizado por un experto.
# 1. Comprender el problema 
Responde brevemente:

## ¿Quién utilizará estos datos?
El ayuntamiento de la ciudad
## ¿Qué decisiones se pueden tomar con ellos?
Modificar el tráfico, disponer o no areas verdes, crear zonas de bajas emisiones, etc.
## ¿Qué diferencia hay entre una alerta inmediata y un informe histórico?
Un informe histórico es todos los datos que se han obtenido a lo largo del tiempo de un conjunto de datos. Una alerta inmediata es un o un conjunto de datos que son inusuales dentro de ese registro histórico.

# 2. Analizar cobertura y calidad 
Utilizando el dossier:

## Identifica dos problemas de calidad y explica sus consecuencias.
Unidades incorrectas: Eso puede crear problemas graves a la hora de analizar los datos, pues destruye las medias.
Lecturas congeladas: Esto es un problema, sobre todo si se sigue repitiendo, porque sus valores volverian anomalas las medias calculadas.

## Indica qué distrito necesita mayor atención y justifica tu respuesta.
D2 Norte residencial y D4 Sur industrial son zonas muy pobladas, muy amplias y con menos sensores que otras zonas. 
D6 parque natural no tiene ninguno. Debería tener al menos uno por control de muestras.

## Elige una anomalía y explica si la corregirías, la marcarías como dudosa o la excluirías.
Valores extremos: Los marcaría como dudosos y analizaría si es un fallo de los sensores o es un problema real a analizar.

# 3. Comparar arquitecturas

Completa esta tabla:

| Criterio |	Batch |	Streaming |
| --- | --- | --- | 
| Rapidez para generar alertas | Minutos u horas | Segundos o pocos minutos		
| Coste y complejidad |	Menores | Mayores	
| Informes históricos |	Muy adecuados | Adecuado, con más complejidad	
| Picos de datos | Se tratan en el siguiente lote | Requieren ventanas y marcas de agua		

# 4. Elaborar una recomendación 
Redacta una recomendación para el ayuntamiento que incluya:

El riesgo más urgente.
La actuación que propones.
Dos razones basadas en el dossier.
Un problema que seguiría pendiente.
Una medida de privacidad.

Recomendaciones para la mejora de los servicios de sensores: Urgentemente se deb catalogar el sensor sin marcar, para no tener datos de origen desconocido. Tambien debería buscar una manera de que el código no permita la entrada de valores fuera de las unidades permitidas. 
Se debería analizar porque hay huecos en los registros y ver si guarda relación con que algunos sensores parecen congelarse a veces.
Estamos pendientes de hacer el manteniemientos de los registros.
Como medida de privacidad, revisar que los datos no generan una posición exacta del lugar del detector, sino de la zona.
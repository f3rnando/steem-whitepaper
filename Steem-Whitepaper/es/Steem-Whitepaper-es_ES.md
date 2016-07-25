	Steem White Paper #spanish translation effort 
# Steem
## Una plataforma de "social media", basada en blockchain, con incentivos.

Daniel Larimer, Ned Scott, Valentine Zavgorodnev, Benjamin Johnson, James Calfee, Michael Vandeberg

Marzo 2016

---

# Abstract
Steem es una base de datos blockchain que permite la contrucción comunitaria e interacción social con premios en criptomoneda. Steem combina conceptos de *social media* con los aprendizajes provenientes de la construcción de criptomonedas y sus comunidades. Una clave importante para inspirar participación de cualquier comunidad, moneda o economía de libre mercado es un sistema de contabilidad justa que refleje consistentemente la contribución de cada persona. Steem es la primer criptomoneda que intenta recompenzar de forma acertada y transparente una cantidad indeterminada de individuos que realizan *contribuciones subjetivas* a su comunidad.

---

# Tabla de contenidos
1. Abstract
2. Tabla de contenidos
3. Introducción
	3.1 Reconociendo las contribuciones
4. Formas de contribuir
	- 4.1 Contribuciones de capital
	- 4.2 Steem (STEEM)
	- 4.3 Steem Power (SP)
	- 4.4 Steem Dollars (SBD)
      - 4.4.1 Minimizando comisiones fraudulentas
      - 4.4.2 Mitigando ataques de cadencia
      - 4.4.3 Minimizando el abuso de conversiones
      - 4.4.4 Liquidez
      - 4.4.5 Deuda sostenible a relaciones de propiedad
      - 4.4.6 Intereses
      - 4.4.7 Definiendo fuentes de precios
	- 4.5 Contribuciones subjetivas
		- 4.5.1 Distribuyendo la moneda
		- 4.5.2 Votando sobre la distribución de la moneda
			- a. Complicidad en la votación
			- b. La historia del *Crab Bucket*
		- 4.5.3 Tasa limitada de voto
		- 4.5.4 Pagos retrazados
		- 4.5.5 Distribución de pagos
			- a. Recompensas para posts padres.
        - 4.5.6 Pagos
    4.6 Algoritmo de consenso
    	- 4.6.1 Consenso en Steem
    	- 4.6.2 Minando en Steem
    		- a. Premios de minado requieren Steem Power
            - b. Algoritmo de minado
            - c. Resistencia a Botnets
            - d. Resistencia de Pools de minado
        - 4.6.3 Eliminando comisiones de transacción
        	- a. El problema de las comisiones
            	- a.a Los micropagos no funcionan
                - a.b Las comisiones son barreras para el acceso.
              	- a.c Cambiando las comisiones
                - a.d Ataques de identidad (Sybil attacks)
                - a.e Reserva completa vs. reserva fraccionada
            - b. Iterando mas allá de los micropagos
            	- b.a Ejemplo de implementación
                - b.b Caso de estudio: Bitcoin
                	- b.b.a Impacto de capacidad
                    - b.b.b Numero máximo de usuarios únicos
                    - b.b.c Comparación a comisiones
                - b.c Creación de cuenta
                - b.d Justificando balances mínimos
                - b.c Ajustando relación de reserva
                - b.d Efectividad relativa a comisiones
                - b.e Renta vs. Compra vs. Tiempo compartido
            - c. Performance y Escalabilidad
            	- c.a Escala Reddit
            - d. Asignación y suministro
            	- d.a Impacto de Tasa de creacion de tokens
                	- d.a.a Impacto de tasa de cración de tokens mayor al noventa porciento
                    - d.a.b Sistema contable
            - e. El poder de Steem
            	- e.a Sin micropagos, Propina opcional
                - e.b El valor está en los enlaces
                - e.c Resolviendo el problema de abordaje de las criptomonedas
                - e.d Resolviendo el problema de liquidación de las criptomonedas
                - e.e Censura
                - e.f Resolviendo el descubrimiento orgánico a través de optimización en motores de búsqueda
                - e.g Viraje hacia la atribución basada en Blockchain
                - e.h Reemplazando la publicadad con recompenzas de contenido basado en Blockchain
            - f. Conclusión
            

---

# Introducción

El contenido generado colectivamente por usuarios ha creado billones de dólares en valor para los accionista de compañias de *social media* como Reddit, Facebook y Twitter. En 2014, Reddit hipotetizó que su plataforma podría ser mejorada si todos los que contribuyen en reddit.com posteando historias, agregando comentarios o votando fuesen premiados con una cantidad justa de participación en Reddit, Inc[[1]](#1). Steem apunta a apoyar comunidades online y de *social media* devolviendo gran parte de su valor a la gente que provee valiosas contribuciones, premiándolos con criptomoneda, y a través de este proceso crear una moneda que puede alcanzar un mercado masivo, incluyendo gente que aún no ha participado en alguna economía de criptomoneda.

Hay algunos principios clave que han sido utilizados para guiar el diseño de Steem. El más importante es que todos los que contribuyen a una empresa deben recibir una participación prorrateada, pago o débito de la empresa.
Este principio es el mismo que se aplica en casi todas las *Startups*, estas colocan acciones durante la fundación y durante rondas de inversión subsecuentes.

El segundo principio es que todas las formas de capital son igualmente valiosas. Esto significa que aquellos que contribuyen su escaso tiempo y atención en producir y curar contenido para otros, son tan valiosos como quienes contribuyen con su capital. Este es el principio de equidad de sudor[[2]](#2) y es un concepto que previo a las criptomonedas ha tenido problemas para proveer a no más de algunas docenas de individuos.

El tercer principio es que la comunidad produce productos para servir a sus miembors. Esto se ejemplifica con las uniones de crédito, coperativas de alimentos, planes de salud compartidos, que sirven a los miembros de sus comunidades mas que vender productos o servicios a la gente fuera de la comunidad.

La comunidad de Steem provee los siguientes servicios a sus miembros:
1. Una fuente de noticias y comentarios curada.
2. Medios para obtener respuestas de alta calidad a preguntas personalizadas.
3. Una criptomoneda estable vinculada al Dólar Estadounidense.
4. Pagos libres.
5. Trabajos que proveen los servicios antes mencionados a otros miembros.


El útil realineamiento de incentivos económicos de Steem tiene el potencial de producir resultados justos y mas inclusivos para todos los involucrados que las plataformas de *social media* y criptomonedas que la preceden.

Este documento explorará los incentivos económicos existentes y demostrará cómo Steem y sus incentivos podrán resultar mejor para la mayoría de los participantes.

---

[1] Reddit’s Cryptocurrency, Forbes, Erika Morphy, Octubre 2014,
http://www.forbes.com/sites/erikamorphy/2014/10/01/reddits-cryptocurrency-could-have-many-uses/#4e07b05332b9
[2] Sweat Equity, Investopedia,
http://www.investopedia.com/terms/s/sweatequity.asp


---

## 3.1 - Reconociendo las contribuciones

Steem está diseñado desde cero para resolver las mayores barreras para su adopción y monetizaciones de una economías basada en *social media*.
Nuestra tésis es que las mismas técnicas usadas para hacer crecer las mas grandes plataformas de *social media* pueden ser utilizadas para iniciar una criptomoneda existosa.
Incentivos económicos habilitados por criptomoneda pueden facilitar dramáticamente el crecimientod de una nueva plataforma de *social media*. Es la sinergía entre criptomoneda y *social media* lo que creemos que puede dar a Steem una poderosa ventaja en el mercado.

El reto afrontado por Steem es derivar un algoritmo para tasar contribuciones individuales que la mayor parte de los miembros de la comunidad consideren una evaluación justa del valor subjetivo de cada contribución.
En un mundo perfecto, los miembros de la comunidad coperarían para valuar la contribución de cada par y devolver una justa compensación. En el mundo real, deben diseñarse algoritmos de tal forma que sean resistentes a manipulación intencional con fines de lucro. Cualquier abuso del sistema de tasación podría causar la pérdida de fe en la percepción de justicia del sistema económico por parte de sus miembros.

Las plataformas existentes operan en un principio de un usuario, un voto. Esto crea un ambiente donde los rankings pueden ser manipulados por ataques de profeta y los proveedores de servicio deben proactivamente identificar y bloquar abusadores. La gente actualmente intenta manipular los sistemas de tasacipon de Reddit, Twitter y Facebook siendo la única ganancia el tráfico web o la censura.

La unidad fundamental de contabilidad en la plataforma de Steem es STEEM, un token de criptomoneda.
Steem opera en la base de un STEEM, un voto. Bajo este modelo, los individuos que mas hayan contribuido a la plataforma, segun lo corroborado por el balance de su cuenta, tienen mayor influencia sobre cómo se valúan las contribuciones. Además, Steem solo permite a los miembros votar con STEEM cuando este es sujeto a un esquema multi-anual de adquisición.
Los miembros tienen un incentivo financiero para votar en el sentido que ésto maximiza el valor a largo plazo de sus propios STEEM.

Steem está diseñado alrededor de un concepto relativamente simple: toda contribución significativa a la comunidad debería ser reconocida por el valor que añade. Cuando la gente es reconocida por sus contribuciones, continúan contribuyendo y la comunidad crece.
Cualquier desbalance en el ida y vuelta dentro de una comunidad es insustentable. Eventualmente los dadores se cansan de soportar a los miembros que restan y atentan contra la comunidad.

El reto es crear un sistema capaz de identificar qué contribuciones son necesarias y su valor relativo de manera que pueda escalar a un numero indeterminado de gente.
Un sistema comprobado para evaluar y premiar contribuciones es el libre mercado. El libre mercado puede ser visto como una comunidad única donde todos intercambian con otros y las recompenzas son asignadas por pérdidas y ganancias. El sistema de mercado premia aquellos que proveen valor a otros y castiga a quienes consumen más valor del que producen. El mercado libre soporta muchas monedas diferentes y el dinero es simplemente una *commodity* que todos encuentran fácil de intercambiar.

Desde que el libre mercado es un sistema comprobado, es tentador intentar crear un sistema de igual característica donde los consumidores de contenido pagan directamente a los productores del mismo. De todas formas, el pago directo es ineficiente y realmente inviable para la creación y curado de contenido. El valor de la mayoría del contenido es muy bajo en relación con el costo cognitivo, financiero y de oportunidad asociado con hacer un pago que algunos pocos lectores eligen beneficiar. La abundancia de alternativas libres siginifica que la aplicación de un *muro de pago* derivará a los lectores a otro lado. Han habido gran cantidad de intentos de implementar micro pagos por artículo de parte de los lectores hacia los autores, pero ninguno se ha alcanzado una amplitud considerable.

Steem está diseñado para permitir micropagos efectivos por cualquier tipo de contribución al cambiar la ecuación económica. Los lectores ya no tienen que decidir si pagar o no a alguien desde su propio bolsillo, en cambio votan  o restan votos y Steem usa estos votos para determinar premios individuales. Esto significa que se le otorga a la gente una interfaz familiar y ampliamente utilizada y ya no enfrentan los costos de oportunidad, cognitivos y financieros asociados tradicionalmente a los micropagos y plataformas de propinas.

El voto de los miembros de la comunidad es crítico para que Steem acomode los pagos a los contribuyentes de forma precisa.
El voto puede por lo tanto ser visto como una contribución crucial y digno de ser recompenzado en sí mismo. Algunas plataformas, como Slashdot, usan meta-moderación[[3]](#3) como una forma de rankear y premiar a los moderadores honestos. Steem entonces premia a quienes mas contribuyen al total de la promoción de una pieza de contenido pagando a los votantes proporcionalmente al pago principal del creador del contenido votado.

Hay otras formas de contribución que Steem reconoce y premia usando métricas objetivas. Entre ellas están: validación de transacciones, minado de prueba de trabajo, premios de liquidez, y reportado de productores de bloque malitencionados.

[3] Meta-moderacion es un segundo nivel de moderación de comentarios. Los usuarios son invitados a valuar las decisiones de los moderadores para mejorar la moderación.
https://en.wikipedia.org/wiki/Meta-moderation_system


---

# 4. Formas de contribuír
Esta sección delínea las ideas detrás de Steem y sus recompenzas para la gente que provee contribuciones significativas y mesurables a la comunidad de Steem.

## 4.1 - Contribuciones de capital
Hay dos items que una comunidad puede ofrecer para atraer capital: deuda y propiedad.
Quienes compran propiedad ganan cuando la comunidad crece pero pierden si la misma decrece.
Quienes compran deuda obtienen la garantia de un cierto monto de interpes pero no llegan a participar de las ganancias realizadas por el crecimiento de la comunidad. Ambos tipos de contribuciones de capital son valiosas para el crecimiento de la comunidad y la valuación de su moneda.
Adicionalmente hay dos formas en que la propiedad puede conservarse: liquidez y colocación.
La colocación de propiedad genera un compromiso de largo plazo y no puede ser vendida por un determinado período de tiempo.

La red Steem llama a estas diferentes clases de asstes Steem (STEEM), Steem Power (SP), y Steem Dollars (SMD)

## 4.2 - Steem (STEEM)

Steem es la unidad fundamental contable en el blockchain de Steem. Los demás tokes derivan su valor del de STEEM. Generalmente STEEM deberia ser mantenido por cortos períodos de tiempo cuando se necesita liquidez. Alguien que busque entrar o salir de la plataforma de Steem tendrá que comprar o vender STEEM. Una vez comprado debería ser convertido a SP o SMD para mitigar el impacto de la dilución en el largo plazo.
STEEM crece constantemente en oferta por un 100% anual debido a incentivos no SMD. Quien tenga STEEM sin convertirlos a SP, se diluirán aproximadamente en un 0.19% diario. Mientras el ritmo puede parecer alto, para transacciones que toman menos de 10 dias, sigue siendo mas barato que las comisiones de proceso de tarjetas de crédito. Ademas, la creación diaria de *tokens* es insignificante al lado de la volatilidad diaria.

Quien compre Bitcoin o cualquier otra criptomoneda y la venda 10 dias después podría perder fácilmente 3% o mas debido a las fluctuaciones de precio. Quien compre Bitcoin y luego lo venda en el mismo dia usualmente pagará mas del 0.4% sólo en comisiones del mercado de intercambio.
En otras palabras, el ritmo de inflacipon es efectivamente insignificante durante el período de tiempo que un individuo típico sostendrá STEEM.

La mayoría de la inflación es de hecho un artefacto de contabilidad en lugar de un verdadero reacomodamiento de riqueza. El 90% de la inflación no SMD es redistribuída a los poseedores existentes de STEEM proporcionalmente al valor de STEEM de su balance de SP, convirtiendo la inflación en mas bien una repartición. Solo alrrededor del 10% de la inflación no SMD redistribuye propiedad en la red.

## 4.3 Steem Power (SP)

Las Startups o los emprendimientos requieren un compromiso de capital a largo plazo. Aquellos que invierten su dinero en estas companías calculan esperar años antes de poder vender sus acciones y efectivizar su ganancia.
Sin compromiso a largo plazo, una *startup* buscando recolectar capital adicionar a través de la venta de acciones adicionales estaría compitiendo con accionistas existentes queriendo retirarse. Los inversores compresivos quieren que sus contribuciones de capital hagan crecer la compañía, pero el crecimiento no puede suceder si el nuevo capital es entregado a los que buscan retirarse.

Hay un valor significativo en tener compromiso a largo plazo porque habilita a las comunidades a hacer planes a largo plazo. El compromiso a largo plazo de los *stakeholders* también causa que estos voten por el crecimiento a largo plazo en lugar de bombeos de corto plazo.

En el espacio de las criptomonedas, los especuladores saltan de criptomoneda en criptomoneda basados mayormente en las expectativas de crecimiento a corto plazo. Steem busca armar una comunidad que sea propiedad y controlada enteramente por aquellos con perspectivas a largo plazo.
Debido a que Steem busca alentar el crecimiento a largo plazo, está fijado en su lógica la acomodacion de 9 STEEM a los poseedores de Steem Power (SP) por cada STEEM que crea para financiar el crecimiento a través de incentivos a la contribución. En el tiempo, esto lleva a que la relación entre el total de valor en STEEM de Steem Power (SP) se balacee al total de los balances STEEM hacia un 9:1. (Al parecer, esta relación probablemente supere el 9:1 debido al contínuo empoderamiento de la red de los nuevos STEEM emitidos)
Esto también significa que los poseedores a largo plazo son potegidos casi por completo de la dilucion utilizada en la financiación del crecimiento.

Los SP sólo pueden ser convertidos a STEEM luego de 2 años a través de 104 pagos semanales equitativos. *1 SP* puede ser visto como una acción en un *pool* de STEEM. La red automáticamente agrega STEEM al *pool* en cada bloque. En cualquier momento, los usuarios puede convertir sus STEEM en SP en la misma relación en que el STEEM en el *pool* de plazos fijos al total de SP. Convertir STEEM a SP no diluye a los poseedores existentes de SP.
Mas bien, cada vez que se convierte de SP a STEEM, se hace con la relación del momento. Los individuos tienen garantizado poseer mas STEEM en el futuro de lo que tienen cuando convierten por primera vez desde STEEM a SP.

Los balances de SP son no-transferibles y no-divisibles excepto a través de las solicitudes recurrentes automáticas de conversión. Esto significa que el SP no puede ser intercambiado en *exchanges* de criptomonedas.

Poseer SP es requerido para votar a favor o denunciar contenido. Esto quiere decir que el SP es el *token* de acceso que otorga a sus poseedores poderes exclusivos dentro de la plataforma de Steem.

La acción de transferir desde STEEM a SP es llamada *Powering Up* mientras laa transferencia de SP a STEEM es *Powering Down*. Por ejemplo, uno puede hacer *Power Down* de sus STEEM sobre un período de 2 años, pero se puede hacer *Power Up* con sus STEEM inmediatamente.

## 4.4 - Steem Dollars (SMD)

La estabilidad es un componente importante en las economías globales exitosas. Sin estabilidad, los individuos en distintas partes del mundo no podrían tener costos cognitivos bajos al participar en el comercio y ahorro. Por este motivo, los Steem Dollars fueron diseñados como un intento de traer estabilidad al mundo de las criptomonedas y a los individuos que usen la red Steem.

Los Steem Dollars (SMD) son creados por un mecanismo similar a las notas convertibles, que son usualmente utilizadas para financias *startups*. En el mundo de las *startups*, las notas convertibles son instrumentos de deuda a corto plazo que pueden ser convertidos a propiedad a un ritmo determinado en el futuro, típicamente durante una futura ronda de inversión. Un *token* basado en blockchain puede ser visto como propiedad mientras una nota convertible puede ser vista como deuda con denominación en otra *commodity* o moneda. Los términos de la nota convertible permiten a su dueño convertirla al *token* que la respalda con una antelación mínima al precio justo del mercado del *token*. Crear dólares convertibles a *tokens* habilita a los blockchains a crecer su efecto de red mientras se maximiza el retorno a los poseedores de *tokens*.

Los *Steem Dollars* son nomenclados con el símbolo SMD, su acrónimo. Para crear los SMD se requiere una combinación entre un indicador de precio confiable, reglas para prevenir el abuso, y liquidez.
Proveer un indicador de precio confiable implica tres factores: minimizar el impacto de un indicador incorrecto, maximizar el costo de producir un indicador incorrecto, y minimazar la importancia de la cadencia.

### 4.4.1 - Minimizando comisiones fraudulentas

Los poseedores de SP eligen individuos para publicar indicadores de precio. Estos individuos seleccionados son presumiblemente poseen la confianza de aquellos que tienen un interés personal en la calidad del indicador. Al pagarle a quienes son elegidos, Steem crea un mercado competitivo para obtener el derecho de producir indicadores. Mientras mas productores de indicadores reciben pagos menos les conviene a éstos publicar información falsa. 

Habiendo varios productores electos y confiables, el precio determinado para conversiones puede ser derivado entonces del promedio de los indicadores. De esta forma si alguna minoría de productores de indicadores publican valores atípicos, éstos tienen entonces un impacto mínimo en el promedio pero de todas formas se afecta su reputación.

Aún si todos los productores son honestos, es posible que la mayoría de éstos sean afectados por eventos que estén más allá de su control. La red de Steem está diseñada para tolerar corrupciones de corto plazo en el indicador promediado mientras la comunidad trabaja activamente en la corrección del problema. Un ejemplo de un problema que puede tomar cierto tiempo para corregir es la manipulación de mercado a corto plazo. La manipulación de mercado es dificultosa y costosa de mantener por períodos largos. Otro ejemplo sería la falla de un servicio de intercambio centralizado o la corrupción de los datos publicados por el mismo.

Steem elimina el factor de las fluctuaciones de precio de corto plazo usando el promedio del período de una semana. El indicador de promedio publicado es generado cada una hora.

Siempre que una corrupción en el indicador de precios dure menos que la ventana de tiempo del promedio móvil, habrá un impacto mínimo en el precio de conversión. Si eventualmente el indicador es corrompido, los participantes de la red tendrán una oportunidad para votar la expulsión de los productores de indicadores corrompidos antes que impacten en el precio efectivo de conversión.

Tal vez lo mas importante es que le da a los productores una oportunidad para detectar y corregir los problemas antes que sus indicadores comiencen a afectar el precio promediado.
Con una ventana de tiempo de una semana, los miembros de la comunidad tienen tres dias y medio para responder y mitigar los problemas que puedan surgir.

### 4.4.2 - Mitigando ataques de cadencia

Los participantes del mercado tienen acceso a información antes de lo que el promedio móvil semanal de precio de conversión pueda reaccionar. Esta información puede ser utilizada para beneficio de los operadores a expensas de la comunidad. Si hay un incremento repentino en el valor de STEEM, los operadores podrían solicitar la conversión de sus SMD al precio anterior, más bajo, y luego vender los STEEM recibidos a un nuevo precio mayor con muy bajo riesgo.

Steem nivela el juego al imponer a todos los pedidos de conversión un retardo de una semana. Esto significa que ni los operadores ni el blockchain tienen ventaja con respecto al precio cuando la conversión se ejecuta.






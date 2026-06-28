link del video:
 https://youtu.be/EuGmN7zJ3ZM

Guion de Exposición: Sistemas Expertos (Versión Extendida)
Diapositiva 1: Portada (Tiempo estimado: 1.5 minutos)
Texto en Diapositiva:

Sistemas Expertos: Fundamentos y Arquitectura.

Presenta: Isaias Emmanuel Poot Orlaineta.

Guion (Tú en cámara, de cuerpo entero):
"Hola a todos, mi nombre es Isaias Emmanuel Poot Orlaineta, soy estudiante de la carrera de Ingeniería en Sistemas Computacionales, en la universidad autonoma del carmen. En esta exposición vamos a profundizar en uno de los pilares históricos y estructurales más importantes de la Inteligencia Artificial: Los Sistemas Expertos._

Hoy en día, cuando escuchamos el término 'Inteligencia Artificial', es muy común que nuestra mente piense inmediatamente en redes neuronales, en ChatGPT o en generación de imágenes. Sin embargo, para que la informática llegara a ese punto, tuvo que dar un salto fundamental en el siglo pasado: pasar de ser máquinas que procesaban simples cálculos matemáticos de manera secuencial, a convertirse en sistemas capaces de procesar el razonamiento humano. Mi objetivo en esta presentación es explicar de forma clara qué son estos sistemas, cómo es que logramos extraer la inteligencia de un especialista humano para meterla en una computadora, y abordar los conceptos clave de su arquitectura. Comencemos."
(Aquí ya puedes quitar tu cámara y dejar solo la presentación).

Diapositiva 2: El Conocimiento en la IA (Tiempo estimado: 2.5 minutos)
Texto en Diapositiva:

¿Qué es el Conocimiento?

Diferencia entre Datos, Información y Conocimiento.

La experiencia estructurada y la heurística.

Guion:
"Para hablar de sistemas expertos, el primer punto que debemos dejar absolutamente claro es el concepto de 'Conocimiento'. En la informática tradicional, los programadores solemos trabajar con 'Datos', que son números o textos sin contexto. Si procesamos esos datos, obtenemos 'Información'. Por ejemplo, un dato es el número '39'. La información sería decir 'El paciente tiene 39 grados Celsius de temperatura'.

Pero el 'Conocimiento' va un paso más allá de la información. El conocimiento es la experiencia humana, los conceptos, las intuiciones y, sobre todo, las reglas prácticas —lo que en Inteligencia Artificial llamamos 'heurística'— que un especialista utiliza para resolver un problema. Saber que '39 grados en un adulto requiere un análisis de infección y administrar paracetamol' es conocimiento empírico.

En la Inteligencia Artificial existe una rama llamada 'Ingeniería del Conocimiento'. Su objetivo es precisamente extraer toda esta experiencia del cerebro de un experto humano (por ejemplo, un médico cardiólogo, un ingeniero geólogo o un analista financiero) y traducirla a un formato lógico que la computadora pueda procesar. Este proceso requiere de dos actores principales: el Experto Humano, que es quien tiene el saber; y el Ingeniero de Conocimiento, que es el informático encargado de entrevistar al experto, analizar cómo toma sus decisiones, y codificar esa lógica en el sistema."

Diapositiva 3: La Base de Conocimiento (Tiempo estimado: 2.5 minutos)
Texto en Diapositiva:

Base de Conocimiento (Knowledge Base).

Hechos (Verdades absolutas del dominio).

Reglas lógicas (Condicionales IF-THEN).

Guion:
"Una vez que el Ingeniero de Conocimiento logra extraer la experiencia del especialista, surge la pregunta: ¿dónde guardamos toda esta inteligencia? Aquí entra nuestro segundo concepto fundamental de la arquitectura: la Base de Conocimiento.

Es muy importante no confundir esto con una Base de Datos tradicional. Una base de datos guarda tablas con registros aislados y estáticos usando lenguajes como SQL. En cambio, una Base de Conocimiento guarda las relaciones lógicas y condicionales entre esos datos, permitiendo que el sistema infiera cosas nuevas.

Se compone principalmente de dos grandes elementos. Primero, tenemos los 'Hechos'. Los hechos representan el conocimiento declarativo, es decir, las verdades dinámicas sobre el problema actual que estamos intentando resolver. Segundo, tenemos las 'Reglas', que representan el conocimiento procedimental. Las reglas son expresiones lógicas estáticas que generalmente siguen la estructura condicional IF-THEN, es decir, 'SI ocurre tal premisa, ENTONCES llego a tal conclusión'. Además, las bases de conocimiento modernas incluyen mecanismos de control de coherencia, para evitar que al sistema se le inyecten reglas contradictorias que provoquen que la máquina arroje resultados absurdos."

Diapositiva 4: El Motor de Inferencia (Tiempo estimado: 3 minutos)
Texto en Diapositiva:

Motor de Inferencia.

El procesador lógico del sistema experto.

Encadenamiento hacia adelante (Forward Chaining).

Encadenamiento hacia atrás (Backward Chaining).

Guion:
"El tercer concepto clave es el Motor de Inferencia. Si dijimos que la base de conocimiento es la 'memoria' del sistema, entonces el motor de inferencia es el 'cerebro o el procesador analítico'. Su trabajo es tomar los hechos que el usuario ingresa, buscar en las reglas almacenadas, hacer coincidencias de patrones y deducir nuevas conclusiones usando leyes lógico-matemáticas como el Modus Ponens (afirmando, afirmo) o el Modus Tollens (negando, niego).

Para resolver problemas, este motor utiliza principalmente dos estrategias algorítmicas o métodos de búsqueda:
El primero es el 'Encadenamiento hacia adelante' o Forward Chaining. Aquí, el sistema es alimentado con los datos iniciales y empieza a disparar reglas en cascada hasta llegar a una solución final. Es un método ideal para tareas de planificación o configuración. Por ejemplo, si le damos las dimensiones de una habitación y el presupuesto, el sistema deduce qué muebles comprar.

El segundo método es el 'Encadenamiento hacia atrás' o Backward Chaining. Aquí, el algoritmo funciona al revés: asume una hipótesis final y busca hacia atrás para ver si los datos que tenemos comprueban esa teoría. Es el método por excelencia para los diagnósticos médicos o el soporte técnico. Por ejemplo, el sistema asume la hipótesis: 'La computadora tiene la fuente de poder quemada', y empieza a preguntar al usuario por los síntomas específicos para validar o descartar esa hipótesis.

Además, algo brillante de este motor es que incluye un Subsistema de Explicación. Esto significa que el sistema puede explicarle al usuario exactamente la ruta de reglas que siguió para darle un resultado, dotando a la IA de una transparencia total."

Diapositiva 5: Línea de Tiempo de los Sistemas Expertos (Tiempo estimado: 2.5 minutos)
Texto en Diapositiva:

1965: DENDRAL (Análisis químico).

1972: MYCIN (Diagnóstico médico).

1979: XCON / R1 (Configuración de hardware).

Guion:
"Pasando al cuarto punto, es fundamental dar un breve recorrido por la línea de tiempo de estos sistemas para comprender su impacto en la historia del software.

Todo comenzó en el año 1965, en la Universidad de Stanford, con la creación de DENDRAL. Este es considerado universalmente como el primer sistema experto del mundo. Fue desarrollado para el campo de la química, y su propósito era deducir la estructura molecular de compuestos a partir de datos de espectrometría de masas, logrando hacerlo a una velocidad y precisión que superaba a la de los químicos humanos de la época.

Posteriormente, en 1972 nace MYCIN, también en Stanford. MYCIN fue un hito absoluto porque se adentró en el diagnóstico médico. Analizaba síntomas para identificar infecciones bacterianas severas en la sangre y recomendaba dosis exactas de antibióticos ajustadas al peso del paciente. Lo más sorprendente de MYCIN fue que operaba con 'factores de certeza', lidiando con información médica incompleta, y en evaluaciones ciegas logró un porcentaje de acierto mayor que el de muchos médicos residentes.

Finalmente, en 1979 surge XCON, originalmente llamado R1. Fue desarrollado para la empresa fabricante de computadoras DEC (Digital Equipment Corporation). A diferencia de los anteriores que eran académicos, XCON fue el primer gran éxito comercial de la IA. Automatizaba la selección y configuración de componentes de hardware, asegurando que los clientes recibieran piezas compatibles. Le ahorró a la compañía decenas de millones de dólares al año, demostrando que la Inteligencia Artificial era económicamente viable en la industria."

Diapositiva 6: Tipos de Sistemas Expertos (Tiempo estimado: 2 minutos)
Texto en Diapositiva:

Sistemas Basados en Reglas (RBS).

Sistemas Basados en Casos (CBR).

Sistemas Basados en Redes Bayesianas.

Guion:
"Como quinto punto, es importante destacar que, debido a la complejidad de los problemas del mundo real, no todos los sistemas expertos estructuran su conocimiento de la misma manera. Existen varias tipologías principales:

Primero tenemos los 'Sistemas Basados en Reglas' o RBS. Son los más clásicos y rigurosos. Utilizan la lógica condicional estricta de IF-THEN que ya mencionamos. Son excelentes para entornos donde las leyes están perfectamente definidas, como el cálculo de impuestos o validaciones contables.

Segundo, están los 'Sistemas Basados en Casos' o CBR. Estos sistemas imitan cómo razona un abogado o un mecánico experto: no usan reglas estrictas, sino que mantienen un historial de problemas pasados. Cuando llega un problema nuevo, el sistema busca el caso antiguo más similar, recupera la solución que funcionó aquella vez y la adapta a la situación actual.

Por último, tenemos los 'Sistemas Basados en Redes Bayesianas'. Estos son sistemas probabilísticos. Se utilizan cuando el entorno es ruidoso, incierto o cuando nos faltan datos. Utilizan la estadística para calcular probabilidades condicionadas, siendo invaluables en la detección de fraudes bancarios o en diagnósticos médicos muy complejos donde los síntomas pueden ser engañosos."

Diapositiva 7: Conclusiones (Tiempo estimado: 1.5 minutos)
Texto en Diapositiva:

Conclusión.

¡Gracias por su atención!

Guion (Tú en cámara, de cuerpo entero):
"A manera de conclusión, podemos afirmar que la aparición de los sistemas expertos marcó un antes y un después en las ciencias de la computación. Demostraron empíricamente que las computadoras tenían el potencial de ir más allá del cálculo matemático puro y adentrarse exitosamente en el terreno del razonamiento deductivo humano.

Si bien es cierto que hoy la inteligencia artificial ha evolucionado hacia arquitecturas de aprendizaje profundo que aprenden solas a partir de millones de datos, los fundamentos de las bases de conocimiento y los motores de inferencia están lejos de ser obsoletos. Siguen siendo vitales y se utilizan actualmente en motores de reglas de negocio corporativos, en sistemas de soporte técnico y en cualquier industria crítica, como la medicina o la aviación, donde la transparencia es obligatoria y necesitamos que la Inteligencia Artificial nos explique exactamente por qué tomó una decisión, algo que las redes neuronales modernas aún tienen dificultades para hacer.

Con esto finalizo mi exposición. Muchas gracias por su tiempo y atención, espero que los conceptos hayan quedado claros."
# Resúmenes Analíticos de Lectura

## 1. Análisis Detallado: 0-Ingeniería-del-Conocimiento.pdf

**Concepto Fundamental y Naturaleza del Conocimiento**
El documento define la Ingeniería del Conocimiento (IC) como la disciplina encargada de la adquisición, representación, validación, inferenciación, explicación y mantenimiento del conocimiento para desarrollar Sistemas Inteligentes Artificiales. A diferencia de la informática convencional que opera con datos estructurados y algoritmos formales, la IC lidia con la subjetividad, la incertidumbre y datos incompletos. El conocimiento en este contexto se divide en tres niveles:
1.  **Conocimiento Declarativo:** Hechos, atributos y relaciones entre objetos.
2.  **Conocimiento Procedural:** Conjunto de reglas heurísticas usadas en la solución de problemas.
3.  **Metaconocimiento:** El conocimiento sobre el propio conocimiento; es decir, la capacidad del sistema para saber cómo razonar.

**Actores Principales en el Desarrollo de un Sistema Experto**
Para que un sistema experto se materialice, se requiere de la interacción de tres actores clave:
* **El Ingeniero de Conocimiento (ICO):** Es el especialista informático. Su rol no es solo programar, sino extraer el conocimiento del experto. Debe tener excelentes habilidades de comunicación y nociones de psicología para interpretar el razonamiento empírico del experto y traducirlo a estructuras de datos (codificación).
* **El Experto Humano:** Un profesional de reconocido prestigio en un dominio específico. Aporta las "fuentes primarias o dinámicas" (su experiencia, intuición y heurística).
* **El Usuario:** Quien operará el sistema final; su nivel de comprensión debe guiar la interfaz y las explicaciones del sistema.

**Fases de la Ingeniería del Conocimiento**
El documento expone 5 actividades principales para construir la inteligencia del sistema:
1.  **Adquisición del Conocimiento (AC):** Es el proceso central y más complejo. Se divide en 5 sub-etapas: Identificación del problema, Entendimiento, Formalización, Implementación de un prototipo y Pruebas. Para extraer este conocimiento se emplean tres familias de métodos:
    * *Manuales:* Entrevistas (estructuradas, semiestructuradas y no estructuradas), análisis de protocolos, análisis de casos y lluvia de ideas.
    * *Semiautomatizados:* Herramientas informáticas (como editores de conocimiento o el "Análisis de Rejilla" basado en la teoría de construcción personal de Kelly) que ayudan al experto y al ICO a codificar más rápido.
    * *Automatizados:* Eliminan la necesidad del ICO y del experto mediante el aprendizaje automático (Machine Learning) o algoritmos de inducción de reglas como el ID3, que analizan matrices de atributos y crean árboles de decisión solos.
2.  **Representación del Conocimiento (KR):** Es el esquema usado para organizar el saber extraído. Debe ser fácil de modificar, transparente e independiente. Los principales esquemas son:
    * *Lógica Simbólica:* Usa lógica proposicional (Fórmulas bien definidas con conectivos AND, OR, NOT) y lógica de predicados (constantes, variables, cuantificadores).
    * *Redes Semánticas:* Representación gráfica de la memoria asociativa mediante nodos (conceptos) y enlaces (relaciones como ES-UN o subconjunto).
    * *Frames (Marcos) o Slots:* Estructuras orientadas a objetos donde el conocimiento se divide en componentes (slots) que permiten el mecanismo de herencia jerárquica.
3.  **Validación, Inferencia y Explicación:** La comprobación de que el modelo emula correctamente la realidad, el diseño del algoritmo analítico y la capacidad del software de justificar por qué tomó cierta decisión.

---

## 2. Análisis Detallado: C-sistemasExpertosBasadosEnReglas.pdf

**Anatomía de los Sistemas Basados en Reglas**
Este documento profundiza en la estructura y el comportamiento matemático de los Sistemas Expertos utilizados para resolver situaciones complejas y deterministas (ej. transacciones bancarias o control de tráfico). El núcleo de estos sistemas se divide en dos grandes contenedores:
* **La Memoria de Trabajo:** Donde se almacenan los *Hechos*. Los hechos son dinámicos, volátiles y representan la información dada por el usuario en una consulta particular (Ej. "El NIP es correcto").
* **La Base de Conocimiento:** Donde se almacenan las *Reglas*. Son de naturaleza estática y permanente. Cada regla relaciona dos o más objetos mediante una estructura condicional lógica: "Si [Premisa], entonces [Conclusión]". 
Para mejorar el procesamiento, los motores suelen aplicar la técnica de *Sustitución de Reglas*, que consiste en traducir reglas compuestas con el operador lógico disyuntivo "O" en conjuntos de reglas simples independientes equivalentes en forma normal conjuntiva.

**Mecanismos Matemáticos del Motor de Inferencia**
El "Motor de Inferencia" es el cerebro del sistema. Realiza un reconocimiento de patrones para decidir qué reglas se activan y ejecuta su parte consecuente apoyado en tres leyes lógicas:
1.  **Modus Ponens (Avance):** Es deductivo. Si la regla dicta "Si A es cierto, entonces B es cierto", y el hecho ingresado dice "A es cierto", el motor concluye obligatoriamente que "B es cierto".
2.  **Modus Tollens (Retroceso):** Es deductivo inverso. Utiliza la misma regla ("Si A, entonces B"), pero partiendo del hecho "B es falso". El motor concluye matemáticamente que "A es falso". Es vital porque permite al sistema expandir la Base de Conocimiento sin necesidad de programar reglas redundantes.
3.  **Mecanismo de Resolución:** Utilizado para conclusiones compuestas. Cuando faltan datos, el sistema asume la *Hipótesis del Mundo Cerrado* (si no se puede demostrar que algo es cierto, el sistema asume temporalmente que es falso) o pausa el análisis para interrogar directamente al usuario.

**Estrategias de Búsqueda Algorítmica**
El motor aplica las leyes matemáticas mediante dos algoritmos de control:
* *Encadenamiento de Reglas (Hacia adelante):* El usuario ingresa una serie de datos aislados. El sistema busca reglas cuyas premisas coincidan con esos datos, dispara conclusiones y convierte esas conclusiones en nuevos hechos. El ciclo se repite hasta que la máquina no puede derivar más información.
* *Encadenamiento Orientado a un Objetivo (Hacia atrás):* Se ingresa un objetivo final (Ej. Diagnosticar si un fallo existe). El algoritmo busca la regla que produce esa conclusión y revisa si en la memoria existen los hechos para validar su premisa. Si no, busca sub-reglas u obliga a interrogar al usuario.

**Sistemas de Seguridad: Control de la Coherencia**
Finalmente, el autor advierte del colapso del sistema si se ingresa información contradictoria. Para prevenir conclusiones absurdas, los Sistemas Expertos ejecutan un Control de Coherencia:
* **Coherencia de Reglas:** Evalúa matemáticamente que ninguna nueva regla programada contradiga a una existente. Identifica "valores no factibles" (variables imposibles lógicamente).
* **Coherencia de Hechos:** Filtra las interacciones del usuario. Una vez que el usuario ingresa un dato, el sistema actualiza continuamente la base de conocimiento y bloquea opciones que choquen con las leyes existentes para evitar "alucinaciones".
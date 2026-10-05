Foro semana 5

Los siguientes escenarios están inspirados en problemas reales. Las cantidades y características de los datos son hipotéticas.

Caso 1. Detección de operaciones fraudulentas

Una empresa de pagos dispone de un millón de operaciones. Solo el 1 % corresponde a fraudes.

El dataset incluye:

Monto de la operación.

Cantidad de operaciones realizadas durante la última hora.

Antigüedad de la cuenta.

Distancia respecto de la ubicación habitual del cliente.

Tipo de comercio y medio de pago.

Etiqueta: operación fraudulenta o legítima.

Hay operaciones legítimas con montos muy elevados y fraudes con montos pequeños. Algunas combinaciones resultan sospechosas: una cuenta nueva que realiza muchas operaciones en pocos minutos, por ejemplo.

La empresa necesita responder rápidamente. Un fraude no detectado produce una pérdida económica, pero bloquear una operación legítima también perjudica al cliente.

Para debatir: ¿qué modelo podría captar mejor las combinaciones entre variables? ¿Qué dificultades tendría KNN al predecir con tantos registros? ¿Sería suficiente obtener un 99 % de exactitud para considerar bueno un modelo?

Caso 2. Predicción de abandono estudiantil

Una institución quiere identificar estudiantes que podrían abandonar durante el próximo mes para ofrecerles acompañamiento.

Dispone de 2.000 registros históricos con:

Porcentaje de asistencia.

Cantidad de actividades entregadas.

Promedio de las calificaciones disponibles hasta el momento de la predicción.

Horas semanales de trabajo.

Carrera y turno.

Disponibilidad de conexión a internet.

Etiqueta: continuó o abandonó durante el mes siguiente.

Algunas variables tienen datos faltantes. En los registros históricos, el 20 % de los estudiantes abandonó. La institución necesita comprender por qué el modelo identifica un caso como riesgoso.

Para debatir: ¿qué ventajas podrían tener la regresión logística y un árbol de poca profundidad para explicar las predicciones? ¿Qué ocurriría si un árbol aprendiera reglas basadas en muy pocos estudiantes? ¿Sería válido incorporar la fecha de baja definitiva como variable predictora?

Caso 3. Clasificación de productos por sus mediciones

Una fábrica quiere clasificar piezas como aceptables o defectuosas.

Cuenta con 6.000 registros que incluyen:

Peso, expresado en gramos.

Longitud y diámetro, expresados en milímetros.

Temperatura de fabricación.

Nivel de vibración.

Tipo de material.

Etiqueta: aceptable o defectuosa.

Las clases están aproximadamente equilibradas. Existen varios grupos de piezas aceptables con combinaciones diferentes de peso y tamaño. Algunas piezas defectuosas tienen valores muy parecidos a los de las aceptables y hay mediciones con ruido.

Para debatir: ¿podría ser útil clasificar una pieza según sus vecinas más cercanas? ¿Qué pasaría si se aplicara KNN sin escalar las variables? ¿Qué dificultades podría tener una regresión logística que utiliza las variables originales sin agregar interacciones ni transformaciones?

Primera participación: elegí un caso y defendé una propuesta

Publicá una intervención de 350 a 500 palabras, aproximadamente, que aborde los siguientes puntos:

Comparación de los tres modelos. ¿Con cuál comenzarías y por qué? Explicá también una ventaja y una limitación de cada uno para el caso elegido. No alcanza con afirmar que uno “es más preciso” sin justificarlo.

Características del dataset. Identificá al menos dos características que podrían favorecer o perjudicar a los modelos: cantidad de registros, cantidad de variables, ruido, valores atípicos, grupos de observaciones similares o relaciones entre variables. Explicá el efecto esperado.

Preparación de los datos. ¿Qué harías con las variables numéricas, categóricas y los valores faltantes? ¿En qué modelos sería especialmente importante el escalado? Si una categoría fuera “canal de contacto”, ¿qué problema podría provocar codificar teléfono = 1, correo = 2 y chat = 3?

Sobreajuste y subajuste. Explicá qué podría pasar al utilizar un K muy pequeño o muy grande, un árbol demasiado profundo o demasiado limitado y una regresión logística con regularización excesiva o insuficiente. Relacioná al menos uno de estos ejemplos con tu caso.

Evaluación y consecuencias de los errores. Definí cuál sería la clase positiva. ¿Qué significarían un falso positivo y un falso negativo? ¿Cuál tendría mayor costo? Elegí una o dos métricas relevantes y justificá por qué la exactitud —accuracy— sería suficiente o insuficiente.

Comparación justa. ¿Cómo comprobarías tu propuesta utilizando entrenamiento, validación y prueba, o validación cruzada? Explicá por qué los tres modelos deberían evaluarse sobre las mismas observaciones de prueba, aunque cada uno necesite un preprocesamiento diferente.

Terminá tu publicación con una pregunta abierta para tus compañeros.

Segunda participación: debatí con otros estudiantes

Respondé a dos compañeros, con intervenciones de entre 100 y 150 palabras cada una:

En una respuesta, cuestioná una decisión de manera fundamentada. Identificá un supuesto que podría no cumplirse y explicá cómo cambiaría la elección del modelo.

En la otra, modificá una condición del caso. Por ejemplo: aumenta la cantidad de registros, aparecen muchas categorías, crece el desbalanceo, se agregan variables irrelevantes o se exige explicar cada predicción. Analizá si mantendrías la propuesta original.

No alcanza con escribir “estoy de acuerdo”. Cada respuesta debe agregar un argumento, un ejemplo, una objeción o una alternativa.

Preguntas para profundizar el intercambio

Pueden incorporar alguna de estas preguntas a sus intervenciones:

Si un árbol obtiene 100 % de exactitud en entrenamiento y 72 % en prueba, mientras que la regresión logística obtiene 81 % y 80 %, respectivamente, ¿cuál elegirían y qué revisarían antes de decidir?

Si agregamos 50 variables irrelevantes, ¿cómo podría verse afectado cada modelo?

¿Dos modelos con la misma exactitud necesariamente cometen los mismos errores?

¿Cambiar el umbral de clasificación de la regresión logística podría ser más conveniente que cambiar de modelo?

¿Qué diferencia hay entre equilibrar los datos de entrenamiento y modificar artificialmente la proporción de clases del conjunto de prueba?

¿Por qué sería problemático escalar los datos o hacer sobremuestreo antes de separarlos en entrenamiento y prueba?

¿Un modelo fácil de interpretar es necesariamente más justo o menos propenso a cometer errores?

Si las características de los clientes, estudiantes o fraudes cambian con el tiempo, ¿seguirían siendo confiables los resultados obtenidos inicialmente?

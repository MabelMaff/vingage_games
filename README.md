# Proyecto-Juegos-Cl-sicos-en-Python
Programación en Python
Proyecto: Juegos Clásicos en Python
Proyecto 1. PyGames: Programando juegos con Python
Resumen

Objetivos

Planificación del proyecto

3.1. sprints

3.2. Criterios de aceptación

3.3. Historias de usuario

Entrega

Presentación

1. Resumen
Bienvenidas al primer proyecto del curso de Data Analytics de Adalab. Nos ha contactado una empresa que se dedica a la creación de juegos clásicos como el "Piedra Papel o Tijera" o el "Tic Tac Toe". En concreto, les gustaría explorar la posibilidad de contratarnos como parte de su equipo para desarrollar juegos en Python utilizando una clase que contenga la lógica de los juegos.

En este proyecto vamos a aprender a trabajar con Python, lo cual será una herramienta esencial en nuestro trabajo como analistas de datos, por lo que nos tendremos que sentir cómodas con el. Para ello vamos a tener que ser capaces de crear una serie de juegos usando código de Python. ¿Estáis preparadas?

Empecemos con los juegos en los que están interesados que desarrollemos:

Piedra Papel o Tijera: este es un juego clásico en el que dos jugadores seleccionan una de tres opciones: Piedra, Papel o Tijera. Cada opción tiene una relación de victoria diferente: la Piedra vence a la Tijera, la Tijera vence al Papel y el Papel vence a la Piedra. El objetivo del juego es elegir la opción que vencerá a la opción seleccionada por el oponente. El juego se juega en rondas y el jugador que gana más rondas es el ganador del juego.

Tic Tac Toe: también conocido como tres en raya, es un juego de estrategia para dos jugadores. El juego se juega en una cuadrícula de tres por tres en la que los jugadores toman turnos para colocar una "X" o una "O" en la cuadrícula. El objetivo del juego es lograr tener tres símbolos iguales en una fila, ya sea horizontalmente, verticalmente o en diagonal, antes que el oponente. El juego termina en empate si la cuadrícula se llena y ningún jugador ha logrado crear una línea de tres símbolos iguales.

Ahoracado: es un juego de adivinanzas en el que un jugador elige una palabra y el otro jugador debe adivinarla letra por letra. El jugador que adivina la palabra tiene un número limitado de oportunidades para adivinar las letras que forman la palabra. Cada vez que el jugador adivina una letra incorrecta, se dibuja una parte del cuerpo del personaje del ahorcado en una horca. Si el jugador adivina todas las letras de la palabra antes de que se complete el dibujo del personaje del ahorcado, gana el juego. Si el dibujo del personaje del ahorcado se completa antes de adivinar la palabra, pierde el juego.

Juego de preguntas y respuestas: es un juego en el que se hacen preguntas sobre una variedad de temas y los jugadores deben responder correctamente para avanzar. Las preguntas pueden ser de diferentes categorías, como historia, ciencias, entretenimiento o cultura general. El objetivo del juego es responder la mayor cantidad de preguntas correctamente para ganar el juego. Este juego puede ser jugado de forma individual o en equipo y es una forma divertida de aprender y poner a prueba tus conocimientos.

Las reglas del juego las tendréis descritas en un jupyter que encontraréis al final de este documento

2. Objetivos
Consolidar los conocimientos de Python básicos.

Utilizar control de versiones en equipo para aprender las ventajas y conflictos que genera.

Implementar Scrum como marco de referencia para el desarrollo del producto, basándonos siempre en los valores de Agile como puntos clave del trabajo en equipo y la mejora continua.

Mejorar la comunicación entre los miembros del equipo.

Mejorar vuestras habilidades de comunicación en público al exponer el proyecto en la sesión final.

3. Planificación del proyecto
3.1. sprints
Para la realización de este proyecto trabajaremos en 2 sprints (2 iteraciones). El primer sprint tendrá una duración de 3 sesiones y el segundo sprint tendrá una duración de 3 sesiones. Siguiendo los principios ágiles, estableceremos pequeños ciclos iterativos de forma que al final de cada uno generemos valor perceptible por nuestros usuarios. Dedicaremos el primer día a la planificación del sprint (sprint planning) y el resto a trabajar en el desarrollo del proyecto. Al final de cada sprint haremos un Sprint Review del proyecto para presentar los resultados conseguidos y recoger feedback.

También haremos una retro corta revisando los working agreements que hemos acordado al inicio del proyecto y añadiendo cualquier otro feedback que nos permita mejorar el proyecto.

Al final del segundo sprint (que coincidirá con el final del proyecto y del módulo), haremos una sesión de presentación más completa, más allá de lo que sería un Sprint Review

3.2. Criterios de aceptación
Crear la infraestructura necesaria: repositorio en GitHub y con acceso para todos los miembros del equipo.

Crear al menos tres juegos de los descritos por el cliente.

Tener todos los juegos automatizados.

Tener en el repositorio de GitHub todo el código del desarrollo del proyecto.

3.3. Historias de usuario
Para la gestión del proyecto, usaremos historias de usuario. Las historias de usuario son descripciones breves y concretas de las funcionalidades o características que un usuario espera encontrar en un producto o sistema. Recordemos que, las historias de usuario son una herramienta importante para asegurarse de que el equipo de desarrollo (es decir, nosotras) entienda las necesidades de las usuarias y construya el producto de manera efectiva.

Una historia de usuario típica describe quién es el usuario, qué necesita hacer y por qué. Por ejemplo, como analista de datos, quiero poder identificar patrones y tendencias en los datos de ventas de mi empresa para poder hacer recomendaciones sobre cómo mejorar la rentabilidad. Quiero poder filtrar los datos por fecha, producto, región y otros factores relevantes, y visualizar los resultados en gráficos y tablas para poder comprender mejor los insights que se derivan de los datos. Además, quiero poder compartir fácilmente los resultados con otros miembros del equipo y exportar los datos en diferentes formatos para su posterior análisis. Si bien estas historias de usuario puede resultar un poco complejas para el tema que nos ocupa, podemos definir unas historias de usuario más claras para este proyecto, estas pueden ser:

Seleccionar los juegos que queréis incluir en vuestro proyecto. Los criterios de aceptación de esta user story son:

Elegir al menos tres de los juegos presentados por el cliente.

Desarrollar los juegos del producto pedido por el cliente

Automatizar todos los procesos en funciones y clases.

Un ejemplo completo de historias de usuario puede ser:

Historia de Usuario 1: Creación del Juego Tic-Tac-Toe

Objetivo: Como estudiante de Python, quiero desarrollar el código para crear un juego de Tic-Tac-Toe como parte de un proyecto para una empresa de videojuegos, para poner en práctica mis habilidades de programación y contribuir al desarrollo del juego.

Descripción: En el proyecto, se nos pide la tarea de crear un juego de Tic-Tac-Toe utilizando Python. La empresa de videojuegos desea agregar este juego clásico a su catálogo. Ana debe desarrollar el código fuente del juego, que incluye la lógica del juego, la interfaz de usuario y la capacidad de jugar contra la computadora o con otro jugador. Además, debe asegurarse de que el juego sea intuitivo y divertido de jugar. Una vez completado, el juego será evaluado por sus compañeras y profesores como parte de su proceso de aprendizaje.

Criterios de Aceptación:

El juego de Tic-Tac-Toe debe ser jugable por dos jugadores o contra la computadora.

Debe haber una interfaz de usuario clara y fácil de entender.

El juego debe seguir las reglas estándar de Tic-Tac-Toe.

Se deben implementar mensajes de victoria, empate y derrota.

El código debe estar bien documentado y seguir las mejores prácticas de programación en Python.

4. Entrega
El formato de entrega de este proyecto será mediante la subida de este proyecto a la plataforma de GitHub. Para subirlo, se creará un repositorio en la organización de Adalab. El nombre del repositorio deberá estar compuesto de las siguientes partes, todo ello separado por guiones:

La palabra: proyecto-da.

Letra de la promoción: promo-F.

Número del módulo: modulo-1.

Número del equipo: team-X.

Por ejemplo:

Adalab/proyecto-da-promo-F-modulo-1-team-1

Adalab/proyecto-da-promo-F-modulo-1-team-3

En lo relacionado en las fechas de los sprints:

Entrega del primer sprint (sprint review ): 13 Octubre.

Entrega del segundo sprint (sprint review): 19 Octubre.

Demo del proyecto (presentación final y retro): 24 Octubre

En las sprint review se revisará que se hayan solucionado todas las tareas técnicas asociadas a la entrega de esos sprints, si algo quedara pendiente se arrastraría al siguiente sprint.

5. Presentación
El último día del módulo presentaréis la versión final de este proyecto a vuestras compañeras y al equipo de Adalab. Cada equipo realizará una presentación de 5 minutos y posteriormente habrá 5 minutos de feedback por parte del público. En este caso, la audiencia podría ser más variada pues no sólo estarán los profesores.

El objetivo es que practiquéis la realización de las demos de los proyectos que habéis desarrollado, explicándolo desde un punto de vista técnico y también desde la perspectiva de producto, mejorando además vuestras habilidades de exposición, objetivo de desarrollo profesional del curso.

Para que la presentación salga bien es imprescindible una buena preparación. Por ello, durante el segundo sprint del módulo tendréis que asignar responsabilidades dentro del equipo relacionadas con la preparación de ésta. Algunos tips para preparaos este demo son:

Todas las participantes del equipo deben hablar en la presentación (sin práctica no hay mejora).

Identificar los objetivos de la presentación: Debemos tener claro qué es lo que queremos lograr con la presentación. ¿Queremos demostrar la funcionalidad de un producto? ¿Queremos mostrar los resultados de un experimento? ¿Queremos atraer inversores? Dependiendo del objetivo, deberemos enfocar la presentación de manera distinta.

Conoce a tu audiencia: La presentación debe estar adaptada al tipo de audiencia que se espera. Si se presentaráis ante posibles inversores, la presentación debe estar enfocada en los beneficios y la rentabilidad del producto. Si es una presentación para usuarios, deberá enfocarse en la usabilidad y la facilidad de uso.

Debéis ser claras y concisas: La presentación debe ser fácil de entender y no debe ser demasiado larga. Es importante presentar la información de manera clara y concisa. Debemos tener en cuenta que los detalles técnicos pueden ser interesantes, pero no deberían opacar la idea principal.

Demostrad la funcionalidad del producto: Si la presentación es para demostrar un producto, es importante que demostremos su funcionalidad. Podemos hacerlo mediante un video o demostrando el producto en vivo. Es importante asegurarse de que el producto funciona correctamente antes de la presentación.

Resaltad los aspectos más importantes: En cualquier presentación, hay aspectos que son más importantes que otros. Debéis resaltar los aspectos que sean más relevantes para su objetivo. Por ejemplo, si queréis atraer inversores, deberéis resaltar los beneficios y la rentabilidad del producto.

Practicad la presentación: Es importante que practiquéis la presentación varias veces antes del evento. Debéis aseguraos de que la presentación esté bien estructurada y que os sentís cómodas hablando frente a la audiencia.

Preparad respuestas a preguntas frecuentes: Es probable que la audiencia tenga preguntas después de la presentación. Debéis preparaos para responder preguntas frecuentes y tener la información necesaria a mano.

Además de esto, para mejorar vuestras habilidades de exposición en público y hacer la presentación más rica, podréis incorporar otros elementos adicionales (son solo ideas, sentíos libres de innovar y ser creativas):

Dejar muy claro quién ha sido vuestro cliente y qué fue lo que os pidió.

Explicar qué necesidades cubre o qué problemas soluciona el producto, cuál es el beneficio principal que aporta y qué lo hace único comparado con otros productos parecidos del mercado.

Aportaciones "únicas y diferenciadoras" de cada equipo al proyecto.

Cómo ha sido la organización del equipo, el reparto de tareas y la coordinación a la hora de trabajar todas en el mismo código.

Cuál de las tareas o los puntos ha sido el que más esfuerzo ha requerido.

Cuál de las tareas o partes del producto es la que hace que el equipo esté más orgulloso.

Las tecnologías qué habéis utilizado y para qué sirven, y algunas partes del código que habéis desarrollado que merezca la pena resaltar.

La presentación debe tener un "buen inicio y un buen cierre" que nos haga a todos estar atentos y aplaudir... ahí os dejamos que echéis a volar vuestra imaginación.

No habléis en primera persona de lo que habéis hecho, hablad del equipo.

No mencionéis problemas, sino "retos" que os han hecho aprender y crecer.

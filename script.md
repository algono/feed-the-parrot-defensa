# Título

Hola, me llamo Alejandro, y voy a presentarles "Al Loro: Lector de feeds RSS para asistente de voz".

# Índice

En primer lugar, este es un índice general donde se muestran las secciones que se van a tratar a lo largo de la defensa.

Para saber a qué altura de la presentación nos encontramos en cada momento, siempre habrá una línea gris visible bajo cada título que se irá rellenando de color verde conforme avancen las diapositivas.

Dicho esto, comencemos.

# Introducción

## ¿Qué es Alexa?

### Diapositiva 1

La plataforma principal en la que se basa este trabajo es Alexa. ¿Qué es Alexa?

Alexa es un asistente de voz creado por la empresa Amazon, el cual se encuentra disponible a través de una app para Android e iOS.

Sin embargo, como más se utiliza es mediante los productos de la familia Amazon Echo, dispositivos calificados como "Home assistants" o "asistentes de hogar", diseñados específicamente para utilizar el servicio de Alexa.

Un ejemplo de este tipo de dispositivos es el Echo Dot, uno de los más populares debido a su precio, más económico.
La última versión (o generación) del producto es la que se muestra en la diapositiva. También pueden verlo a mi lado en la cámara (\**mostrar Echo*\*).

### Diapositiva 2

Entre las cosas que se puede hacer con un asistente de voz como este, están: la obtención de información como el tiempo, el tráfico o las noticias; activar alarmas o recordatorios; o funcionalidades relacionadas con la domótica como encender y apagar luces, o enchufes inteligentes, entre otras cosas.

Uno de los aspectos más interesantes de Alexa como desarrollador Software es la habilidad de crear aplicaciones personalizadas (llamadas *skills*). Si son publicadas, cualquier usuario de la plataforma podrá usarlas.

Esto tiene mucho futuro a nivel de negocio, y ya se están empezando a ver estrategias de monetización como skills premium o suscripciones en grandes empresas.

# Motivación

Dicho todo esto: ¿cuál ha sido mi motivación de cara a realizar este trabajo?
Esta se ha basado principalmente en tres aspectos:

- Saber más acerca de los servicios en la nube. Se trata de un área con mucha demanda y bastante novedosa, y me resulta bastante interesante en cuanto a la infraestructura que requiere y aquello que ofrece.

- Aprender un lenguaje de programación que es bastante popular últimamente, es moderno y ha tenido muy buen recibimiento durante los últimos años: TypeScript. Está basado en JavaScript (el llamado "lenguaje de la web") y añade funcionalidades muy útiles para encontrar errores y, en general, mejorar la experiencia del desarrollador.

- De forma similar a lo anterior, introducirme en el campo de los asistentes de voz, el cual tiene un futuro muy prometedor.

# Estado del arte

## Asistentes de voz más populares

Ahora vamos a echar un vistazo al mercado actual de los asistentes de voz, y a hacer una comparativa entre ellos.

Los asistentes de voz más conocidos son: el Asistente de Google, Amazon Alexa, y Siri (de la empresa Apple).

## Asistente de Google

### Ventajas

En primer lugar, veamos el Asistente de Google.

Entre sus ventajas se encuentran:

- su popularidad;

- el hecho de que venga instalado por defecto en Android;

- y su sistema de búsqueda por internet, que destaca sobre el resto (lo cual tiene sentido porque la empresa que lo creó, Google, es conocida por tener el buscador más importante del mundo).

### Kit de desarrollo

Su kit de desarrollo para crear aplicaciones se llama "Google Actions", y tiene un mayor enfoque a desarrolladores principiantes.

Esto se puede ver en el hecho que su principal herramienta para programar está basada en modelos mediante diagramas, lo cual hace el proceso más visual.

Como los modelos de diagramas pueden ser demasiado simples para según qué aplicaciones, existe la funcionalidad de *webhooks*, que permite crear programas externos que se comuniquen con la aplicación. 

## Amazon Alexa

### Ventajas

En segundo lugar, se encuentra Amazon Alexa.

Sus puntos fuertes son:

- su popularidad entre los dispositivos "Smart Home", los asistentes de hogar que hemos visto antes;

- la capacidad de integración con otras plataformas, que es superior al resto porque Amazon se ha enfocado mucho en eso;

- y la mayor inversión en su sistema de skills, lo cual está muy relacionado con el punto anterior.

### Inconvenientes

Sin embargo, tiene un principal inconveniente: su sistema de búsqueda por internet es significativamente peor que el de los demás.

Un estudio del año 2020 reveló que no era capaz de responder a un 23% de las preguntas que se le hacían, mientras que el porcentaje de error del resto de asistentes probados era menor del 10%.

### Kit de desarrollo

Su kit de desarrollo, Alexa skills, tiene una curva de aprendizaje mayor que el asistente de Google, pero menor que Siri.

Como el principal objetivo de Amazon es que un gran número de grandes empresas integre sus sistemas con Alexa mediante la creación de skills, su principal enfoque es la facilidad de uso para quien trabaja en desarrollo web: un mercado enorme que comparte muchas tecnologías con los asistentes de voz; ya que, al fin y al cabo, la infraestructura de estos últimos está basada en servicios web.

Para ello, da soporte a lenguajes muy utilizados en este campo: JavaScript y Python.

## (Apple) Siri

### Ventajas

Por último tenemos a Siri.

- Su principal ventaja es que es muy querido entre los usuarios de productos Apple, que es donde se encuentra disponible.

- También tiene una mayor integración con las apps para iOS, ya que es el sistema operativo de Apple.

- Y su mayor enfoque es la productividad: aumentar la rapidez para realizar tareas repetitivas, especialmente entre sus dispositivos móviles.

### Inconvenientes

Los inconvenientes que tiene están íntimamente relacionados con las ventajas:

- En primer lugar, Siri sólo está disponible para productos Apple. Aunque es una estrategia similar a la de Google con su asistente, para Siri resulta una mayor desventaja debido a la menor cuota de mercado de estos productos frente a sistemas como Android.

- En segundo lugar, las aplicaciones personalizadas requieren una app para iOS asociada. Esto lleva a una mayor integración como vimos antes, pero lleva a una gran falta de flexibilidad.

- Por último, desarrollar aplicaciones para Siri es más complejo que para el resto de asistentes. Ahora veremos los motivos con más detalle al hablar de su kit de desarrollo, llamado SiriKit.

### Kit de desarrollo

SiriKit, como acabamos de ver, está muy ligado al sistema iOS.

Por este motivo, es más difícil para nuevos desarrolladores introducirse en el desarrollo de aplicaciones para Siri.

De hecho, los requisitos sólo para empezar son **muy** específicos:

- Uno debe saber sobre el lenguaje de programación *Swift*, el cual se usa mayoritariamente en el desarrollo de servicios para productos de Apple;

- Y el desarrollador debe haber adquirido un ordenador de la familia *Mac* para tener acceso al editor *XCode*, el cual es necesario para poder crear aplicaciones para iOS.

## Tabla comparativa

Para resumir esta sección, tenemos una tabla comparativa de los tres asistentes, donde se comparan:

- El kit de desarrollo que utiliza cada uno,

- qué lenguajes de programación soportan,

- en qué plataformas están disponibles,

- y su mayor enfoque de cara a ser competitivo frente al resto.

# Propuesta de solución

El principal objetivo de este trabajo es crear un puente entre la creación de skills en Alexa y el desarrollo de aplicaciones en otras áreas más consolidadas.
Para ello, se busca profundizar en aquellos aspectos que los unen:

- Los puntos en común con el desarrollo *backend* (una especialidad dentro del desarrollo web);

- y cómo integrar una skill con otros servicios, como apps, bases de datos, etcétera.

Sin embargo, también es importante mostrar aquello que diferencia a los asistentes de voz: la interfaz, basada en comandos activados por voz, y con un gran hincapié en la comunicación fluida y el modelo pregunta-respuesta.

## Creación de una skill

Para ello, se va a implementar una skill que sirva de ejemplo e incluya todo lo comentado anteriormente: Al Loro.

Se trata de una skill cuyo objetivo será mejorar la integración del sistema de noticias de Alexa con los servicios web de noticias que existen.

## Sistema de noticias de Alexa

Para entender un poco mejor el problema que Al Loro trata de resolver, hay que explicar en qué consiste el sistema de noticias de Alexa.

Mediante este sistema, los administradores de las plataformas de noticias pueden incluir un enlace a una página web con una feed, que es un listado con un formato especial estandarizado para contenido que se actualiza cada cierto tiempo como son las noticias, y Alexa crea automáticamente una skill que lee los artículos en orden.

Los formatos que soporta son dos:

### RSS

- El primero es RSS, que era un formato popular a principios de los 2000 y está muy extendido, pero ahora está en desuso y las webs no suelen mantenerlo. A pesar de esto, como es el que considero que tiene más posibilidades de resurgir porque muchas webs ya tienen una implementación básica, es el formato que utiliza "Al Loro".

### JSON

- Y el segundo es JSON, que aunque es el recomendado por Alexa, su uso para este caso concreto no está extendido como el anterior, y debe implementarse a propósito para poder utilizarse con Alexa. No creo que muchas webs de noticias estén dispuestas a hacer eso.

### Conclusión

En resumen, que como el primer formato está en desuso y el segundo requiere un trabajo extra, es muy complicado encontrar webs de noticias que funcionen bien con este sistema. Además, el usuario depende de los creadores de cada web para que incluyan soporte para Alexa, y no creo que eso tenga mucho sentido, sobretodo teniendo en cuenta que el campo de los asistentes de voz es relativamente nuevo y poco explorado.
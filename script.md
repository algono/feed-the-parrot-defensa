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

- Similar a lo anterior, introducirme en el campo de los asistentes de voz; que como ya he comentado antes, tiene un futuro muy prometedor.

# Estado del arte

## Asistentes de voz más populares

Ahora vamos a echar un vistazo al mercado actual de los asistentes de voz, y a hacer una comparativa entre ellos.

Los asistentes de voz más conocidos son: el Asistente de Google, Amazon Alexa, y Siri (de la empresa Apple).

## Asistente de Google

### Ventajas

En primer lugar, veamos el Asistente de Google.

Entre sus ventajas se encuentran: su popularidad; el hecho de que venga instalado por defecto en Android; y su sistema de búsqueda por internet, que destaca sobre el resto (lo cual tiene sentido porque la empresa que lo creó, Google, es conocida por tener el buscador más importante del mundo).

### Kit de desarrollo

Su kit de desarrollo para crear aplicaciones se llama "Google Actions", y tiene un mayor enfoque a desarrolladores principiantes.

Esto se puede ver en el hecho que su principal herramienta para programar está basada en modelos mediante diagramas, lo cual hace el proceso más visual.

Como los modelos de diagramas pueden ser demasiado simples para según qué aplicaciones, existe la funcionalidad de *webhooks*, que permite crear programas externos que se comuniquen con la aplicación. 

# TODO: ADAPTAR AL NUEVO LAYOUT
## ¿Qué es una feed?

### Diapositiva 1

El siguiente concepto clave que es necesario comentar es el de las feeds. Se tratan de listas disponibles en páginas web asociadas a noticias, blogs, podcasts... aquel tipo de contenido que esté basado en artículos que se añaden cada cierto tiempo.

El objetivo de tener un servicio de feeds es que los usuarios tengan un sistema centralizado donde gestionar todas sus noticias fácilmente. 

Por desgracia, este servicio ha caído en desuso debido a las redes sociales, siendo su pico de popularidad durante los años 90 y principios de los 2000; pero aún está disponible en muchos sitios web que o son antiguos o utilizan servicios para mostrar sus artículos que crean feeds por defecto.

### Diapositiva 2

A pesar de todo esto, Alexa hace uso de las feeds en su sistema de noticias (probablemente por su presencia extendida y facilidad para integrar con otros servicios).
En él, los administradores de las plataformas de noticias pueden incluir un enlace a una feed, y Alexa crea automáticamente una skill que lee los artículos en orden.

Los formatos de feed que soporta son:

- RSS, que es del que hace uso la skill que he desarrollado para este trabajo, "Al Loro";
- y JSON, que aunque es el recomendado por Alexa, su uso no está extendido como el anterior, y debe implementarse a propósito para poder utilizarse con Alexa.
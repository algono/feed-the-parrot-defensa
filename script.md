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
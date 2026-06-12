# Libro Blanco de PlaneSight

## Investigación Experimental sobre Esteganografía, Valor Digital y Propiedad Vinculada a Medios Digitales

**Versión:** Experimental v0.9.1  
**Autor:** Christian Blaze  
**Licencia:** MIT License

---

# Resumen

PlaneSight es una plataforma experimental de código abierto dedicada a investigar la intersección entre la esteganografía, los medios digitales, la criptografía y el valor digital.

El proyecto comenzó como una prueba de concepto destinada a explorar si una clave privada de Bitcoin podía incrustarse dentro de una imagen y recuperarse posteriormente. Con el tiempo, esta idea evolucionó hacia una iniciativa de investigación más amplia enfocada en comprender cómo la información puede ocultarse, preservarse y codificarse de forma redundante en múltiples tipos de medios digitales.

PlaneSight explora técnicas diseñadas para sobrevivir transformaciones como compresión JPEG, redimensionamiento, conversión de formatos, filtrado y manipulación de metadatos, mientras investiga simultáneamente si los propios medios digitales pueden convertirse en portadores de valor criptográfico.

Este documento describe la motivación, arquitectura, objetivos de investigación, métodos experimentales y direcciones futuras del proyecto.

---

# Introducción

Los medios digitales pueden copiarse infinitamente a un costo prácticamente nulo.

Imágenes, audio, video y documentos pueden duplicarse sin degradación, lo que plantea desafíos relacionados con la escasez digital, la propiedad y la preservación.

Al mismo tiempo, sistemas criptográficos como Bitcoin permiten que exista valor digital independiente de autoridades centralizadas.

PlaneSight explora la posibilidad de conectar estos dos mundos.

La pregunta central es:

> ¿Pueden los medios digitales contener valor criptográfico de manera directa?

El proyecto no pretende responder esta pregunta de forma definitiva. En cambio, proporciona una plataforma para la experimentación y la investigación.

---

# Origen del Proyecto

PlaneSight nació a partir de un sencillo experimento mental.

Una billetera Bitcoin podría crearse y recibir fondos. La clave privada que controla dicha billetera podría posteriormente ocultarse dentro de una imagen utilizando técnicas de esteganografía.

Quien lograra recuperar la clave tendría acceso al bitcoin asociado.

Este concepto reveló inmediatamente una serie de desafíos interesantes:

- ¿Cómo puede sobrevivir la información oculta a transformaciones de imágenes?
- ¿Cuánta información puede ocultarse?
- ¿Cómo puede permanecer visualmente indetectable?
- ¿Pueden combinarse múltiples métodos de codificación independientes?
- ¿Puede un medio digital convertirse en un instrumento portador de valor?

Estas preguntas se convirtieron en la base de PlaneSight.

---

# Objetivos del Proyecto

## Objetivo 1: Investigación en Esteganografía

Investigar métodos prácticos para incrustar información dentro de medios digitales minimizando su detección.

## Objetivo 2: Resistencia a Transformaciones

Estudiar si la información oculta puede sobrevivir:

- Compresión JPEG
- Redimensionamiento
- Escalado
- Filtrado
- Conversión de formatos
- Eliminación de metadatos

## Objetivo 3: Codificación Multicapa

Explorar si una misma carga útil puede codificarse de forma redundante mediante múltiples técnicas independientes.

## Objetivo 4: Valor Vinculado a los Medios

Investigar mecanismos mediante los cuales los medios digitales puedan transportar valor criptográfico.

---

# Arquitectura Actual

PlaneSight funciona actualmente como un marco experimental de investigación en esteganografía más que como un único algoritmo de codificación.

Los métodos actualmente investigados incluyen:

- PNG Stealth
- JPEG Resilient
- Resize Lab
- Scale Lab
- DCT Lab
- Wavelet Lab
- Watermark Lab
- Incrustación en Metadatos

Múltiples métodos pueden combinarse simultáneamente para evaluar compatibilidad y resiliencia.

---

# Codificación Multicapa

La esteganografía tradicional suele depender de un único mecanismo de ocultamiento.

PlaneSight explora un modelo diferente.

La misma carga cifrada podría codificarse simultáneamente en:

- Valores de píxeles
- Coeficientes de frecuencia
- Metadatos
- Estructuras de marcas de agua
- Futuras pistas de audio
- Futuras pistas de video

La redundancia puede aumentar la probabilidad de recuperación después de transformaciones o daños.

---

# Medios Respaldados por Bitcoin

Una de las áreas de investigación consiste en vincular medios digitales con valor en Bitcoin.

Un flujo conceptual podría ser:

1. Crear una billetera Bitcoin.
2. Financiar la billetera.
3. Cifrar la clave privada.
4. Incrustar la carga cifrada dentro del medio.
5. Distribuir el medio.

La posesión del medio podría proporcionar una vía para recuperar el valor asociado.

Este concepto sigue siendo experimental y no debe interpretarse como un método seguro de custodia de Bitcoin.

---

# Gestión de Derechos Mediante Multifirma

PlaneSight también explora la posibilidad de combinar la distribución de medios con billeteras Bitcoin multifirma.

En un modelo conceptual:

- Una clave de firma se encuentra incrustada dentro del medio.
- Otra clave de firma es controlada por el emisor o distribuidor.

La posesión del medio por sí sola no otorgaría acceso inmediato al bitcoin asociado.

El distribuidor podría participar en la firma de transacciones bajo condiciones predefinidas.

Algunos ejemplos incluyen:

- Canje con bloqueo temporal
- Cronogramas de liberación gradual
- Incentivos por conservación a largo plazo
- Sistemas de verificación de propiedad
- Programas de recompensas para coleccionistas

Por ejemplo, un emisor podría acordar liberar el valor total asociado únicamente después de cinco años.

Si el rescate se realiza antes, podría liberarse solamente una parte del valor.

Tales mecanismos podrían incentivar la preservación del medio digital en lugar de su redistribución indiscriminada.

---

# Investigación Futura en Audio y Video

Actualmente PlaneSight se enfoca principalmente en imágenes.

Las futuras investigaciones podrían explorar:

## Incrustación en Audio

Codificación de información cifrada en:

- Bandas de frecuencia
- Información de fase
- Señales de espectro expandido

## Incrustación en Video

Codificación de información dentro de:

- Fotogramas de video
- Vectores de movimiento
- Coeficientes de frecuencia
- Estructuras de metadatos

## Redundancia Multimedios

Una misma carga cifrada podría existir simultáneamente en:

- Imágenes
- Audio
- Video
- Metadatos

Una visión a largo plazo consiste en que un mismo secreto cifrado pueda existir simultáneamente en la información visual, la información de audio, los metadatos y los componentes de frecuencia de un archivo multimedia.

---

# Consideraciones de Seguridad

PlaneSight es experimental.

Ningún método de codificación actualmente implementado debe considerarse adecuado para almacenar:

- Bitcoin
- Claves privadas
- Contraseñas
- Comunicaciones sensibles
- Secretos de alto valor

Los usuarios deben asumir que la información oculta puede perderse, ser detectada o volverse irrecuperable.

---

# Filosofía de Investigación

PlaneSight no es simplemente un proyecto de esteganografía.

Es una exploración de cómo los medios digitales pueden convertirse en algo más que contenido.

La visión consiste en explorar si los medios digitales pueden evolucionar hacia una nueva clase de activo digital capaz de transportar valor, propiedad e información criptográfica.

---

# Descargo de Responsabilidad

PlaneSight es un proyecto de investigación.

Nada de lo descrito en este documento debe interpretarse como asesoría financiera, asesoría de seguridad o una recomendación para almacenar cantidades significativas de Bitcoin utilizando este software.

El proyecto es experimental y se proporciona exclusivamente con fines educativos y de investigación.

---

# Licencia

PlaneSight se distribuye bajo la licencia MIT.

Consulte el archivo LICENSE para más detalles.

---

*Prueba de concepto creada por Christian Blaze.*
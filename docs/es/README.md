# PlaneSight

## Idiomas

- 🇪🇸 Español (este documento)
- 🇺🇸 [English](../../README.md)

## Documentación

- 📚 [Índice de Documentación](README-INDEX.md)

---

**PlaneSight** es una plataforma experimental y de código abierto para la investigación de esteganografía, enfocada en ocultar información dentro de medios digitales mientras explora la resistencia a transformaciones como compresión JPEG, redimensionamiento, filtrado y conversión de formatos.

Originalmente concebido como una prueba de concepto para incrustar claves privadas de Bitcoin dentro de imágenes, PlaneSight ha evolucionado hacia un entorno de investigación para probar múltiples técnicas de esteganografía y explorar nuevas formas de asociar valor digital con medios digitales.

---

# Visión

La inspiración original para PlaneSight surgió de una pregunta simple:

> ¿Se puede ocultar Bitcoin dentro de una imagen?

La idea consistía en crear una billetera Bitcoin, depositar bitcoin en ella y codificar la clave privada dentro de una imagen.

Con el tiempo, este concepto evolucionó hacia una exploración más amplia sobre cómo los medios digitales y el valor digital podrían estar conectados.

---

# Características Actuales

- Codificación PNG Stealth
- Codificación JPEG Resilient
- Experimentos de Resize Lab
- Experimentos de Scale Lab
- Experimentos DCT (dominio de frecuencia)
- Experimentos Wavelet
- Experimentos de Watermark
- Codificación en metadatos
- Capas múltiples de codificación
- Verificación de compatibilidad

---

# Objetivos de Investigación

PlaneSight investiga varias preguntas:

## ¿Puede la información oculta sobrevivir transformaciones de medios?

Ejemplos:

- Conversión PNG → JPEG
- Redimensionamiento
- Recompresión
- Eliminación de metadatos
- Edición de imágenes

## ¿Se pueden combinar múltiples métodos de esteganografía?

PlaneSight permite experimentar con múltiples técnicas simultáneamente y verificar si interfieren entre sí.

## ¿Pueden los medios digitales transportar valor?

Una dirección de investigación a largo plazo es explorar si los medios digitales pueden contener secretos criptográficos que incentiven su preservación y almacenamiento.

---

# Descargo de Responsabilidad

PlaneSight es un proyecto experimental de investigación.

No debe utilizarse para almacenar cantidades significativas de Bitcoin ni información sensible.

---

# Licencia

Este proyecto se distribuye bajo la licencia MIT.

Consulte el archivo LICENSE para más detalles.

---

*Prueba de concepto creada por Christian Blaze.*
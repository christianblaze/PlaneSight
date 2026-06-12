# Métodos de PlaneSight

PlaneSight es una plataforma experimental de investigación en esteganografía que explora múltiples técnicas para incrustar información dentro de medios digitales.

Cada método implica distintos compromisos entre:

- Capacidad
- Invisibilidad
- Resistencia a JPEG
- Resistencia al redimensionamiento
- Complejidad computacional
- Fiabilidad de recuperación

Este documento proporciona una descripción general de cada método actualmente implementado o en investigación.

---

# PNG Stealth

PNG Stealth se centra en la incrustación visualmente discreta.

El objetivo es realizar modificaciones difíciles de detectar por observadores humanos mientras se mantiene una recuperación fiable desde el archivo PNG original.

## Ventajas

- Alta capacidad
- Artefactos visuales mínimos
- Codificación y decodificación rápidas

## Limitaciones

- Frágil frente a conversión a JPEG
- Frágil frente a redimensionamiento
- Frágil frente a filtros y edición

---

# JPEG Resilient

JPEG Resilient está diseñado para sobrevivir a la recompresión JPEG.

En lugar de depender únicamente de valores exactos de píxel, introduce modificaciones más robustas capaces de resistir compresión moderada.

## Ventajas

- Mejor supervivencia ante JPEG
- Recuperación fiable bajo compresión moderada

## Limitaciones

- Menor capacidad
- Modificaciones potencialmente más visibles
- No diseñado para redimensionamientos agresivos

---

# Resize Lab

Resize Lab es un sistema experimental diseñado para investigar si la información oculta puede sobrevivir a operaciones de escalado y redimensionamiento.

Utiliza regiones normalizadas en lugar de posiciones absolutas de píxeles.

## Ventajas

- Potencial resistencia al redimensionamiento proporcional
- Permite experimentos de redundancia

## Limitaciones

- Experimental
- Capacidad limitada
- Puede introducir artefactos visibles
- Actualmente poco fiable frente a transformaciones agresivas

---

# Scale Lab

Scale Lab explora enfoques alternativos para codificación resistente a cambios de escala.

El objetivo es determinar si la información oculta puede recuperarse después de que una imagen haya sido redimensionada.

## Ventajas

- Potencial resistencia futura a escalado
- Plataforma de investigación para codificación independiente de escala

## Limitaciones

- Experimental
- En desarrollo activo

---

# DCT Lab

DCT (Discrete Cosine Transform) Lab explora la incrustación en el dominio de frecuencia.

JPEG utiliza internamente la Transformada Discreta del Coseno, por lo que este enfoque resulta atractivo para futuras técnicas resistentes a JPEG.

## Ventajas

- Potencial resistencia a JPEG
- Incrustación en dominio de frecuencia

## Limitaciones

- Experimental
- Restricciones de capacidad
- Requiere técnicas adicionales de sincronización

---

# Wavelet Lab

Wavelet Lab explora la incrustación de información dentro de coeficientes wavelet.

Las técnicas basadas en wavelets son ampliamente utilizadas en investigación de marcas de agua digitales.

## Ventajas

- Representación multi-escala
- Potencial robustez frente a transformaciones

## Limitaciones

- Experimental
- Fiabilidad todavía en investigación

---

# Watermark Lab

Watermark Lab explora técnicas ligeras de marcas de agua digitales.

El objetivo es introducir patrones detectables sin alterar significativamente la apariencia visual.

## Ventajas

- Ligero
- Bajo costo computacional

## Limitaciones

- Menor capacidad
- No diseñado para grandes cantidades de información

---

# Incrustación en Metadatos

Este método almacena información dentro de los metadatos de la imagen en lugar de modificar directamente los píxeles.

## Ventajas

- Alta fiabilidad mientras los metadatos permanezcan intactos
- Sin modificaciones visuales

## Limitaciones

Los metadatos pueden ser eliminados por:

- Redes sociales
- Editores de imágenes
- Capturas de pantalla
- Exportaciones o conversiones

---

# Codificación Multicapa

Uno de los principales objetivos de investigación de PlaneSight es permitir que la misma carga cifrada sea almacenada simultáneamente utilizando múltiples métodos independientes.

Por ejemplo:

- Metadatos
- Píxeles
- Dominio de frecuencia
- Marcas de agua
- Futuro audio
- Futuro video

Al almacenar la misma información cifrada en múltiples ubicaciones, el sistema podría lograr mayor resistencia frente a daño, compresión o modificaciones.

---

# Investigación Futura

Las futuras versiones de PlaneSight podrían investigar:

- Esteganografía de audio
- Esteganografía de video
- Codificación de video en dominio de frecuencia
- Sistemas multimedia respaldados por Bitcoin
- Gestión de derechos mediante multifirma
- Almacenamiento criptográfico multicapa
- Medios auto-verificables
- Sistemas distribuidos de recuperación

---

# Estado Experimental

PlaneSight es un proyecto de investigación.

Todos los métodos descritos en este documento deben considerarse experimentales, salvo que se indique explícitamente lo contrario.

Actualmente ninguno de estos métodos debe utilizarse para almacenar secretos valiosos o cantidades significativas de Bitcoin.
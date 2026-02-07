# Laboratorio: Comparación entre tecnología TTL y CMOS

## Descripción general

En este laboratorio se estudiará el comportamiento **lógico y físico real** de compuertas digitales pertenecientes a las familias **TTL** y **CMOS**. A diferencia de un enfoque puramente ideal, esta práctica busca que el estudiante comprenda que las compuertas lógicas son **dispositivos físicos**, limitados por parámetros eléctricos como corriente, potencia, velocidad y capacidad de carga.

El laboratorio se divide en **dos partes claramente diferenciadas**:

- **Parte 1:** Análisis físico y verificación lógica en tecnología **TTL**
- **Parte 2:** Comparación física con tecnología **CMOS**

La sesión de laboratorio tiene una duración total de **dos (2) horas**, por lo que **todos los montajes deberán estar previamente construidos**.

---

## Contenido

1. [Introducción](#introducción)  
2. [Objetivos](#objetivos)  
3. [Estructura del laboratorio](#estructura-del-laboratorio)  
4. [Trabajo previo obligatorio](#trabajo-previo-obligatorio)  
5. [Recursos requeridos](#recursos-requeridos)  
6. [Procedimiento experimental](#procedimiento-experimental)  
7. [Entregables](#entregables)  
8. [Referencias](#referencias)  
9. [Material de apoyo](#material-de-apoyo)

---

## Introducción

Las familias lógicas TTL (Transistor-Transistor Logic) y CMOS (Complementary Metal-Oxide Semiconductor) representan dos enfoques tecnológicos distintos para la implementación de circuitos digitales. Mientras que TTL se basa en transistores bipolares, ofreciendo buena velocidad y robustez, CMOS emplea transistores MOS complementarios, caracterizándose por su bajo consumo de potencia y alta impedancia de entrada.

En esta práctica se analizarán estas tecnologías desde dos niveles:

- **Nivel lógico:** verificación experimental de tablas de verdad.
- **Nivel físico:** mediciones reales de respuesta en frecuencia, fan-out, tiempos de conmutación y consumo de potencia.

El objetivo es que el estudiante relacione el comportamiento ideal aprendido en teoría con las limitaciones físicas reales de los dispositivos.

---

## Objetivos

- Analizar experimentalmente el comportamiento físico de compuertas TTL.
- Verificar tablas de verdad de compuertas AND y OR mediante implementación física.
- Evaluar parámetros reales de la compuerta NOT: respuesta en frecuencia, fan-out y consumo de potencia.
- Comparar el comportamiento físico de tecnologías TTL y CMOS.
- Comprender el impacto de la tecnología en el diseño de sistemas digitales reales.

---

## Estructura del laboratorio

El laboratorio se divide en **dos partes**, desarrolladas dentro de 2 sesiónes de **dos (2) horas**:

### Parte 1 – Tecnología TTL
- Análisis físico de la compuerta NOT TTL.
- Implementación lógica de compuertas AND y OR.
- Verificación experimental de tablas de verdad.
- Discusión de limitaciones físicas.

### Parte 2 – Tecnología CMOS
- Repetición del análisis físico usando compuertas CMOS.
- Comparación directa con resultados obtenidos en TTL.
- Discusión de ventajas y desventajas tecnológicas.

---

## Trabajo previo obligatorio



### 1. Análisis teórico y simulación

Antes del laboratorio, el estudiante deberá:

- Consultar las hojas de datos de:
  - 74LS04 (TTL)
  - CD4069 (CMOS)
- Comparar parámetros eléctricos y realizar una tabla con los parametros:
  - $V_{IH}$, $V_{IL}$, $V_{OH}$, $V_{OL}$
  - Corrientes de entrada y salida
  - Retardo de propagación
- Dibujar el circuito equivalente interno de la compuerta NOT.
- Calculos de potencia de la salida. 
- Simular en SPICE:
  - Función de transferencia $V_{out}$ vs $V_{in}$
  - Respuesta ante señales de distinta frecuencia (recomendacion 5 frecuencias entre 1 khz y 1 Mhz)
  - Consumo de potencia aproximado

### 2. Preparación previa de los montajes

Con el fin de aprovechar adecuadamente las **dos (2) horas del laboratorio**, **todos los circuitos deberán estar previamente armados**.

El estudiante deberá llegar al laboratorio con:

- Circuito de prueba de la **compuerta NOT TTL** listo para mediciones.(Practica 1)
- Circuitos **AND y OR** implementados con:
  - Pulsadores como entradas lógicas (Practica 1)
  - Relés de 5 V como elementos de conmutación (Practica 1)
- Montajes con compuertas **AND y OR TTL** completamente funcionales. (Practica 1)
- Circuito equivalente para la compuerta NOT CMOS preparado.(Practica 2)

Durante la sesión **no se destinará tiempo al armado desde cero** de los circuitos, sino exclusivamente a la **verificación, medición y análisis**.

---

## Recursos requeridos

### Dispositivos
- 74LS04 (NOT TTL)
- 74LS08 (AND TTL)
- 74LS32 (OR TTL)
- CD4069 (NOT CMOS)

### Implementación
-  2 Pulsadores
- 2 Relés de 5 V
- Resistencias de 1 ohm
- potenciometro de 100 ohms
- LEDs indicadores

### Instrumentación
- Fuente de alimentación de 5 V
- Generador de funciones
- Osciloscopio
- Multímetro

### Software
- LTSpice u otro simulador compatible
- Modelos SPICE de los dispositivos

---

## Procedimiento experimental

> **Nota importante:**  
> Dado que la sesión de laboratorio tiene una duración de **dos (2) horas**, se asume que todos los circuitos han sido previamente armados. El tiempo en laboratorio se dedicará exclusivamente a la **verificación funcional, mediciones experimentales y análisis de resultados**.

---

### Parte 1 – Análisis físico y lógico en TTL

1. Medir la función de transferencia $V_{out}$ vs $V_{in}$ de la compuerta NOT TTL.
2. Determinar experimentalmente:
   - $V_{IH}$, $V_{IL}$, $V_{OH}$, $V_{OL}$
3. Medir tiempos de subida, bajada y retardo de propagación.
4. Evaluar la respuesta en frecuencia de la compuerta.
5. Determinar el **fan-out máximo** permitido.
6. Medir el consumo de potencia estática y dinámica.
7. Verificar las tablas de verdad de las compuertas AND y OR:
   - Implementación con pulsadores y relés
   - Implementación con integrados TTL
8. Comparar comportamiento ideal vs comportamiento real.

---

### Parte 2 – Comparación física con tecnología CMOS

1. Repetir las mediciones realizadas en la Parte 1 usando la compuerta NOT CMOS.
2. Comparar:
   - Respuesta en frecuencia
   - Fan-out
   - Consumo de potencia
   - Tiempos de conmutación
3. Analizar las diferencias observadas entre TTL y CMOS.
4. Discutir implicaciones prácticas en el diseño digital.

---

## Entregables

El estudiante deberá entregar un **informe técnico** que incluya:

- Resultados de simulación y mediciones experimentales.
- Verificación de tablas de verdad.
- Comparación física entre TTL y CMOS.
- Análisis crítico de resultados.
- Conclusiones sustentadas en datos reales.

El incumplimiento del trabajo previo podrá limitar la realización completa de las mediciones.

---

## Referencias

[1] Cornell University. *EE 2301 Experiment 3: TTL and CMOS Logic*.

---

## Material de apoyo

- Modelos SPICE del 74LS04 y CD4069  
- Guía de importación de modelos en LTSpice  
- Video: niveles lógicos y consumo en familias digitales  

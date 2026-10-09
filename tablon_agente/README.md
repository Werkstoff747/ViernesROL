# DELTA GREEN // THE PROGRAM - OPERATION BOARD

![Classification](https://img.shields.io/badge/CLASSIFICATION-TOP%20SECRET-red.svg)
![Status](https://img.shields.io/badge/STATUS-ACTIVE%20OPERATION-green.svg)
![Tech](https://img.shields.io/badge/TECH-HTML5%20%2F%20JS%20%2F%20CSS-blue.svg)

Tablero táctico e interactivo de investigación criminal y conspiranoia, inspirado en la estética de **Delta Green** y *The Program*. Diseñado para que los agentes organicen sus pistas, sospechosos, vínculos y evidencias en un espacio infinito con soporte para hilos de conexión y persistencia de datos.

---

## 📋 Características Principales

* **Tablero Infinito con Paneo y Zoom:** Muévete libremente por el espacio arrastrando el fondo y haz zoom con la rueda del ratón para examinar los detalles o ver el mapa general.
* **Selector de Fondos Dinámico:** Cambia al instante entre un **Tablero de Corcho** clásico y una **Pizarra Blanca** limpia mediante la barra de herramientas.
* **Expedientes Estilo Polaroid:** Fichas personalizables con fotografía de retrato, nombre, rol/cargo y notas de inteligencia clasificadas.
* **Previsualización de Imagen a Pantalla Completa:** Al hacer clic en la foto de cualquier expediente, se amplía al 96% de la pantalla con un diseño cinematográfico y un panel inferior translúcido que muestra el **Nombre** y el **Cargo** con alto contraste.
* **Sistema de Hilos Rojos:** Conecta sospechosos mediante líneas de hilo rojo interactivo y córtalas individualmente con un solo clic si la línea de investigación se desvía.
* **Gestión de Operaciones:** Guarda tus progresos en la memoria local del navegador (`localStorage`) o exporta/importa expedientes completos mediante archivos JSON.

---

## 🛠️ Guía Detallada de Opciones y Controles

### 1. Barra de Herramientas Superior (`Toolbar`)

* **`OP: [Nombre de la Operación]`**: Permite cambiar el nombre identificativo de la investigación actual (por defecto `OPERATION-STYX`). Al guardar, se almacena de forma independiente por cada nombre de operación.
* **`Fondo`**: Selector para alternar el fondo del tablero entre:
  * *Corcho*: Estética clásica de investigación clandestina en motel/sótano.
  * *Pizarra Blanca*: Estética limpia tipo sala de guerra de agencia federal.
* **`💾 Guardar`**: Almacena el estado actual del tablero (fichas, posiciones, hilos y tipo de fondo) en la memoria local (`localStorage`) de tu navegador.
* **`📂 Cargar`**: Recupera una operación previamente guardada introduciendo su nombre en el campo `OP`.
* **`📤 Exportar JSON`**: Descarga un archivo `.json` con toda la información de la operación en tu ordenador para compartirlo o guardarlo como copia de seguridad.
* **`📥 Importar JSON`**: Carga un archivo `.json` previamente exportado para restaurar el tablero completo.
* **`Modo: [Mover / Conectar]`**: 
  * *Modo Mover*: Permite arrastrar las fichas por el tablero, hacer zoom y moverte por el lienzo.
  * *Modo Conectar / Cortar Hilo*: Permite hacer clic en dos chinchetas de diferentes fichas para tensar un hilo rojo de conspiración entre ellas. Si haces clic directamente sobre un hilo existente, podrás cortarlo y eliminarlo.
* **`➕ Añadir Ficha`**: Abre un formulario flotante para crear un nuevo expediente introduciendo la URL de la imagen, el nombre, el cargo y las notas de inteligencia.
* **`Limpiar`**: Elimina de golpe todas las conexiones de hilos rojos del tablero tras una confirmación de seguridad.

---

### 2. Gestión de Fichas (Expedientes)

Cada ficha cuenta con controles avanzados integrados directamente en su diseño:

* **Selector de Chinchetas**: En la esquina superior izquierda de cada ficha hay tres puntos de color (**Rojo, Azul y Amarillo**) para cambiar el color de la chincheta superior según la prioridad o categoría del sujeto.
* **Botón de Edición (✏️)**: Situado en la esquina superior derecha de la ficha. Abre el formulario modal para editar los datos o la imagen del expediente.
* **Botón de Destrucción (✕)**: Elimina permanentemente la ficha del tablero y desvincula todos sus hilos asociados.
* **Ampliación de Fotografía**: Al hacer clic en la fotografía en blanco y negro de la Polaroid, se activa el modo teatro a pantalla completa.

---

## 🚀 Despliegue y Uso Local

Este proyecto es una aplicación web de **archivo único (`HTML` autónomo)**. No requiere bases de datos, servidores de NodeJS ni dependencias externas.

1. Clona o descarga este repositorio.
2. Abre el archivo principal (`.html`) directamente en cualquier navegador web moderno (Chrome, Firefox, Edge, Safari).
3. ¡Empieza a investigar!

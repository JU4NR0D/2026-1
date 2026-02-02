# Instalación de Icarus-Verilog

Icarus-Verilog es un compilador *open source* para **Verilog HDL**, ampliamente utilizado en cursos de **electrónica digital** y **diseño de hardware**.  
Nos permitirá **compilar y simular** nuestros diseños digitales escritos en Verilog.

En esta guía se describe el proceso de instalación paso a paso en **Windows**.

---

## 1️⃣ Descarga del instalador

* Entramos a la página oficial de Icarus Verilog en el siguiente enlace:  
 https://bleyer.org/icarus/

![pagina_web_icarus](/Labs/figs/lab00/Icarus_windows.png)

* Descargamos la versión **subrayada** correspondiente a Windows.
* Abrimos el instalador descargado (`.exe`).

---

## 2️⃣ Proceso de instalación

* Seguimos los pasos del instalador aceptando las opciones por defecto.
* En la pestaña **Select Components**, verificamos que esté seleccionada la opción:

  **✔ Full Installation**

Esto asegura que se instalen todas las herramientas necesarias para compilar y simular diseños en Verilog.

![install](/Labs/figs/lab00/full_install_iverilog.png)

---

## 3️⃣ Configuración final

* En el paso final del instalador, colocamos **las 2 opciones activas**.

Estas opciones permiten que Icarus Verilog se ejecute correctamente desde la terminal del sistema.

![pagina_web_icarus](/Labs/figs/lab00/Instalador_icarus.png)

* Finalizamos la instalación.

---

## 4️⃣ Verificación de la instalación

Para validar que el software se instaló correctamente:

* Entramos al **Símbolo del sistema (CMD)**.
* Escribimos el siguiente comando:

```bash
iverilog -V
```
*  Si la instalación fue exitosa, se mostrará en pantalla la versión de Icarus Verilog, como se observa en la siguiente imagen.

![pagina_web_icarus](/Labs/figs/lab00/iverilog_V.png)
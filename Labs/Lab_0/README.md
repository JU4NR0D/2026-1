
# Lab 0: Instalación de herramientas

En este laboratorio nos enfocaremos en la **instalación y configuración de las herramientas esenciales** que utilizaremos a lo largo del curso para el diseño, simulación e implementación de sistemas digitales.

El correcto funcionamiento de estas herramientas será clave para el desarrollo de los laboratorios posteriores.

---

## 1️⃣ *FPGA Design Software* – Quartus  
### (Para síntesis en FPGA Cyclone IV)

Quartus es un software de diseño digital e implementación FPGA desarrollado por **Intel** (anteriormente **Altera**).  
Es ampliamente utilizado para la **síntesis**, **implementación** y **verificación** de diseños digitales en FPGAs de la familia **Cyclone**.

A continuación, se proporcionan las guías de instalación según el sistema operativo:

* [Guía de instalación (linux)](/Labs/Lab_0/Quartus_installation_guide_linux.md)  
* [Guía de instalación (Windows)](/Labs/Lab_0/Quartus_installation_guide_windows.md)

Además, se incluye un tutorial práctico de implementación:

* [Tutorial de implementación en la FPGA Cyclone IV](/Labs/Lab_0/proyectoQuartus.md)

---

## 2️⃣ Herramientas de simulación *Open Source*

Estas herramientas nos permitirán **simular y verificar** el comportamiento de los circuitos digitales antes de su implementación en hardware real.

### 2.1 Icarus Verilog

Icarus Verilog es una herramienta de **simulación de código abierto** para HDL (*Hardware Description Language*).  
Es ideal para simular y verificar diseños digitales escritos en **Verilog**, permitiendo detectar errores de diseño de manera temprana.

* [Guía de instalación (linux)](/Labs/Lab_0/iverilog_linux.md)
* [Guía de instalación (Windows)](/Labs/Lab_0/iverilog_windows.md)

---

### 2.2 Digital – Simulador de circuitos

Digital es un simulador gráfico que permite diseñar y analizar circuitos digitales de forma visual, siendo especialmente útil para la **comprensión conceptual** de los sistemas digitales.

* [Digital - Simulador de circuitos (linux)](/Labs/Lab_0/digital_linux.md)
* [Digital - Simulador de circuitos (Windows)](/Labs/Lab_0/digital_Windows.md)

---

## 3️⃣ Visual Studio Code

```Visual Studio Code``` (```VS Code```) es un editor de código ligero pero potente, desarrollado por **Microsoft**.  
Es altamente personalizable y cuenta con una amplia variedad de extensiones que lo hacen ideal tanto para el **desarrollo de software** como para **proyectos de hardware digital**.

Pasos para su instalación:

1. Descargar Visual Studio Code desde el sitio oficial:  
   👉 https://code.visualstudio.com/

2. Seguir las instrucciones del instalador para completar la instalación.

3. Una vez instalado, abrir ```VS Code``` y explorar las extensiones disponibles en el *Marketplace*, las cuales se utilizarán a lo largo del curso.

---

## 4️⃣ ```Git``` y GitHub

Git es un **sistema de control de versiones** ampliamente utilizado para gestionar proyectos de software y hardware.  
GitHub es una plataforma basada en Git que permite **alojar repositorios**, **controlar versiones** y **colaborar** en proyectos.

### 4.1 Configuración básica de Git (recomendado para Linux)

En sistemas **Linux**, el flujo de trabajo del curso se realizará principalmente utilizando Git desde la **terminal**.

Pasos iniciales:

1. Crear una cuenta en GitHub:  
   👉 https://github.com/

2. Descargar Git desde el sitio oficial:  
   👉 https://git-scm.com/

3. Seguir las instrucciones del instalador.

4. Configurar Git con el nombre de usuario y correo electrónico asociados a la cuenta de GitHub:

  ``` bash
  git config --global user.name "cuenta de usuario"
git config --global user.email correo@email.com
  ```

5. Comandos básicos que se utilizarán durante el curso:

* ```git init``` : Inicializa un repositorio.
* ```git clone <url>``` : Clona un repositorio remoto.
* ```git add <archivo>``` : Añade archivos al área de preparación.
* ```git commit -m "mensaje"``` : Guarda los cambios en el repositorio.
* ```git push``` : Sube los cambios al repositorio remoto.
* ```git pull``` : Actualiza el repositorio local con los cambios remotos.

---

### 4.2 GitHub Desktop (opción recomendada para Windows)

En **Windows**, los estudiantes pueden utilizar **GitHub Desktop**, una herramienta oficial que ofrece una **interfaz gráfica clara, intuitiva y fácil de usar**, ideal para quienes están comenzando con Git.

GitHub Desktop permite realizar las mismas acciones fundamentales que Git en terminal, pero de forma visual:
- Clonar repositorios
- Realizar *commits*
- Sincronizar cambios (*push* y *pull*)
- Revisar el historial de versiones

#### Descarga de GitHub Desktop

👉 https://desktop.github.com/

---

#### Instalación de GitHub Desktop (Mini-tutorial)

1. Descargar el instalador desde el sitio oficial.
2. Ejecutar el archivo descargado y seguir los pasos del instalador.
3. Una vez instalado, abrir **GitHub Desktop**.
4. Iniciar sesión con la cuenta de GitHub creada previamente.
5. Clonar el repositorio del curso utilizando la opción **“Clone a repository”**.

Durante el curso, se aceptará el uso de **Git por terminal (Linux)** o **GitHub Desktop (Windows)**, siempre que se mantenga un uso correcto del control de versiones.

El objetivo principal es **aprender a trabajar de forma ordenada y reproducible**, no memorizar comandos.

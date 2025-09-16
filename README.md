# Introduccion_a_Bash_y_echo

Este trabajo práctico tiene como objetivo introducirte al scripting en Bash utilizando comandos básicos de Linux.

<h3>📘 Tabla de comandos utilizados</h3>

<table border="1" cellspacing="0" cellpadding="6">
  <thead>
    <tr>
      <th>Comando</th>
      <th>Función</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><code>#!/bin/bash</code></td>
      <td>Indica que el script se ejecuta con Bash.</td>
    </tr>
    <tr>
      <td><code>echo</code></td>
      <td>Muestra texto en la terminal.</td>
    </tr>
    <tr>
      <td><code>uname</code></td>
      <td>Detecta el sistema operativo.</td>
    </tr>
    <tr>
      <td><code>date</code></td>
      <td>Muestra la fecha y hora actual.</td>
    </tr>
    <tr>
      <td><code>pwd</code></td>
      <td>Muestra el directorio actual.</td>
    </tr>
    <tr>
      <td><code>ls -la</code></td>
      <td>Lista archivos con detalles, incluyendo ocultos.</td>
    </tr>
    <tr>
      <td><code>chmod +x</code></td>
      <td>Da permisos de ejecución al script.</td>
    </tr>
    <tr>
      <td><code>read</code></td>
      <td>Permite ingresar datos desde el teclado.</td>
    </tr>
    <tr>
      <td><code>case</code></td>
      <td>Estructura condicional para evaluar el sistema operativo.</td>
    </tr>
  </tbody>
</table>

Objetivos del script:
- Familiarizarse con comandos básicos de Linux.

- Aprender a crear y ejecutar scripts en Bash.

- Detectar el sistema operativo y adaptar el comportamiento del script.

- Interactuar con el usuario mediante entrada dinámica.

- Modularizar tareas usando funciones.

- Mostrar información útil del sistema como permisos, espacio en disco y cantidad de archivos.


Procedimientos paso a paso 

1- Crear el archivo del script

nano script.sh

2- Dar permisos de ejecución

chmod +x script.sh

3- Ejecutar el script

./script.sh

4- Bonus opcional explicado
El uso de read permite que el script interactúe con el usuario. En este caso, se le pide su nombre y se lo saluda dinámicamente:

read nombre
echo "¡Mucho gusto, $nombre!"


Expansiones sugeridas (opcional para destacar)
Si querés ir más allá y mostrar tu dominio de Bash, podés agregar:

✅ Verificación de si el usuario tiene permisos de administrador (whoami)

📦 Mostrar el espacio libre en disco (df -h)

🔐 Mostrar los permisos de los archivos (stat o ls -l)

📊 Contar cuántos archivos hay en el directorio (ls | wc -l)

🧬 Crear funciones para modularizar el script

🐞 Errores comunes
Permiso denegado al ejecutar el script Solución: asegurarse de haber ejecutado chmod +x script.sh

El script no se ejecuta en Windows Solución: usar Git Bash o WSL (Windows Subsystem for Linux)

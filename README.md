# Unidad 1. Interfaz gráfica de usuario
Una Interfaz Gráfica de Usuario (GUI, por sus siglas en inglés Graphical User Interface) es el medio visual mediante el cual el usuario interactúa con un sistema informático. Utiliza elementos gráficos como ventanas, botones, menús, iconos y cuadros de texto para facilitar la comunicación entre el usuario y el programa.
En esta unidad se trabajará con Flet, un framework que permite desarrollar aplicaciones interactivas utilizando el lenguaje Python. Flet facilita la construcción de interfaces modernas mediante componentes visuales predefinidos y un modelo de programación basado en eventos, lo que permite que las aplicaciones respondan dinámicamente a las acciones del usuario.

## 1.1. Creación de interfaz Gráfica para usuarios
La interfaz gráfica de usuario o GUI (Graphic User Interface) por sus siglas en inglés se refiere a las ventanas gráficas e interactivas con las que el usuario de una aplicación puede interactuar, en lugar de utilizar sólo la ventana de comandos del sistema.
Para construir una GUI en genral se deben seguir los siguientes pasos:

**1.** Crear un contenedor superior y obtener su contenedor intermedio.

**2.** Seleccionar un gestor de esquemas para el contenedor intermedio.

**3.** Crear los componentes necesarios.

**4.** Agregar los componentes al contenedor intermedio.

**5.** Dimensionar el contenedor superior.

**6.** Mostrar el contenedor superior.

En Flet, la interfaz se construye dentro de una función principal con los siguientes elemnetos básicos:
* **Page:** Representa la ventana principal.
* **Text:** Muestra texto.
* **TextField:** Campo para ingresar datos.
* **ElevatedButton:** Botón.
* **Row y Column:** Organizadores de componentes.
  
**Proceso de creación**
* Se define la página.
* Se crean los controles.
* Se agregan a la página con page.add().
* Se ejecuta la aplicación con ft.app().

## 1.2. Tipos de eventos
Un evento es una acción iniciada por el usuario desde la aplicación gráfica. Los eventos se pueden activar (disparar) por los diferentes elementos que componen a la GUI.
Los principales tipos de eventos son:

**Eventos de interacción**
* Presionar un botón.
* Escribir en un campo de texto.
* Seleccionar una opción en una lista.
* Marcar o desmarcar una casilla.
  
**Eventos de teclado**
* Presionar una tecla.
* Confirmar información mediante la tecla Enter.
  
**Eventos del sistema**
* Abrir o cerrar la aplicación.
* Cambiar el tamaño de la ventana.

### Eventos comunes en Flet
* **on_click:** Cuando se presiona un botón.
* **on_change:** Cuando cambia el contenido de un campo.
* **on_submit:** Cuando se presiona Enter en un campo.
* **on_hover:** Cuando el cursor pasa sobre un elemento.
* **on_focus:** Cuando un usuario entra o sale de un campo.
  
## 1.3. Manejo de eventos
El manejo de eventos es el proceso mediante el cual se define qué acción realizará el programa cuando ocurra un evento específico.
### ¿Cómo funciona en flet?

**1.** El usuario realiza una acción.

**2.** Se activa un evento.

**3.** Se ejecuta una función.

**4.** Se actualiza la interfaz con *page.update()* si es necesario.

## 1.4. Manejo de componentes gréficos de control
También llamados controles o widgets, son los elementos visuales que permiten la interacción dentro de la interfaz.

**Controles más comunes**
* Texto informativo.
* Campos de entrada de datos.
* Botones de acción.
* Listas desplegables.
* Casillas de verificación.
* Botones de selección.
* Contenedores organizadores.
  
**Propiedades**
* Valor o contenido.
* Tamaño y posición.
* Color de fondo y texto.
* Estado (habilitado o deshabilitado).
* Visibilidad.

### Controles comunes en flet
* Text
* TextField
* ElevatedButton
* Checkbox
* Radio
* Dropdown
* Container
* Image
* DataTable
  
### Propiedades comunes en flet
* value
* label
* width
* height
* color
* bgcolor
* visible
* disabled
  
# Bibliografía
* Ricci, T. I. A., Cervantes, A. N., de León Razo, J. A., & Gálvez, J. A. S. (n.d.). Interfaz Gráfica de Usuario. Unidades de Apoyo para el Aprendizaje - CUAED - UNAM. Retrieved February 23, 2026, from https://repositorio-uapa.cuaed.unam.mx/repositorio/moodle/pluginfile.php/3058/mod_resource/content/1/UAPA-Interfaz-Grafica-Usuario/index.html

* Flet. (n.d.). Introduction. Flet.dev. Retrieved February 23, 2026, from https://docs.flet.dev/



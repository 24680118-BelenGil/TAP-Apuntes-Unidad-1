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

## Ejemplo
En el siguiente link se muestra un programa aplicando lo aprendido.

https://github.com/24680118-BelenGil/TAP-U1.-Proyecto-Integrador.git
## Bibliografía
* Ricci, T. I. A., Cervantes, A. N., de León Razo, J. A., & Gálvez, J. A. S. (n.d.). Interfaz Gráfica de Usuario. Unidades de Apoyo para el Aprendizaje - CUAED - UNAM. Retrieved February 23, 2026, from https://repositorio-uapa.cuaed.unam.mx/repositorio/moodle/pluginfile.php/3058/mod_resource/content/1/UAPA-Interfaz-Grafica-Usuario/index.html

* Flet. (n.d.). Introduction. Flet.dev. Retrieved February 23, 2026, from https://docs.flet.dev/

# Unidad 2. Componentes y librerías
En el desarrollo moderno de software, la eficiencia no reside en escribir todo el código desde cero, sino en la capacidad de modularizar y reutilizar. Esta unidad explora cómo Python y el framework Flet permiten organizar aplicaciones mediante componentes y librerías. Comprender estos conceptos es fundamental para transformar scripts lineales en sistemas escalables, donde la interfaz visual y la lógica de negocio coexisten de forma ordenada y profesional.

## 2.1 Definición conceptual de componentes, paquetes/librerías.
**Componente:** Unidad independiente que encapsula funcionalidad específica y que puede ser reutilizada en distintas partes de una aplicación. Los componentes permiten dividir un sistema en elementos más pequeños, facilitando su comprensión, mantenimiento y escalabilidad.

En el caso de Python con Flet, los componentes corresponden a elementos de interfaz gráfica conocidos como controles, tales como botones, campos de texto, etiquetas y contenedores. Cada componente posee propiedades, métodos y eventos que determinan su comportamiento dentro de la aplicación.
```Python
header = ft.Text(
    "🛒 BAZARE",
    color=ft.Colors.PURPLE,
    size=30,
    weight="bold"
)
  ```
📌 Este componente:
* Muestra texto en pantalla
* Tiene propiedades como color, tamaño y estilo

**Librería:** Conjunto de funciones, clases y módulos previamente desarrollados que ofrecen soluciones a problemas comunes. Las librerías evitan la creación de código desde cero, optimizando así el tiempo de desarrollo y reduciendo la probabilidad de errores.
```Python
import flet as ft
  ```
📌 Se está utilizando la librería Flet, que permite crear toda la interfaz gráfica.

**Paquetes:** Representan una forma de organización del código, ya que agrupan múltiples módulos dentro de una estructura jerárquica. Esta facilita la gestión de proyectos grandes, promoviendo una mejor distribución de responsabilidades dentro del sistema.

## 2.2 Uso de librerías proporcionadas por el lenguaje.
Python cuenta con una amplia colección de librerías estándar que proporcionan funcionalidades esenciales, como operaciones matemáticas, manejo de fechas, generación de números aleatorios, entre otras. Estas librerías pueden ser utilizadas mediante instrucciones de importación, lo que permite integrar fácilmente sus funciones en cualquier programa.

Además de las librerías estándar, Python permite el uso de librerías externas, como Flet, que amplían significativamente las capacidades del lenguaje. Flet, en particular, permite desarrollar interfaces gráficas modernas sin necesidad de conocimientos avanzados en diseño visual, ya que proporciona componentes predefinidos que simplifican la construcción de aplicaciones.
```Python
page.add(
    header,
    catalogo
)
  ```
📌 Aquí Flet permite:
* Agregar componentes a la pantalla
* Construir la interfaz de forma dinámica
  
**Ventajas del uso de librerías**
1. Reduce tiempo de desarrollo.
2. Evita reinventar soluciones.
3. Código más limpio.
4. Mayor confiabilidad.

## 2.3 Creación de componenetes (visuales y no visuales) definidos por el usuario.
**Componentes visuales personalizados:** Permiten diseñar elementos de interfaz que combinan múltiples controles, como botones, textos y contenedores, en una sola unidad reutilizable. Esto favorece la consistencia visual y reduce la duplicación de código.
```Python
class ProductoCard(ft.Container):

    def __init__(self, producto):

        super().__init__()

        self.width = 250
        self.padding = 10
        self.border_radius = 15
        self.bgcolor = ft.Colors.WHITE
  ```
📌 Este componente:
* Hereda de Container
* Define su propio diseño
* Es reutilizable
  
**Componentes no visuales:** Clases o funciones que encapsulan la lógica del programa, como operaciones matemáticas, validaciones o procesamiento de datos. Estos componentes son fundamentales para separar la lógica de la interfaz, lo que mejora la organización del sistema.
```Python
def main(page: ft.Page):
  ```
📌 También es no visual porque:
* Controla la lógica de la app
* Organiza los componentes
  
La creación de componentes definidos por el usuario fomenta la modularidad del software, permitiendo construir aplicaciones más claras, estructuradas y fáciles de mantener.

## 2.4 Creación y uso de paquetes/librerías definidas por el usuario.
Python permite a los desarrolladores crear sus propias librerías y paquetes. Esto se logra organizando el código en módulos que pueden ser reutilizados en diferentes proyectos.

La creación de paquetes implica estructurar el código en carpetas que contienen archivos relacionados, lo que facilita su distribución y mantenimiento. Asimismo, permite dividir el sistema en diferentes capas, como interfaz, lógica y acceso a datos.

**Ventajas de crear librerías propias**
1. Reutilización de código
2. Organización clara
3. Facilita trabajo en equipo
4. Escalabilidad
```Python
productos = [
{"id": 1, "nombre": "Totoro", "descripcion": "Peluche de 1 metro de altura, suave y esonjoso.", "precio": 1000, "ruta_imagen": "1.jpg"},
{"id": 2, "nombre": "Gatitos", "descripcion": "Hermosos llaveros de gatitos", "precio": 100, "ruta_imagen": "2.webp"},
{"id": 3, "nombre": "Libreta", "descripcion": "LIbreta en forma de lapiza, rayada.", "precio": 50, "ruta_imagen": "3.webp"},
{"id": 4, "nombre": "Capibara", "descripcion":"Mochila de capibara con flor.", "precio": 200, "ruta_imagen": "4.jpg"},
{"id": 5, "nombre": "Nimona", "descripcion": "Funko de Nimona.", "precio": 500, "ruta_imagen": "5.jpg"},
{"id": 6, "nombre": "Sailor Moon", "descripcion": "Set de 6 mangas de Sailor Moon.", "precio": 2000, "ruta_imagen": "6.webp"},
{"id": 7, "nombre": "Cry baby", "descripcion": "Perfume original, sellado.", "precio": 3000, "ruta_imagen": "7.webp"},
{"id": 8, "nombre": "Van Gogh", "descripcion": "Set de notas adhesivas Noche estrellada.", "precio": 100, "ruta_imagen": "8.webp"},
]
  ```
Aunque el código está en un solo archivo, ya se aplica el concepto de organización modular.}

📌 Esto funciona como:
* Base de datos simple
* Fuente de información reutilizable
## Ejemplo
En el siguiente link se muestra un programa aplicando lo aprendido.

https://github.com/24680118-BelenGil/Proyecto-Catalogo.git
## Conclusión 
La implementación de componentes y paquetes personalizados en Flet marca la diferencia entre un prototipo simple y una aplicación robusta. Al dominar la creación de controles propios y la estructuración de librerías, el desarrollador logra un código más limpio, fácil de mantener y altamente reutilizable. En definitiva, la modularidad en Python no es solo una técnica de organización, sino una estrategia esencial para optimizar el tiempo de desarrollo y la calidad del software.
## Bibliografía
* Flet. (n.d.). Introduction. Flet.dev. Retrieved February 23, 2026, from https://docs.flet.dev/



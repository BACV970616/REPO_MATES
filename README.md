<div align="center">

# A4 - Entorno de desarrollo (Visual Studio 2026)
Asignatura: Entornos de Desarrollo.

**Ciclo:** DAW A.1

**Alumno:** BRAYAN ALEXIS CARDENAS VELLASQUEZ.
</div>


# 1. Conceptos Iniciales Previos
##  Definición de IDE
Un **IDE** (*Integrated Development Environment* o Entorno de Desarrollo Integrado) es un entorno de software que proporciona un conjunto unificado de herramientas para facilitar el desarrollo, la programación, la compilación y la depuración de aplicaciones informáticas dentro de una única interfaz gráfica centralizada.

## 2. Características generales de un IDE

1. **Editor de código fuente:** Proporciona resaltado de sintaxis, autocompletado inteligente de código y detección visual de errores en tiempo real. 
2. **Compilador / Intérprete integrado:** Permite traducir y ejecutar el programa directamente desde la interfaz sin necesidad de usar herramientas externas. 
3. **Herramientas de depuración (*Debugger*):** Facilita la inclusión de puntos de interrupción (*breakpoints*), la inspección del valor de las variables y la ejecución paso a paso para identificar errores de lógica. 
4. **Gestor de proyectos y soluciones:** Organiza la estructura de carpetas, ficheros de código, dependencias y bibliotecas del software. 
5. **Integración con control de versiones:** Ofrece soporte nativo para conectar y sincronizar el proyecto con plataformas de control de versiones como **Git** y **GitHub**.

## 3. Características más relevantes de Visual Studio
### 3a) Sistemas operativos soportados
Visual Studio está diseñado de forma nativa para el sistema operativo **Windows** (Windows 10, Windows 11 y Windows Server). Anteriormente existía una versión para macOS (*Visual Studio for Mac*), aunque actualmente Microsoft impulsa la extensión C# Dev Kit sobre **VS Code** para entornos Linux y macOS. 
### 3b) Lenguajes de programación, frameworks y definición de .NET
 * **Lenguajes compatibles:** C#, C++, F#, Visual Basic, Python, JavaScript, TypeScript, HTML/CSS, entre otros. * **Frameworks principales:** .NET (.NET Core, .NET 8/9), ASP.NET Core (desarrollo web), WPF y Windows Forms (aplicaciones de escritorio), MAUI (aplicaciones móviles y multiplataforma).  
 
 
 **¿Qué es .NET?** 
 
 **.NET** es una plataforma de desarrollo gratuita, de código abierto y multiplataforma creada por Microsoft. Proporciona un entorno de ejecución unificado (*CLR - Common Language Runtime*), bibliotecas de clases estándar y un sistema de compilación híbrido (CIL/Bytecode + compilador JIT) que permite escribir código en lenguajes como C# y ejecutarlo en distintos sistemas y arquitecturas. 
 
 ### 3c) Herramientas incluidas de serie y pasos para codificar y ejecutar
  * **Herramientas de serie:**
    * Editor de código inteligente con **IntelliSense** (autocompletado y refactorización). 
    * Compilador **MSBuild** e integradores de proyectos (`.sln` y `.csproj`). 
    * Depurador avanzado (*Debugger*) con puntos de interrupción y ventanas de inspección en vivo. 
    * Diseñador gráfico de interfaces (para WPF y Windows Forms). 
    * Gestor de paquetes **NuGet** e integración nativa con **Git/GitHub**. 
    
   
   
   * **Pasos básicos para codificar y ejecutar un programa:** 
   1. **Crear el proyecto:** Abrir Visual Studio y seleccionar una plantilla (por ejemplo, *Aplicación de consola* en C#). 
   2. **Escribir el código:** Editar los archivos de código fuente (como `Program.cs`) en el editor principal. 
   3. **Compilar el proyecto:** Ir al menú *Compilar &gt; Compilar solución* (o pulsar `Ctrl + Mayús + B`) para comprobar que no existan errores de sintaxis. 
   4. **Ejecutar el programa:** Pulsar el botón **Iniciar** (flecha verde), o usar el atajo `F5` (con depuración) o `Ctrl + F5` (sin depurar) para abrir la consola y ver el resultado. 
   ### 3d) Coste del software 
   Existe una versión completamente **gratuita** (*Community Edition*) orientada a estudiantes, colaboradores de código abierto y desarrolladores individuales. Para empresas y uso corporativo existen versiones comerciales de pago (*Professional* y *Enterprise*). 
   ### 3e) Número y fecha de la versión actual 
   En el contexto de la práctica se trabaja con la versión **Visual Studio 2026**. 
   ### 3f) Tipo de licencia de desarrollador 
   Ofrece una **licencia Community (gratuita para uso individual y académico)** que requiere iniciar sesión con una cuenta de Microsoft para su activación gratuita, y **licencias por suscripción de pago** (*Professional / Enterprise*) destinadas a entornos profesionales y corporativos.
   
   ## 4. Pasos para crear una Aplicación de Consola en C# y versión de .NET
   ### Pasos para crear una Aplicación de Consola en Visual Studio 2026:
   1. **Abrir Visual Studio 2026** y seleccionar la opción **Crear un proyecto** (*Create a new project*) en la pantalla de inicio.
   2. **Filtrar la plantilla:**
        * **Lenguaje:** C# 
        * **Plataforma:** Windows (o Todas las plataformas) 
        * **Tipo de proyecto:** Consola
   3. Seleccionar la plantilla **Aplicación de consola** (*Console App*) y hacer clic en **Siguiente**.
   4. **Configurar el proyecto:**
        * **Nombre del proyecto:** Escribir el nombre deseado (por ejemplo, `MatesConsola`). 
        * **Ubicación:** Elegir la ruta del directorio de trabajo (*workspace*). 
        * **Nombre de la solución:** Definir el nombre del contenedor de la solución (por ejemplo, `MATES_NOM`).
   5. **Información adicional:** Seleccionar la versión del marco de trabajo (.NET) y hacer clic en **Crear**.
   ---
   ### Versión actual de .NET: 
   * La versión de desarrollo estándar multiplataforma actual de la plataforma es **.NET 9.0 / .NET 10.0** (según el SDK instalado en el equipo), sustituyendo progresivamente a las versiones antiguas de .NET Framework.

   ## 5. Ventanas y paletas principales de Visual Studio 2026
   ### 5.1. Descripción de las ventanas principales
   * **Explorador de soluciones (*Solution Explorer*):** 
        * **Función:** Muestra la estructura jerárquica del proyecto, permitiendo navegar entre los archivos de código, dependencias, referencias y configuraciones. 
        * **¿Qué es una Solución?** Es el contenedor principal (archivo `.sln`) que agrupa y organiza uno o varios proyectos relacionados para que puedan trabajar juntos. 
        * **¿Qué es un Proyecto?** Es un conjunto de archivos de código fuente, recursos y configuraciones (archivo `.csproj`) que se compilan para generar un producto concreto (como una biblioteca de clases `.dll` o un ejecutable `.exe`).
* **Editor de código:** 
    * **Función:** Es la ventana central donde se escribe y modifica el código fuente de los archivos (por ejemplo, `Program.cs`). Ofrece resaltado de sintaxis, autocompletado (IntelliSense) y detección de errores.
* **Consola de compilación (*Ventana de Salida / Output*):** 
    * **Función:** Muestra los mensajes generados por el compilador durante el proceso de construcción (*build*), indicando si la compilación ha sido exitosa o detallando los errores y advertencias de sintaxis detectados.
* **Ventanas de depuración (*Debugger*):** 
    * **Función:** Permiten inspeccionar el estado de la aplicación mientras se ejecuta en modo depuración (`F5`). Incluye ventanas como *Inspección rápida (Watch)\*, \*Pila de llamadas (Call Stack)* o *Autos/Locales* para ver el valor en tiempo real de las variables. 
    * **Ejemplo de funcionamiento de la depuración** 
        1. Se hace clic en el margen izquierdo del editor de código junto a una línea (o pulsando `F9`) para colocar un **punto de interrupción (*breakpoint*)** (círculo rojo). 
        2. Se inicia la aplicación pulsando `F5`. 
        3. La ejecución se detiene automáticamente en la línea del *breakpoint* antes de ejecutarla, permitiendo avanzar línea a línea (`F10` para *Paso a paso por procedimientos* / `F11` para *Paso a paso por instrucciones*) para examinar cómo cambian las variables.
* **Editor de diseño (*Diseñador de WPF / Forms*):** 
    * **Función:** Entorno gráfico de tipo arrastrar y soltar (*drag and drop*) que permite diseñar visualmente la interfaz de usuario de aplicaciones de escritorio mediante formularios y controles (botones, etiquetas, cuadros de texto). 
    * **¿Cómo crear una nueva solución para usar el Diseñador?** Se va al menú **Archivo &gt; Nuevo &gt; Proyecto**, se selecciona la plantilla **Aplicación de Windows Forms** (o *Aplicación de WPF*) en C# y se hace clic en **Crear**.
---
### 5.2. ¿Cómo volver a visualizar las ventanas si se cierran por error?  
Si alguna de estas ventanas se cierra accidentalmente, se puede recuperar fácilmente desde el menú superior: 
* **Menú Ver (*View*):** 
    * **Explorador de soluciones:** `Ver ; Explorador de soluciones` (o `Ctrl + Alt + L`). 
    * **Consola de compilación:** `Ver ; Salida` (o `Ctrl + Alt + O\`). 
    * **Editor de diseño / Código:** `Ver ; Diseñador` (o `Mayús + F7` para alternar entre código y diseño). 
* **Menú Depurar &gt; Ventanas (*Debug &gt; Windows*):** Para reactivar ventanas específicas de depuración como *Locales*, *Autos* o *Pila de llamadas* mientras la aplicación está en pausa.
# 2. Personalización y Configuración
Para modificar y establecer una carpeta personalizada por defecto donde guardar las soluciones y proyectos en Visual Studio 2026, se deben seguir estos pasos:
1. Ir al menú superior y hacer clic en **Herramientas &gt; Opciones** (*Tools &gt; Options*). 
2. En el árbol de navegación de la izquierda, desplegar **Proyectos y soluciones** (*Projects and Solutions*) y seleccionar **Ubicaciones** (*Locations*). 
3. En el apartado **Ubicación de proyectos** (*Projects location*), hacer clic en el botón de exploración (`...`) para examinar las carpetas del equipo y seleccionar la ruta deseada (por ejemplo, `C:\Usuarios\TuNombre\\Proyectos`). 
4. Pulsar el botón **Aceptar** para confirmar la configuración. A partir de este momento, Visual Studio propondrá esa carpeta de forma predeterminada al crear cualquier nuevo proyecto.
## 7. Configuración del tema oscuro (*Dark theme*) 
Para cambiar el tema visual de la interfaz de Visual Studio 2026 a una tonalidad oscura (*Dark theme*), se siguen estos pasos: 
1. Ir al menú superior y seleccionar **Herramientas &gt; Opciones\*\* (\*Tools &gt; Options*). 
2. En la barra lateral izquierda, desplegar el menú **Entorno &gt; General** (*Environment &gt; General*). 
3. En el desplegable **Tema de color** (*Color theme*), seleccionar la opción **Oscuro** (*Dark*). 
4. Pulsar el botón **Aceptar** para guardar los cambios y aplicar la apariencia oscura inmediatamente.
## 8. Instalación de paquetes para conexión a MariaDB mediante NuGet
 Para instalar los paquetes necesarios que permiten conectar una aplicación C# a una base de datos **MariaDB** utilizando el gestor de paquetes **NuGet** en Visual Studio 2026, se deben realizar los siguientes pasos: 
 1. Abrir la solución o proyecto en Visual Studio 2026. 
 2. En el **Explorador de soluciones** (*Solution Explorer*), hacer clic con el botón derecho sobre el proyecto (o la solución) y seleccionar **Administrar paquetes NuGet...** (*Manage NuGet Packages...*). *(También se puede acceder desde el menú superior: `Herramientas ; Administrador de paquetes NuGet ; Administrar paquetes NuGet para la solución`).* 
 3. En la ventana del gestor NuGet, hacer clic en la pestaña **Examinar** (*Browse*). 
 4. En la barra de búsqueda, escribir el nombre del conector oficial de MariaDB / MySQL (por ejemplo, `MySqlConnector` o `MySql.Data`). 
 5. Seleccionar el paquete en la lista de resultados, marcar el proyecto donde se desea instalar en el panel derecho y hacer clic en el botón **Instalar** (*Install*). 
 6. Aceptar los términos de la licencia en la ventana emergente para completar la descarga e integración de las bibliotecas DLL en las dependencias del proyecto.
 ## 9. Localización e instalación del Diseñador de Clases (*Class Designer*) 
 El **Diseñador de clases** (*Class Designer*) no siempre viene instalado por defecto en las opciones básicas de Visual Studio, pero se puede agregar fácilmente mediante la herramienta **Visual Studio Installer**: 
 ### Pasos para instalar la herramienta: 
 1. Abrir el programa **Visual Studio Installer** desde el menú de inicio de Windows (o ir dentro de Visual Studio a `Herramientas ; Obtener herramientas y características...`). 
 2. Hacer clic en el botón **Modificar** (*Modify*) en la versión instalada de Visual Studio 2026. 
 3. Ir a la pestaña **Componentes individuales** (*Individual components*) en la parte superior. 
 4. En la barra de búsqueda, escribir **Diseñador de clases** (*Class Designer*). 5. Marcar la casilla del componente **Diseñador de clases** y pulsar el botón **Modificar** en la esquina inferior derecha para descargar e instalar el módulo. ### Pasos para utilizarlo en el proyecto: 
 1. Hacer clic con el botón derecho sobre el proyecto o la clase en el **Explorador de soluciones**. 
 2. Seleccionar la opción **Ver diagrama de clases** (*View Class Diagram*), o bien ir a `Agregar ; Nuevo elemento...` y seleccionar **Diagrama de clases** (*Class Diagram*).
## 10. Instalación y activación de la extensión GitHub Copilot

 Para activar y utilizar **GitHub Copilot** como asistente de inteligencia artificial para la generación de código dentro de Visual Studio 2026, se deben realizar los siguientes pasos: 
 1. Abrir **Visual Studio 2026**. 2\. Ir al menú superior **Extensiones &gt; Administrar extensiones** (*Extensions &gt; Manage Extensions*). 
 3. En la pestaña **En línea** (*Online*), utilizar la barra de búsqueda en la esquina superior derecha y escribir `GitHub Copilot`. 
 4. Seleccionar la extensión oficial **GitHub Copilot** (y/o *GitHub Copilot Chat*) en la lista de resultados y hacer clic en **Descargar** (*Download*). 
 5. Cerrar todas las ventanas abiertas de Visual Studio para permitir que el instalador de extensiones (VSIX Installer) ejecute la instalación en segundo plano. 
 6. Volver a iniciar Visual Studio 2026 e **iniciar sesión con la cuenta de GitHub** que tenga la suscripción activa (como la suscripción gratuita para estudiantes *GitHub Student Developer Pack*). 
 7. Una vez autenticado, Copilot comenzará a mostrar sugerencias de autocompletado de código en tiempo real y habilitará la ventana de chat interactivo para asistencia.
 

# 3. Tarea Final: Desarrollo de la Solución `MATES_NOM` ## 
3.1. Creación del repositorio público en GitHub (`REPO_MATES`) Para preparar el entorno de control de versiones del proyecto, se realizan los siguientes pasos iniciales en GitHub: 
1. **Crear el repositorio en GitHub:** 
    * Acceder a la cuenta personal de GitHub y pulsar en **New Repository**. 
    * **Nombre del repositorio:** `REPO_MATES`. 
        * **Visibilidad:** Seleccionar **Public**. * **Archivos iniciales:** 
    * Marcar la casilla **Add a README file**. 
    * En el desplegable **Add .gitignore**, seleccionar la plantilla de **Visual Studio** (para evitar subir archivos temporales de compilación como `/bin` o `/obj`). 
2. **Clonar el repositorio localmente:** 
    * Copiar la URL del repositorio creado en GitHub: `https://github.com/BACV970616/REPO\_MATES.git\`. 
    * Abrir **Visual Studio 2026** (o la consola Git / GitKraken) y seleccionar **Clonar un repositorio** (*Clone a repository*). 
    * Indicar la URL del repositorio (`https://github.com/BACV970616/REPO_MATES.git`) y seleccionar la carpeta local de destino en el equipo.
    
## 3.2. Creación de la Solución `MATES_NOM` y los proyectos

### Paso A: Creación de la Solución en blanco
1. Abrir **Visual Studio 2026** y seleccionar **Crear un proyecto**.
2. Buscar y seleccionar la plantilla **Solución en blanco** (*Blank Solution*).
3. Establecer el nombre de la solución como `MATES_NOM` (reemplazando `NOM` por el nombre real, por ejemplo: `MATES_BRYAN`).
4. Seleccionar como ubicación la carpeta local del repositorio clonado (`REPO_MATES`).

---

### Paso B: Creación e implementación del proyecto `MatesLib`
1. Hacer clic con el botón derecho sobre la solución en el **Explorador de soluciones** y seleccionar **Agregar &gt; Nuevo proyecto...**
2. Seleccionar la plantilla **Biblioteca de clases** (*Class Library*) en C# y hacer clic en **Siguiente**.
3. Asignar el nombre **`MatesLib`** al proyecto y finalizar su creación.
4. En el Explorador de soluciones, renombrar el archivo por defecto `Class1.cs` por **`Mates.cs`**.
5. Reemplazar el contenido de `Mates.cs` por el siguiente código C#:

```csharp
namespace MatesLib
{
    public static class Mates
    {
        /// <summary>
        /// Muestra por pantalla la tabla de multiplicar de n (del 1 al 10)
        /// </summary>
        /// <param />Número de la tabla de multiplicar
        public static void TaulaMultiplicar(int n)
        {
            for (int i = 1; i &lt;= 10; i++)
            {
                Console.WriteLine(\$"{n} x {i} = {n * i}");
            }
        }

        /// <summary>
        /// Suma tots els nombres de l'1 fins a n
        /// </summary>
        /// <param />El valor a sumar
        /// 
        public static int SumaFins(int n)
        {
            int suma = 0;
            for (int i = 1; i &lt;= n; i++)
            {
                suma += i;
            }
            return suma;
        }
    }
}

```

1. Compilar el proyecto `MatesLib` (`Ctrl + Mayús + B`) para verificar que no existen errores.

---

### Paso C: Creación del proyecto `MatesConsola` y vinculación

1. Hacer clic con el botón derecho sobre la solución `MATES_NOM` y seleccionar **Agregar &gt; Nuevo proyecto...**
2. Seleccionar la plantilla **Aplicación de consola** (*Console App*) en C# y asignarle el nombre **MatesConsola**.
3. **Agregar la referencia de la biblioteca:**
  * En el proyecto `MatesConsola`, hacer clic con el botón derecho sobre **Dependencias** (*Dependencies*).
  * Seleccionar **Agregar referencia del proyecto...** (*Add Project Reference...*).
  * Marcar la casilla del proyecto **MatesLib** y hacer clic en **Aceptar**.
4. Abrir el archivo **Program.cs** de `MatesConsola` e incluir el código de validación y llamada a la biblioteca:

```csharp
using MatesLib;

namespace MatesConsola
{
    internal class Program
    {
        static void Main(string[] args)
        {
            Console.Write("ENTRA UN NÚMERO DE 1 A 9: ");
            int num = Convert.ToInt32(Console.ReadLine());

            while (num &lt; 1 || num &gt; 9)
            {
                Console.WriteLine("EL NÚMERO QUE HAS ENTRAT NO ÉS CORRECTE.");
                Console.Write("ENTRA UN NÚMERO DE 1 A 9: ");
                num = Convert.ToInt32(Console.ReadLine());
            }

            Mates.TaulaMultiplicar(num);
        }
    }
}
```
# 4. Documentación de la actividad (Capturas de pantalla y entregables) 
## 4.1. Repositorio público de GitHub 
* **Enlace al repositorio:** [https://github.com/BACV970616/REPO\_MATES](https://github.com/BACV970616/REPO\_MATES) 
--- 
## 4.2. Ubicación del ejecutable compilado en modo Release 
* **Nombre del ejecutable:** `MatesConsola.exe` \
* **Ruta completa en el disco:** `C:\Users\bacv9\OneDrive\Desktop\DAW\ENTORNS\A1.4REPO_MATES\MATES_NOM\MatesConsola\bin\Release\net10.0\MatesConsola.exe` 

 📷 ![Ubicación del ejecutable en bin/Release](imagenes/captura1\_exe.png) 

## 4.3. Tema claro y Tema oscuro de Visual Studio 2026 

### Tema Oscuro (Dark Theme) 

📷 ![Visual Studio 2026 en Tema Oscuro](imagenes/captura2\_oscuro.png)

### Tema Claro (Light/Blue Theme) 

 📷 ![Visual Studio 2026 en Tema Claro](imagenes/captura3\_claro.png)

## 4.4. Configuración de la versión de .NET 

📷 ![Propiedades del proyecto - Marco de destino .NET 10.0](imagenes/captura4\_dotnet.png) 



## 4.5. Ejecución y funcionamiento interactivo de la aplicación 
 📷 ![Ejecución de MatesConsola en la ventana de comandos](imagenes/captura5\_consola.png)

## 4.6. Historial de commits y subida a GitHub desde Visual Studio
  📷 ![Historial de Git y confirmación Push en Visual Studio](imagenes/captura6\_git.png)
  ---

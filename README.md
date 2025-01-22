# TaskTelegram

1. **¿Qué es Git y para qué sirve?**

   **R=** "Git es un software de control de versiones, el cual su finalidad radica en la seguridad, edicion y unificacion de diferentes codigos en uno solo a travez de sus
   diferentes comandos para unir repositorios en uno solo. Este esta enfocado casi en su totalidad para trabajos en equipo."

2. **¿Cuáles son las ventajas de usar Git?**

   **R=** "Seguridad, flexibilidad de entorno, flujo de trabajo y organizacion."

3. **¿Qué diferencia hay entre Git y GitHub/GitLab/Bitbucket?**

   **Git** es una herramienta de control de versiones, es decir, un software que te permite rastrear los cambios realizados en archivos a lo largo del tiempo.

   **GitHub, GitLab y Bitbucket** son plataformas que ofrecen servicios adicionales basados en Git, como alojamiento de repositorios, colaboración, integración continua, etc.

4. **¿Qué hacen los siguientes comandos Git?**:  
   `clone`, `add`, `commit`, `push`, `pull`, `branch`, `merge`, `checkout`)

   **git clone:** Crea una copia local del repositorio ejecutando
   **git add:** Agrega cambios de archivos al área de preparación
   **git commit:** Guarda los cambios del área de preparación en el historial del proyecto. Es como crear un punto de control en el desarrollo
   **git push:** Envía los cambios locales a un repositorio remoto. Es como subir tus cambios a un servidor.
   **git pull:** Descarga los cambios de un repositorio remoto y los fusiona con la rama local. Es como actualizar tu copia local con los cambios de otros.
   **git branch:** Crea, elimina o lista las ramas existentes en el repositorio. Las ramas son como líneas de desarrollo paralelas.
   **git merge:** Combina los cambios de una rama en otra. Es como unir dos líneas de desarrollo en una sola.
   **git checkout:** Cambia a una rama existente. Es como cambiar de contexto de trabajo.

5. **¿Qué es un repositorio y cuáles son los tipos de repositorios que existen?**

   un repositorio es un lugar centralizado donde los equipos de desarrollo almacenan, rastrean y administran los cambios realizados en el código a lo largo del tiempo.

   Tipo:
   **Locales:** Se encuentran en la computadora local del desarrollador.
   Son útiles para proyectos personales o cuando no se necesita compartir el código con otros.

   **Remotos:** Se encuentran en servidores en la nube o en una red interna.
   Permiten la colaboración entre equipos distribuidos y ofrecen mayor seguridad y respaldo.(github por ejemplo)

   **Privados:** Solo pueden acceder personas autorizadas.
   Ideales para proyectos comerciales o código sensible.

   **Publicos:** Cualquiera puede acceder y ver el código.
   Perfectos para proyectos de código abierto y para compartir conocimientos.

   **Codigo fuente:** Almacenan código fuente de software.

   **Paquetes:** Almacenan paquetes de software precompilados.
   Facilitan la instalación y distribución de software.
   

6. **¿Qué son los "branch" en Git y para qué se utilizan?**

   Los **"branch"** aquellas versiones de un mismo codigo en diferentes computadoras, estas son las lineas de flujo paralelas.
   Las cuales se enfocan en distintas cosas dependiendo de la tarea que tengan los desarrolladores, estas pueden ser añadidas, modificadas o eliminadas.

11. **Describe un flujo de trabajo típico con Git.  (Ejemplo: Gitflow)**

   -Se crea un repositorio con **git init** o se clona uno existente con **git clone**
   -Se crea una rama con **git branch <nombre>**
   -Se cambia a la rama creada con **git checkout <nombre>**
   -Se agregan los cambios con **git add <archivo>**
   -Se realiza el commit con **git commit -m "descripcion"**
   -Se suben los cambios en el repositorio remoto con **git push origin <nombre_de_la_rama>**
   -Se realiza una solicitud de union o fusion. Esto se hace desde el portal donde se aloja el repositorio (Github, Gitlab, Gitbucket)
   -Luego de revisar dicho rama se fuciona con **git merge <nombre_de_la_rama>**
   -Finalizando en subir o pushear tu repo con **git push origin main**

   
11. **¿Qué es un "merge conflict" y cómo se resuelve?**

    ocurre cuando se intentan combinar cambios de dos o más ramas que han modificado las mismas líneas de un archivo.
    Cuando se produce un conflicto, Git detiene la fusión y te indica qué archivos están afectados.

    ¿Cómo se resuelven?

    Identificar los conflictos: Git te dirá qué archivos tienen conflictos.
    Editar los archivos: Abre los archivos con conflicto en tu editor de texto y revisa las secciones delimitadas por los marcadores.
    Elegir la versión correcta: Decide qué cambios quieres conservar de cada versión y elimina los marcadores.
    Marcar como resuelto: Utiliza git add <archivo> para indicar a Git que el conflicto ha sido resuelto.
    Commit: Realiza un nuevo commit para registrar la resolución del conflicto.
    Continuar la fusión: Utiliza git merge --continue para completar la fusión.
    

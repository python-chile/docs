
# Flujo de Trabajo para Equipo en GitHub

## 1. Crear un Issue

1. Ir a pestaña **Issues** y seleccionar **New Issue**.
2. Opcionalmente describir problema o tarea. Se recomienda añadir mínimo una breve descripción.
3. Agregar a Issue **Labels**, **Type**, **Projects (más status)** según corresponda.
4. **Importante** en caso de ser un Issue que tiene prioridad por sobre otras, se debe agregar en **Labels** el tag **Urgent**.

> [!NOTE]  
> - Labels: Corresponde a la(s) categoría(s) general  
> - Type: Representa qué tipo de tarea es, según la(s) categoría(s).
> - Projects: Por defecto se debe agregar a **Calendario Anual** de Python Chile.

## 2. Revisar el Issue

1. Ingresa al repositorio en GitHub.
2. Revisa la lista de Issues para identificar tareas pendientes.
3. Lee los detalles y comentarios del Issue que deseas trabajar.

## 3. Descargar el Repositorio

1. Clona el repositorio:
   - macOS/Windows/Linux:

     ```bash
     git clone <URL_DEL_REPOSITORIO>
     ```

   - Asegúrate de estar en el directorio correcto antes de continuar:

     ```bash
     cd <NOMBRE_DEL_REPOSITORIO>
     ```
> [!NOTE]  
> Ten en consideración que debes tener tu usuario de git configurado [LINK](https://git-scm.com/book/es/v2/Inicio---Sobre-el-Control-de-Versiones-Configurando-Git-por-primera-vez)

## 4. Crear un Entorno Virtual

1. macOS/Linux:

   ```bash
   python3 -m venv env
   source env/bin/activate
   ```

2. Windows:

   ```bash
   python -m venv env
   .\env\Scripts\activate
   ```
> [!TIP]
> Existen otros tipos de entornos virtuales por lo que te invitamos a explorar otras alternativas como por ejemplo _conda_, _poetry_, _virtualenv_.

## 5. Instalar las Dependencias

1. Primero corroborar si existe el archivo __requirements.txt__ y proceder a instalar.

   ```bash
   pip install -r requirements.txt
   ```
> [!WARNING]  
> Procura mantener siempre actualizado tu repositorio local
> ```bash
> git checkout main
> git pull
> ```

## 6. Crear una Rama

1. Crea una rama con la siguiente nomenclatura ``<tipo>-<número issue>-<título cambio>``. Ejemplo ``fix-108-texto-justificado``.
2. Explicación de la nomenclatura:
   1. **tipo**: Define si la rama es para cambios menores, mayores o corregir algún bug.
   2. **número issue**: Corresponde al número del issue precedido por caracter **#**. El issue debe estar creado para avanzar con PR.
   3. **título cambio**: Breve título que englobe los cambios contenidos en la rama.

3. Tabla con opciones para ``tipo``:

|  Tipo   |             Definición             |
|:-------:|:----------------------------------:|
| change  | Modificaciones de código existente |
| feature |        Funcionalidad nueva         |
|   fix   |         Corrección de bug          |

4. Ejemplo de número de Issue para **número issue**:
![image](https://github.com/user-attachments/assets/620571f3-3e7f-4e77-bafa-ec77c89ba4c5)

## 7. Realizar las Modificaciones

1. Realiza los cambios necesarios en el código o documentación.
2. Verifica tus cambios antes de continuar:

   ```bash
   git status
   ```

## 8. Realizar el Push

1. Guarda tus cambios en el repositorio local:

   ```bash
   git add .
   git commit -m "Descripción breve del cambio"
   ```

2. Envía los cambios al repositorio remoto:

   ```bash
   git push origin <NOMBRE_DE_LA_RAMA>
   ```

## 9. Realizar el Pull Request

1. Ve al repositorio en GitHub.
2. Crea un Pull Request (PR) desde tu rama hacia la rama principal (`main`).
3. Describe los cambios realizados en el PR.
4. Asigna la revisión al menos a los siguientes usuarios Aldo Caneo @ancaneo, Tony Rodriguez @Tony-Rome, Pablo Lira @pablolirag y Carlos Carrasco @krlitosforever .


## 10. Proceso de Revisión Pull Request (PR)

Según la importancia de avanzar con los cambios, se contemplan dos casos:

### Revisión Estándar
Cualquier PR por defecto entra en esta categoría.

1. Esperar revisión de al menos 2 integrantes del equipo de desarrollo.
2. Resolver/responder comentarios realizados en PR. Opcionalmente quién crea comentarios debe dar **resolve**.
   - **Aclaración: Resolver significa analisar comentarios según su viabilidad.**
3. Cumpliendo **punto 1** y **punto 2**, se debe esperar 24 hrs para hacer merge. Quién crea PR debe realizar **merge**.
4. Cumpliendo **punto 3**, se debe esperar 24 hrs para que cualquier integrante del equipo de desarrollo pueda realizar **merge**.

### Revisión Urgente
Caso particular para PR que deben ser completadas lo antes posible.

1. Esperar revisión de al menos 1 integrante del equipo de desarrollo.
2. Opcionalmente resolver/responder comentarios realizados en PR. Todo comentario **no resuelto/respondido** se pospone para una próxima PR.
3. Solamente quién **crea** PR o **aprueba** PR puede realizar **merge**.
4. Notificar en canal de discord **equipo-desarrollo**  con tag **@desarrollo** más enlace de la PR urgente. Issue relacionada a dicha PR debe contener **label urgent**.
5. En caso extremo por temas de tiempo o por falta de revisión, sugerir reunión con integrantes de desarrollo. 

## 11. Eliminación de rama post PR

1. Toda rama que sea de tipo **change** o **fix** se debe eliminar una vez se realiza **merge** en la respectiva PR.
2. Rama de tipo **feature** _no se debe eliminar de inmediato_, se debe esperar **30 días** para que dueño/a deba eliminar dicha rama.

## 12. No dudes solicitar ayuda en caso de necesitarla

Esperamos que este proceso sea lo más fácil posible; sin embargo, si tienes algunda duda o presentas problemas, no dudes en preguntar a algún miembro de la comunidad. Estaremos felices de poder ayudar.

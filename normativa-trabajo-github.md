
# Flujo de Trabajo para Equipo en GitHub

## 1. Revisar el Issue

1. Ingresa al repositorio en GitHub.
2. Revisa la lista de Issues para identificar tareas pendientes.
3. Lee los detalles y comentarios del Issue que deseas trabajar.

## 2. Tomar o Crear un Issue

1. **Tomar un Issue existente**:
   - Comenta en el Issue indicando que lo trabajarás.
   - Asóciate al Issue si tienes los permisos necesarios.
2. **Crear un nuevo Issue**:
   - Ve a la pestaña "Issues" y selecciona "New Issue".
   - Describe el problema o tarea de manera detallada.
   - Etiqueta el Issue según corresponda (e.g., bug, feature, enhancement).

## 3. Descargar el Repositorio

1. Clona el repositorio:
   - macOS/Windows:

     ```bash
     git clone <URL_DEL_REPOSITORIO>
     ```

   - Asegúrate de estar en el directorio correcto antes de continuar:

     ```bash
     cd <NOMBRE_DEL_REPOSITORIO>
     ```

## 4. Crear un Entorno Virtual

1. macOS:

   ```bash
   python3 -m venv env
   source env/bin/activate
   ```

2. Windows:

   ```bash
   python -m venv env
   .\env\Scripts\activate
   ```

## 5. Instalar las Dependencias

1. Instala Pelican u otras dependencias requeridas:

   ```bash
   pip install -r requirements.txt
   ```

## 6. Crear una Rama

1. Crea una rama basada en la tarea del Issue:

   ```bash
   git checkout -b <NOMBRE_DE_LA_RAMA>
   ```

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

## 10. Proceso de Revisión

1. Espera la revisión de otros 2 miembros del equipo.
2. Atiende los comentarios realizados en el PR.

## 11. Aplicar Correcciones o No

1. Si se solicitan cambios:
   - Realiza las modificaciones necesarias.
   - Realiza otro commit y push a la misma rama.
2. Si no hay cambios solicitados:
   - Debes esperar la aprobación de un miembro antiguo de la comunidad.

## 12. Actualización de repositorio

1. Una vez aprobado, Actualiza el repositorio local:

   ```bash
   git pull origin <NOMBRE_DE_LA_RAMA_PRINCIPAL>
   ```

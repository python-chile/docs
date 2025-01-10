
# Flujo de Trabajo para Equipo en GitHub

## 1. Crear un Issue

1. **Crear un nuevo Issue**:
   - Ve a la pestaña "Issues" y selecciona "New Issue".
   - Describe el problema o tarea de manera detallada.
   - Etiqueta el Issue según corresponda (e.g., bug, feature, enhancement).

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

1. Crea una rama basada en la tarea del Issue un ejemplo sería __pch-<tipo>-<numero de issue>-<título cambio>__:

   ```bash
   git checkout -b pch-<tipo>-<numero issue>-<titulo cambio>

   #ejemplo
   git checkout -b pch-fix-108-texto-justificado
   ```
> [!NOTE]  
> Esta nomenclatura pch-[tipo]-[numero issue]-[titulo cambio] corresponde a la abreviatura de Python Chile (pch). El tipo corresponde a si es un fix o change. El número de issue corresponde al correlativo que entrega github (imagen de ejemplo al final). Y en la parte final se agrega un texto descriptivo a la modificación realizada.
> 
> ![image](https://github.com/user-attachments/assets/620571f3-3e7f-4e77-bafa-ec77c89ba4c5)

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


## 10. Proceso de Revisión

1. Espera la revisión de al menos otros 2 miembros del equipo.
2. Realiza las modificaciones necesarias según los comentarios realizados en la _pull request_.
3. Con dos revisiones aprobadas se puede hacer _merge_ 24 horas después.
4. La responsabilidad de realizar el _merge_ es de quien creó el _pull request_.

## 11. No dudes solicitar ayuda en caso de necesitarla

Esperamos que este proceso sea lo más fácil posible; sin embargo, si tienes algunda duda o presentas problemas, no dudes en preguntar a algún miembro de la comunidad. Estaremos felices de poder ayudar.

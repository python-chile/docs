# **Guía para la creación de un post**

## **1. Preparación de la imagen**  

- Asegúrate de que la imagen cumpla con las siguientes especificaciones:
  - Dimensiones: **330x330 píxeles**.
  - Formato: **jpg**, **jpeg** o **png**.
- Guarda la imagen con el siguiente nombre:  
     **coordinacion_nombre_apellido.extensión**  
     (Reemplaza "nombre" y "apellido" con los correspondientes, y "extensión" con el formato de la imagen).  
- Ubica la imagen en la siguiente carpeta dentro del proyecto:  
     **content/images/**

## **2. Creación del archivo Markdown**  

- El archivo que contendrá el post debe ubicarse en la carpeta:  
     **content/**  
- Sigue la siguiente nomenclatura para el nombre del archivo:  
     **año-mes-día-presentacion-nombre-apellido.md**  
  - Ejemplo:  
       **2025-01-23-presentacion-carlos-carrasco.md**.

## **3. Estructura del contenido del post**  

- Edita el contenido del archivo Markdown que se encuentra en el punto 5 siguiendo las normas definidas en la guía oficial:  
     [Normativa para trabajo en GitHub](https://github.com/python-chile/docs/blob/master/normativa-trabajo-github.md).  
- Asegúrate de incluir:
  - Una presentación clara y concisa.
  - Información relevante y acorde al propósito del post.
  - Un tono respetuoso y profesional.

##  **4. Revisión final**  

- Verifica que:
  - La imagen cumple con los requisitos de tamaño, formato y ubicación.
  - El archivo Markdown está correctamente nombrado y ubicado.
  - El contenido del post sigue la normativa mencionada.

## **5. Formato**

```text
---
layout: post
title: Presentación de [Tu Nombre] 🎉
subtitle: Presentación nuevo integrante de coordinación
author: Python Chile
image: coordinacion_nombre_apellido.jpg #extensión jpg,jpeg, png, medida 330x330 px
tags: coordinación, presentación, pythonchile2025
category: presentación
---

## Introducción breve

Hola, mi nombre es **[Tu Nombre]**. Soy [tu ocupación/rol] y actualmente resido en [ciudad, país]. [Agrega una línea adicional sobre ti, como un dato curioso o algo que te motive].

## ¿Cómo descubriste Python y qué te motivó a aprenderlo?

[Cuenta cómo conociste Python y por qué decidiste aprenderlo. Comparte tu experiencia inicial.]

## ¿Qué proyectos has trabajado o estás trabajando actualmente en Python?

[Habla de proyectos relevantes en los que hayas participado o que estés desarrollando ahora. Menciona sus objetivos o aprendizajes clave. (Esto puede incluir proyectos personales, laborales o académicos).]

## ¿Cuál es tu experiencia previa en tecnología o programación?

[Describe tu formación, experiencias anteriores o si estás comenzando desde cero.]

## ¿Qué te inspiró a unirte a la comunidad Python Chile?

[Explica qué te atrajo de la comunidad y por qué decidiste formar parte de ella.]

## ¿Qué esperas lograr o aprender siendo parte de esta comunidad?

[Habla sobre tus metas dentro de la comunidad Python Chile y lo que te gustaría aportar.]

## ¿Hay alguna área específica de Python o la tecnología que te apasione?

[Por ejemplo: inteligencia artificial, desarrollo web, análisis de datos, etc.]

## ¿Qué recursos o consejos le darías a alguien que está comenzando con Python?

[Comparte algún recurso, técnica o consejo que haya sido útil para ti.]

## ¿Qué te gusta hacer fuera del mundo de la programación?

[Cuéntanos sobre tus hobbies, intereses personales o actividades favoritas.]

## ¿Hay algo más que quieras compartir con la comunidad?

[Incluye cualquier otra información que creas relevante o algún mensaje personal.]

### Encuéntrame en:

- GitHub: [Tu perfil de GitHub] *(opcional)*
- LinkedIn: [Tu perfil de LinkedIn] *(opcional)*
- Twitter: [Tu usuario de Twitter] *(opcional)*

¡Gracias por leer mi presentación!
```

## **6. Generar contenido**

Para generar el contenido debes ejecutar el siguiente comando:

```python
pelican content
```

Para ver la correcto visualización del contenido puedes hacerlo a través del siguiente comando:

```python
pelican -l
```

Si todo ha salido bien se deberá desplegar la web en tu servidor local. Ahora puedes proseguir con [Normativa para trabajo en GitHub](https://github.com/python-chile/docs/blob/master/normativa-trabajo-github.md)

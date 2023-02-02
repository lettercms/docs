---
sidebar_position: 3
---

# Arquitectura

LetterCMS tiene una arquitectura basica de **microservicios** en su mayoria en entornos **Serverless**. Debido a su escalabilidad y alta disponibilidad.

## Servicios

Los servicios disponibles son:

- Control de mando
- Cliente
- API
- Proxy de Contenido
- Documentacion (Donde estas en este momento)

Todos desplegados y alojados en Vercel. Excepto la Documentacion que esta alojada en Netlify 

### Dashboard

El dashboard es la interfaz de usuario principal, con la cual podras escribir contenido, revisar datos y demás acciones.

#### Tecnologias
 
- NextJS
- Firebase
- Mongoose
- NextAuth
- CKEditor
- GrapesJS

#### Integraciones

- Sendinblue
- API de Unsplash

### API

La API es el motor principal. El control de mando se integra utilizando el **SDK** y el propio [blog](https://lettercms.vercel.app/blog) esta contruido utilizando **LetterCMS**.

#### Tecnologias

- NextJS
- Firebase
- Mongoose
- QStash
- BrainJS [Posible cambio](/docs/roadmap#machine-learning)

#### Integraciones

- API de Facebook
- API de Twitter
- API de Linkedin

### Proxy de Contenido

El proxy de contenido es un proxy con el cual se sirven las imagenes almacenadas en firebase. Optimizando la entrega de imagenes y redimension via URL

#### Tecnologias

- Sharp
- Firebase

### Documentación

Esta Pagina. Desplegada en Netlify

#### Tecnologias

- Sharp
- Firebase
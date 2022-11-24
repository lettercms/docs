---
sidebar_position: 1
---

# Arquitectura

LetterCMS tiene una arquitectura basica de **microservicios** en su mayoria en entornos **Serverless**. Debido a su escalabilidad y alta disponibilidad.

## Servicios

Los servicios disponibles son:

- Dashboard
- API
- Proxy de Contenido
- Proxy de las plantillas
- Servicio de Machine Learning
- Documentacion (Donde estas en este momento)

Todos desplegados y alojados en Vercel. Excepto la Documentacion que esta alojada en Netlify 

### Dashboard

El dashboard es la interfaz de usuario principal.

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

La API el el motor principal. El dashboard se integra utilizando el [SDK](/docs/sdk) y el [blog](https://lettercms.vercel.app/blog) esta contruido utilizando LetterCMS.

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

### Proxy de plantillas

### Motor de Mahine Learning

### Documentación


# Fase 1: Sitio Web Estático en Amazon S3

## Descripción

La primera fase del proyecto AWS Café Bistro Platform consistió en implementar un sitio web estático para una cafetería y panadería ficticia utilizando Amazon S3.

El objetivo fue proporcionar una presencia digital básica que permitiera mostrar información relevante del negocio, como productos, horarios de atención, ubicación y datos de contacto.

---

## Objetivo

Desplegar un sitio web estático accesible desde Internet utilizando servicios administrados de AWS, minimizando costos y complejidad operacional.

---

## Arquitectura

```text
Usuario
   │
   ▼
Amazon S3
   │
   ▼
Sitio Web Estático
```

---

## Servicios AWS Utilizados

- Amazon S3
- AWS IAM

---

## Funcionalidades Implementadas

- Publicación de contenido web estático.
- Almacenamiento de archivos HTML, CSS e imágenes.
- Configuración de alojamiento web estático.
- Acceso público al sitio web.
- Gestión de permisos para los recursos.

---

## Proceso de Implementación

### 1. Creación del Bucket S3

Se creó un bucket en Amazon S3 para almacenar los archivos del sitio web.

### 2. Carga de Archivos

Se cargaron los archivos necesarios para el funcionamiento del sitio:

- HTML
- CSS
- Imágenes

### 3. Configuración de Static Website Hosting

Se habilitó la funcionalidad de alojamiento web estático del bucket y se configuró:

- Documento principal: `index.html`
- Documento de error: `error.html` (si corresponde)

### 4. Configuración de Acceso

Se ajustaron los permisos necesarios para permitir que los usuarios accedieran al contenido del sitio web.

### 5. Validación

Se verificó que el sitio estuviera disponible mediante la URL generada por Amazon S3.

---

## Resultado

El sitio web quedó disponible públicamente, permitiendo a los usuarios consultar información básica de la cafetería y panadería sin necesidad de utilizar servidores o bases de datos.

Esta arquitectura proporciona una solución simple, económica y altamente disponible para contenido estático.

---

## Beneficios de la Solución

- Bajo costo operativo.
- Alta disponibilidad.
- Fácil administración.
- Escalabilidad automática del almacenamiento.
- No requiere administración de servidores.

---

## Evidencias

Las capturas de pantalla de esta implementación se encuentran en:

```text
screenshots/
```

---

## Aprendizajes Obtenidos

Durante esta fase se adquirieron conocimientos prácticos sobre:

- Amazon S3.
- Hosting de sitios web estáticos.
- Gestión de permisos.
- Conceptos básicos de arquitectura cloud.
- Publicación de contenido en AWS.
- Buenas prácticas para soluciones serverless simples.

---

## Próxima Fase

La siguiente etapa del proyecto incorporará una aplicación capaz de recibir pedidos en línea mediante Amazon EC2, transformando el sitio informativo en una solución interactiva para los clientes.

➡️ Fase 2: Sistema de pedidos en línea con Amazon EC2.

# Fase 1: Sitio Web Estático en Amazon S3

## Descripción

La primera fase del proyecto AWS Café Bistro Platform consistió en implementar un sitio web estático para una cafetería y panadería ficticia utilizando Amazon S3.

El objetivo fue proporcionar una presencia digital básica que permitiera mostrar información relevante del negocio, como productos, horarios de atención, ubicación y datos de contacto.

Además, se aplicaron controles de acceso mediante AWS Identity and Access Management (IAM) para administrar de forma segura los recursos utilizados en la solución.

---

## Objetivo

Desplegar un sitio web estático accesible desde Internet utilizando servicios administrados de AWS, aplicando principios básicos de seguridad y administración de recursos.

---

## Arquitectura

```text
Administrador
      │
      ▼
   AWS IAM
      │
      ▼

┌──────────────────────── AWS Cloud ────────────────────────┐

┌───────────────────────────────────────────────────────────┐
│                        Amazon S3                          │
│                                                           │
│               Static Website Hosting                      │
│                                                           │
│  • index.html                                             │
│  • archivos CSS                                           │
│  • imágenes                                               │
│  • contenido estático                                     │
└───────────────────────────────────────────────────────────┘

└───────────────────────────────────────────────────────────┘
                       ▲
                       │ HTTP/HTTPS
                       │
                 Usuario Final
```

> El diagrama definitivo se encuentra en la carpeta `architecture/`.

---

## Servicios AWS Utilizados

### Amazon S3

Utilizado para:

- Almacenar archivos del sitio web.
- Habilitar el alojamiento web estático.
- Publicar contenido accesible desde Internet.

### AWS IAM

Utilizado para:

- Administrar permisos de acceso a AWS.
- Controlar quién puede crear y modificar recursos.
- Aplicar el principio de mínimo privilegio.
- Gestionar de forma segura la configuración del bucket S3.

---

## Funcionalidades Implementadas

- Publicación de un sitio web estático.
- Almacenamiento de archivos HTML, CSS e imágenes.
- Configuración de Static Website Hosting.
- Acceso público al contenido web.
- Administración segura mediante IAM.
- Validación de disponibilidad del sitio.

---

## Proceso de Implementación

### 1. Creación del Bucket S3

Se creó un bucket destinado al almacenamiento de los archivos del sitio web.

### 2. Configuración del Sitio Web Estático

Se habilitó la característica Static Website Hosting y se definió el documento principal del sitio.

### 3. Carga de Contenido

Se cargaron los archivos necesarios para el funcionamiento del sitio:

- HTML
- CSS
- Recursos gráficos

### 4. Configuración de Permisos

Se ajustaron las políticas y permisos necesarios para permitir el acceso público al contenido publicado.

### 5. Administración Mediante IAM

Se utilizaron identidades y permisos administrados por AWS IAM para controlar el acceso a los recursos y las tareas administrativas del proyecto.

### 6. Validación

Se verificó la correcta publicación y disponibilidad del sitio web mediante la URL generada por Amazon S3.

---

## Consideraciones de Seguridad

Durante esta fase se aplicaron conceptos básicos de seguridad en AWS:

- Uso de IAM para administración de acceso.
- Separación entre usuarios administradores y usuarios finales.
- Gestión controlada de permisos sobre los recursos.
- Aplicación del principio de mínimo privilegio.

---

## Resultado

Se obtuvo un sitio web estático alojado en Amazon S3, accesible desde Internet y gestionado de forma segura mediante AWS IAM.

La solución proporciona una arquitectura simple, económica y escalable para publicar contenido informativo de una cafetería o panadería sin necesidad de administrar servidores.

---

## Beneficios de la Solución

- Bajo costo operativo.
- Alta disponibilidad.
- Escalabilidad automática.
- Administración simplificada.
- Seguridad basada en IAM.
- Ausencia de infraestructura de servidores.

---

## Evidencias

Las capturas de pantalla y evidencias de implementación se almacenan en:

```text
screenshots/
```

---

## Aprendizajes Obtenidos

Durante esta fase se adquirieron conocimientos prácticos sobre:

- Amazon S3.
- Hosting web estático.
- AWS IAM.
- Control de acceso basado en permisos.
- Administración de recursos cloud.
- Publicación de aplicaciones estáticas.
- Conceptos fundamentales de arquitectura en AWS.

---

## Próxima Fase

La siguiente etapa del proyecto transformará el sitio informativo en una solución interactiva incorporando una aplicación web alojada en Amazon EC2 para la recepción de pedidos en línea.

➡️ Fase 2: Sistema de pedidos utilizando Amazon EC2.

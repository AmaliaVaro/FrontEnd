# Premium Padel Club – Front-End

Front-end estático en **HTML + CSS** para la aplicación web de **reserva de pistas de pádel** desarrollada en la asignatura de **Programación de Aplicaciones Telemáticas**.

Este repositorio contiene la parte visual de la aplicación para la entrega de frontend, incluyendo tanto la zona de usuario como la zona de administración. La interfaz está construida sin JavaScript, por lo que las páginas funcionan como maqueta navegable y representación de los flujos principales de la aplicación.

---

## Objetivo del proyecto

El objetivo de este front-end es ofrecer una interfaz clara y coherente con el backend del sistema de reservas de pistas, permitiendo representar los principales casos de uso del proyecto:

- consulta de pistas disponibles
- visualización de reservas del usuario
- acceso al perfil
- consulta de notificaciones
- gestión administrativa de usuarios
- gestión administrativa de pistas
- gestión administrativa de reservas
  
---

## Estructura del proyecto

### Zona pública / usuario

- `index.html`  
  Página principal de la aplicación con acceso a reservas, reservas del usuario, perfil, login, registro y portal admin. 

- `logIn.html`  
  Pantalla de inicio de sesión. 

- `SignIn.html`  
  Pantalla de registro de nuevo usuario. 

- `reservas.html`  
  Vista de reserva de pistas con fecha, filtros visuales por tipo y tarjetas con horarios disponibles y ocupados.
  
- `misReservas.html`  
  Pantalla de consulta de reservas del usuario con filtros por reservas actuales e históricas.

- `perfil.html`  
  Página de perfil del usuario con información personal editable a nivel visual.
  
- `notificaciones.html`  
  Vista de notificaciones y recordatorios relacionados con reservas.

---

### Zona de administración

- `admin.html`  
  Panel principal de administración con métricas resumen, accesos rápidos y tabla de últimas reservas.

- `adminPistas.html`  
  Gestión de pistas en formato tabla, con filtros por estado y acceso al formulario de edición/alta.

- `adminFormularioPista.html`  
  Formulario de gestión de pista para editar sus datos principales.

- `adminUsuarios.html`  
  Gestión de usuarios en formato tabla con filtros por estado y rol.

- `adminUsuarioDetalle.html`  
  Vista de detalle y edición de un usuario.
  
- `adminReservas.html`  
  Gestión global de reservas en formato tabla, con filtros por estado y reservas del día.

- `adminReservaDetalle.html`  
  Vista de detalle y edición de una reserva concreta.

- `styles.css`  
  Hoja de estilos común para toda la aplicación, incluyendo estilos de usuario y del área de administración.
  
---

## Características del diseño

- Navegación común mediante cabecera compartida
- Estilo visual homogéneo en todas las pantallas
- Diseño responsive basado en `flex`, `grid` y `@media`
- Uso de tablas para la gestión administrativa
- Uso de tarjetas para la parte de reserva y consulta del usuario
- Filtros visuales implementados con `input type="radio"` y CSS puro
- Distinción visual entre zona de usuario y zona admin mediante badge y navegación específica

---

## Flujo principal de navegación

### Usuario
Desde `index.html` se puede acceder a:

- reservar pista
- ver reservas personales
- iniciar sesión
- crear cuenta
- acceder al perfil
- consultar notificaciones

### Administrador
Desde `index.html` o desde el enlace al portal admin se accede a:

- panel de administración
- gestión de usuarios
- gestión de pistas
- gestión de reservas

---

## Limitaciones actuales

Esta entrega corresponde únicamente a **HTML + CSS**, por lo que:

- no hay autenticación real
- no existe validación funcional de formularios más allá del HTML
- los filtros y acciones son demostrativos
- no hay persistencia de datos
- no hay integración aún con la API backend

Las páginas representan la estructura visual y los flujos esperados de la aplicación de cara a la siguiente fase del proyecto.

---

## Autores

Proyecto realizado para la asignatura **Programación de Aplicaciones Telemáticas**.

Front-end desarrollado por el equipo del proyecto **Raffaella Boccacci, Carlos Gárate, Martina Íscar, Irene Morales y Amalia Varo**.

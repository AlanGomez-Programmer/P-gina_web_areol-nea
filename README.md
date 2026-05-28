# ✈️ VUESU AIR

## 📌 Descripción General

**VUESU AIR** es una interfaz web estática para una aerolínea ficticia enfocada en la gestión y reserva de vuelos.
El proyecto fue desarrollado únicamente con **HTML5** y **CSS3**, sin utilizar JavaScript, simulando navegación y tiempos de carga mediante páginas intermedias con redirecciones automáticas.

La aplicación está diseñada bajo un enfoque **responsive**, comenzando desde una versión móvil y posteriormente adaptada para escritorio mediante `media queries`.

---

# 🎯 Objetivo del Proyecto

Desarrollar una experiencia visual moderna para una aerolínea, permitiendo:

* Inicio de sesión de usuarios
* Registro de cuentas
* Recuperación de contraseña
* Búsqueda de vuelos
* Visualización de vuelos disponibles
* Gestión de vuelos reservados
* Realización de check-in
* Simulación de cargas y transiciones de navegación

---

# 🛠️ Tecnologías Utilizadas

* HTML5
* CSS3
* Flexbox
* CSS Grid
* Media Queries
* Google Fonts
* Material Symbols

---

# 📁 Estructura del Proyecto

```txt
VUESU-AIR/
│
├── index.html
├── menu.html
├── buscar_vuelos.html
├── vuelos.html
├── checkin.html
├── mis_vuelos.html
├── registro.html
├── recuperar.html
├── crear_contrasena.html
│
├── animacion/
│   ├── cargando_menu.html
│   ├── cargando_buscar_vuelos.html
│   ├── cargando_check_in.html
│   ├── cargando_mis_vuelos.html
│   ├── cargando_vuelos_disponibles.html
│   ├── cargando_cuenta_registro.html
│   ├── cargando_crear_contrasena.html
│   ├── cargando_crear_contraseña_recuperar.html
│   ├── cargando_recuperar_contraseña.html
│   └── cerrar_sesion.html
│
├── css/
│   ├── style.css
│   ├── layout.css
│   ├── forms.css
│   ├── menu.css
│   ├── vuelos.css
│   ├── cargando.css
│   └── responsive.css
│
└── img/
    ├── logo.png
    ├── logo_horizontal.png
    ├── avion.png
    ├── buscar_vuelos.png
    ├── check_in.png
    └── mis_vuelos.png
```

---

# 🧭 Flujo de Navegación

## 🔐 Inicio de Sesión

```txt
index.html
↓
animacion/cargando_menu.html
↓
menu.html
```

---

## ✈️ Buscar Vuelos

```txt
menu.html
↓
animacion/cargando_buscar_vuelos.html
↓
buscar_vuelos.html
↓
animacion/cargando_vuelos_disponibles.html
↓
vuelos.html
```

---

## ✅ Check-in

```txt
menu.html
↓
animacion/cargando_check_in.html
↓
checkin.html
↓
animacion/cargando_menu.html
↓
menu.html
```

---

## 🧾 Mis Vuelos

```txt
menu.html
↓
animacion/cargando_mis_vuelos.html
↓
mis_vuelos.html
```

---

## 👤 Registro de Usuario

```txt
index.html
↓
animacion/cargando_cuenta_registro.html
↓
registro.html
↓
animacion/cargando_crear_contrasena.html
↓
crear_contrasena.html
```

---

## 🔑 Recuperación de Contraseña

```txt
index.html
↓
animacion/cargando_recuperar_contraseña.html
↓
recuperar.html
↓
animacion/cargando_crear_contraseña_recuperar.html
↓
crear_contrasena.html
```

---

# 📄 Descripción de Páginas

## 🔐 `index.html`

Página principal de inicio de sesión.

### Características

* Formulario de correo y contraseña
* Recordatorio de sesión
* Enlaces para:

  * Crear cuenta
  * Recuperar contraseña

---

## 🏠 `menu.html`

Menú principal de navegación.

### Opciones disponibles

* Buscar vuelos
* Check-in
* Mis vuelos
* Cerrar sesión

---

## 🔎 `buscar_vuelos.html`

Formulario para consultar vuelos disponibles.

### Funcionalidades

* Selección de:

  * origen
  * destino
  * fecha de salida
  * fecha de regreso
* Opción “Solo ida”

---

## ✈️ `vuelos.html`

Visualización de vuelos disponibles.

### Información mostrada

* Horarios
* Duración
* Número de vuelo
* Precio

---

## ✅ `checkin.html`

Página para realizar check-in.

### Incluye

* Información del vuelo
* Formulario de contacto de emergencia

---

## 🧾 `mis_vuelos.html`

Listado de vuelos reservados por el usuario.

### Muestra

* Estado del vuelo
* Horario
* Ruta
* Código de vuelo

---

## 📝 `registro.html`

Formulario para creación de cuenta.

### Campos

* Nombre completo
* Documento de identidad
* Correo electrónico
* Teléfono
* Ciudad

---

## 🔑 `recuperar.html`

Formulario de recuperación de contraseña mediante correo electrónico.

---

## 🔒 `crear_contrasena.html`

Página para registrar o actualizar contraseña.

---

# 🎨 Sistema de Estilos

## `style.css`

Contiene:

* Variables globales
* Colores
* Tipografías
* Reset CSS

---

## `layout.css`

Maneja:

* Contenedores
* Layout principal
* Header/logo

---

## `forms.css`

Estilos de:

* Formularios
* Inputs
* Botones
* Login y registro

---

## `menu.css`

Diseño del menú principal:

* Tarjetas
* Hover effects
* Animaciones

---

## `vuelos.css`

Estilos para:

* Tarjetas de vuelos
* Check-in
* Mis vuelos

---

## `cargando.css`

Animaciones de carga:

* Barra de progreso
* Avión en movimiento
* Pantallas intermedias

---

## `responsive.css`

Adaptaciones responsive:

* Desktop
* Layouts amplios
* Grid systems
* Reorganización visual

---

# 📱 Diseño Responsive

El proyecto fue construido siguiendo una estrategia:

```txt
Mobile First
```

Posteriormente se agregaron adaptaciones para escritorio mediante:

```css
@media (min-width: 1024px)
```

---

# ✨ Características Destacadas

* Diseño moderno para aerolínea
* Navegación visual intuitiva
* Animaciones CSS
* Transiciones suaves
* Responsive Design
* Simulación de cargas sin JavaScript
* Organización modular de estilos

---

# 🚀 Cómo Ejecutar el Proyecto

1. Descargar o clonar el repositorio.
2. Abrir el proyecto en Visual Studio Code.
3. Ejecutar con Live Server o abrir `index.html` directamente en el navegador.


---


## 👨 AUTOR
Programador Full-Stack Jr. Alan Gomez

GitHub: [AlanGomez-Programmer](https://github.com/AlanGomez-Programmer)

Linkedln: alan-gomez-763163320
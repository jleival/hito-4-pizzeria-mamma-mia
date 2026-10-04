# 🍕 Pizzería Mamma Mía! — Hito 4

> Aplicación web desarrollada en **React + Vite**, que implementa el consumo de una API REST externa alojada en un backend local, utilizando hooks para la gestión de estados y efectos asíncronos.

---

## 📋 Descripción del Hito

El objetivo principal de este hito es conectar la aplicación frontend desarrollada con **React + Vite** a un servidor backend, obteniendo dinámicamente la información de las pizzas mediante peticiones HTTP utilizando `fetch`.

De esta manera, los datos que anteriormente podían encontrarse almacenados de forma estática en el frontend son reemplazados por información obtenida directamente desde una **API REST**.

---

## 🚀 Características Principales

### 🍕 Consumo de API con `useEffect`

Implementación de `useEffect` para ejecutar peticiones asíncronas al backend y obtener la información de las pizzas.

### 🏠 Componente `Home.jsx`

Renderiza dinámicamente una lista completa de tarjetas de pizzas obtenidas desde el endpoint general de la API.

### 🍕 Componente `Pizza.jsx`

Muestra el detalle de una pizza específica utilizando su identificador (`p001`), incluyendo:

* Imagen
* Nombre
* Descripción
* Ingredientes
* Precio

### 📱 Interfaz Responsiva

La aplicación utiliza **React Bootstrap** y **Bootstrap** para crear una interfaz adaptable a distintos tamaños de pantalla, tanto en dispositivos móviles como en computadores de escritorio.

---

## 🛠️ Tecnologías y Librerías Utilizadas

| Tecnología             | Descripción                                                         |
| ---------------------- | ------------------------------------------------------------------- |
| ⚛️ **React**           | Biblioteca de JavaScript para la creación de interfaces de usuario  |
| ⚡ **Vite**             | Herramienta de desarrollo y construcción para aplicaciones frontend |
| 🎨 **React Bootstrap** | Biblioteca de componentes Bootstrap para React                      |
| 🅱️ **Bootstrap**      | Framework CSS para el diseño responsivo                             |
| 🟨 **JavaScript ES6+** | Lenguaje utilizado para la lógica de la aplicación                  |
| 🌐 **HTML5**           | Estructura de la aplicación                                         |
| 🎨 **CSS3**            | Estilos y presentación visual                                       |

---

## 📁 Estructura del Proyecto

```text
src/
├── assets/
│   └── img/
│
├── components/
│   ├── CardPizza.jsx
│   ├── Footer.jsx
│   ├── Header.jsx
│   └── Navbar.jsx
│
├── views/
│   ├── Home.jsx
│   └── Pizza.jsx
│
├── App.jsx
└── main.jsx
```

> La estructura puede variar dependiendo de la organización final del proyecto.

---

## ⚙️ Instalación y Ejecución

Para ejecutar correctamente la aplicación es necesario levantar tanto el **Backend** como el **Frontend**.

Se recomienda utilizar **dos terminales independientes**.

---

### 1. 📥 Clonar el repositorio

```bash
git clone https://github.com/jleival/hito-4-pizzeria-mamma-mia
cd hito-4-pizzeria-mamma-mia
```

> Reemplaza `tu-repositorio` y `nombre-de-tu-repositorio` por los datos correspondientes a tu repositorio.

---

### 2. 🔧 Levantar el Backend

Primero debes disponer del servidor backend proporcionado para el ejercicio.

Dirígete a la carpeta donde se encuentra el backend y ejecuta:

```bash
npm install
```

Luego inicia el servidor:

```bash
npm start
```

El backend estará disponible en:

```text
http://localhost:5000
```

---

### 3. 💻 Levantar el Frontend

Abre una **segunda terminal** y dirígete a la carpeta principal del proyecto React.

Instala las dependencias:

```bash
npm install
```

Luego inicia el servidor de desarrollo de Vite:

```bash
npm run dev
```

Vite mostrará en la terminal la dirección donde estará disponible la aplicación.

Generalmente será:

```text
http://localhost:5173
```

Abre esa dirección en tu navegador.

---

## 🌐 Endpoints de la API

La aplicación consume los siguientes endpoints del backend:

### 📋 Obtener todas las pizzas

```http
GET http://localhost:5000/api/pizzas
```

Este endpoint permite obtener la información de todas las pizzas disponibles para mostrarlas en la página principal.

---

### 🍕 Obtener una pizza por ID

```http
GET http://localhost:5000/api/pizzas/p001
```

Este endpoint permite obtener la información específica de una pizza utilizando su ID.

Por ejemplo:

```text
p001
```

La información obtenida se utiliza para mostrar el detalle de la pizza seleccionada.

---

## 🔄 Flujo de funcionamiento

```text
┌─────────────────────┐
│   Usuario ingresa   │
│   a la aplicación   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│      React + Vite   │
└──────────┬──────────┘
           │
           │ fetch()
           ▼
┌─────────────────────┐
│   Backend / API     │
│ localhost:5000      │
└──────────┬──────────┘
           │
           │ JSON
           ▼
┌─────────────────────┐
│     useEffect()     │
│ procesa los datos   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Componentes React   │
│ Home / Pizza        │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  Pizzas mostradas   │
│   en la interfaz    │
└─────────────────────┘
```

---

## 🎯 Objetivos de Aprendizaje

Con este proyecto se practican principalmente los siguientes conceptos:

* Consumo de APIs REST.
* Peticiones HTTP mediante `fetch`.
* Uso de `useEffect`.
* Manejo de datos obtenidos desde un backend.
* Renderizado dinámico de componentes.
* Uso de parámetros para obtener información específica.
* Componentización en React.
* Uso de React Bootstrap.
* Diseño responsivo.
* Integración entre frontend y backend.

---

## 👤 Autor

**Jorge Leiva**

💻 Desarrollo Frontend
🎓 Talento Digital / Desafío Latam

---

## 📚 Proyecto Académico

Proyecto desarrollado como parte del proceso de aprendizaje de **Desarrollo Frontend con React** en **Desafío Latam**.

---

⭐ **Proyecto desarrollado con React, Vite y consumo de API REST.**
# 🛍️ Mi Marketplace: Aplicación Android con Jetpack Compose

Este proyecto es una aplicación móvil que simula un marketplace o tienda online de productos tecnológicos. Fue desarrollado utilizando **Kotlin** y la interfaz de usuario moderna de **Jetpack Compose** (Material Design 3).

El objetivo principal fue demostrar la implementación de una arquitectura limpia (Modelo-Repositorio) junto con navegación y gestión de estados reactivos en un entorno nativo de Android.

## ✨ Funcionalidades Destacadas (Requisitos y Extras)

El proyecto cumple con todos los requisitos funcionales básicos, además de incorporar **tres extras opcionales** que mejoran la calidad y la experiencia de usuario (UX):

| Requisito | Estado | Implementación Técnica |
| :--- | :--- | :--- |
| **Lista de Productos** | ✅ Completo | Uso de `LazyColumn` para eficiencia. |
| **Pantalla de Detalle** | ✅ Completo | Uso de `verticalScroll` para contenido largo. |
| **Navegación** | ✅ Completo | `Navigation Compose` con paso de argumentos (`productId`). |
| **Repositorio** | ✅ Completo | Clase `ProductRepository` con **7 productos simulados**. |
| **Botón de Interacción** | ✅ Completo | Botón "Añadir al Carrito" en la vista de detalle. |
| **EXTRA: Búsqueda / Filtros** | ⭐ Implementado | Filtrado reactivo en `ProductListScreen` usando `remember` y `mutableStateOf`. |
| **EXTRA: Animaciones (UX)** | ⭐ Implementado | Efecto de elevación (`animateDpAsState`) en las tarjetas al presionar. |
| **EXTRA: Tema Oscuro** | ⭐ Implementado | Detección automática del tema del sistema (`isSystemInDarkTheme`). |

---

## ⚙️ Arquitectura y Estructura del Código

El código sigue una estructura limpia y modular organizada en los siguientes paquetes principales:

1.  **`data` (Modelo y Repositorio):** Define la estructura (`Product.kt`) y la fuente de datos (`ProductRepository.kt`).
2.  **`ui.theme` (Estilos):** Define la paleta de colores personalizada y la lógica de cambio entre **Modo Claro** y **Modo Oscuro**.
3.  **`ui.screens` (Vistas Composable):** Contiene las implementaciones de la lista, el detalle y los componentes interactivos.
4.  **`MainActivity.kt` (Navegación):** Define las rutas (`NavHost`) y el flujo de la aplicación, incluyendo el paso de argumentos.

---




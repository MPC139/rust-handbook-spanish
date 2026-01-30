# Rust HandBook in Spanish 🦀📖

Este proyecto es un manual detallado de Rust escrito totalmente en español, diseñado para explicar conceptos complejos de una manera sencilla, visual e interactiva.

## 🚀 Cómo visualizar el libro

Este proyecto utiliza **mdBook**, el estándar de la comunidad de Rust para crear documentación.

### Requisitos previos
Debes tener instalado `mdbook`. Si no lo tienes, puedes instalarlo con Cargo:
```bash
cargo install mdbook
```

### Ejecución en modo desarrollo
Para ver el libro y que se actualice automáticamente mientras haces cambios:
```bash
mdbook serve --open
```
Esto abrirá tu navegador en `http://localhost:3000`.

### Compilación estática
Si solo quieres generar los archivos HTML:
```bash
mdbook build
```
Los archivos se generarán en la carpeta `book/`.

---

## 📝 Resumen del progreso

Hasta el momento, hemos completado el capítulo de **Smart Pointers**, uno de los temas más desafiantes de Rust.

### Capítulos Desarrollados:

#### 1. Smart Pointers (Punteros Inteligentes) 📦
Se ha creado una guía completa que cubre:
*   **Fundamentos:** Conceptos de Stack vs Heap, y cómo `Box<T>` gestiona datos en el montón.
*   **Traits Mágicos:** Implementación manual y explicación de `Deref` (acceso a datos) y `Drop` (limpieza automática).
*   **Gestión de Memoria:**
    *   `Rc<T>` para propiedad compartida (conteo de referencias).
    *   `Weak<T>` para prevenir ciclos de referencia y fugas de memoria.
*   **Mutabilidad Interior:** Uso de `RefCell<T>` para modificar datos bajo referencias inmutables y la combinación poderosa `Rc<RefCell<T>>`.
*   **Desafío Integrador:** Creación de una estructura de **Árbol Genealógico** que combina todas las herramientas anteriores en un caso de uso real.

#### Próximamente... 🔜
*   **Concurrencia:** Exploraremos cómo Rust garantiza la seguridad en entornos multihilo sin carreras de datos.

---
*Este manual está en constante desarrollo. ¡Sigue explorando la seguridad y potencia de Rust!*

# Rust HandBook in Spanish 🦀📖

Este proyecto es un manual detallado de Rust escrito totalmente en español, diseñado para explicar conceptos complejos de una manera sencilla, visual e interactiva.

## 🛠️ Instalación de Rust y Cargo

Si es tu primera vez con Rust, necesitas instalar el conjunto de herramientas básico. La forma recomendada es a través de **rustup**.

### 1. En Linux o macOS
Abre una terminal y ejecuta el siguiente comando:
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
Sigue las instrucciones en pantalla (normalmente basta con presionar `1` y `Enter`).

### 2. En Windows
Descarga y ejecuta el instalador **rustup-init.exe** desde el sitio oficial:
👉 [rustup.rs](https://rustup.rs/)

> **Nota:** En Windows, es posible que también necesites las "Herramientas de compilación de C++ para Visual Studio". El instalador te guiará si faltan.

### 3. Verificar la instalación
Una vez terminada la instalación, reinicia tu terminal y comprueba que todo funciona:
```bash
rustc --version
cargo --version
```

---

## 🚀 Cómo visualizar el libro

Este proyecto utiliza **mdBook**, el estándar de la comunidad de Rust para crear documentación.

### Requisitos previos
Una vez que tengas Rust instalado, puedes instalar `mdbook` con Cargo:
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

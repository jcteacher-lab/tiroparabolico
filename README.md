# Tiro parabólico

Simulación interactiva del movimiento de un proyectil mediante HTML, CSS y JavaScript.

## Descripción

**Tiro parabólico** es una aplicación web educativa diseñada para visualizar y comprender el movimiento de un proyectil bajo condiciones ideales.

La aplicación permite modificar parámetros iniciales del lanzamiento y observar gráficamente la trayectoria del proyectil mediante un elemento `canvas` de HTML5.

El proyecto está pensado como recurso didáctico para apoyar el estudio de conceptos de **física, cinemática, programación y simulación computacional**.

## Objetivos

- Comprender el comportamiento del movimiento parabólico.
- Visualizar la trayectoria de un proyectil.
- Relacionar variables físicas con su representación gráfica.
- Aplicar conceptos de programación mediante JavaScript.
- Utilizar una simulación computacional como recurso de aprendizaje.

## Tecnologías utilizadas

- **HTML5** — estructura de la aplicación.
- **CSS3** — diseño y presentación de la interfaz.
- **JavaScript** — cálculos, interacción y animación.
- **HTML5 Canvas** — representación gráfica de la trayectoria.
- **GitHub Pages** — publicación de la aplicación web.

## Características

- Simulación interactiva del tiro parabólico.
- Representación gráfica mediante `canvas`.
- Animación de la trayectoria del proyectil.
- Controles para modificar los parámetros del lanzamiento.
- Cálculo de las variables físicas involucradas.
- Aplicación completamente ejecutable desde un navegador web.
- No requiere instalación de software adicional.

# ⚡ Tiro Parabólico Interactivo

Simulador educativo de movimiento de proyectiles (tiro parabólico) desarrollado
en **HTML + CSS + JavaScript** puro con **Canvas 2D**. Autocontenido en un solo
archivo, sin dependencias externas.

---

## ✨ Características

- 🎚️ Controles interactivos de **velocidad inicial** y **ángulo**.
- 🎬 Animación en tiempo real de la trayectoria parabólica.
- 📐 Cálculo automático de **tiempo de vuelo**, **alcance máximo** y **altura máxima**.
- 📋 Tabla de **tabulación por segundo** con posición y velocidad del proyectil.
- 📊 Cuadrícula adaptativa con ejes etiquetados en metros.
- 🌐 Interfaz completamente en **español**.

---

## 🆕 Novedades v2.0.0

- 📋 **Módulo de tabulación por segundo:** nueva tabla en vivo con `t`, `x`, `y`,
  `vₓ` y `v_y`. La fila final (punto de impacto) se resalta en verde.
- 🎨 **Canvas optimizado:** márgenes superior e inferior reducidos para aprovechar
  mejor el espacio vertical de la gráfica.
- 🎨 **Panel lateral ampliado** de `240px` a `260px` para acomodar la tabla.
- ✅ **Módulo 100% aditivo:** no se modificó la lógica del simulador original.

---

## 🚀 Cómo usar

1. Descarga el archivo `tiro_parabolico.html`.
2. Ábrelo con cualquier navegador moderno (Chrome, Firefox, Edge, Safari).
3. Ajusta la **velocidad inicial** y el **ángulo** con los deslizadores.
4. Presiona **🚀 Lanzar proyectil** para ver la animación.
5. Consulta la **tabla de tabulación** para revisar los valores segundo a segundo.

---

## 🎮 Controles del simulador

| Control | Rango | Descripción |
|---|:---:|---|
| Velocidad inicial | 5 – 80 m/s | Magnitud de la velocidad de lanzamiento |
| Ángulo | 5° – 85° | Inclinación respecto a la horizontal |
| Botón Lanzar | — | Inicia la animación de la trayectoria |

### 📤 Salidas en pantalla

- ⏱️ **Tiempo de vuelo** (s)
- 📏 **Alcance máximo** (m)
- 📈 **Altura máxima** (m)
- 📋 **Tabla de tabulación por segundo** con columnas:

  | t (s) | x (m) | y (m) | vₓ (m/s) | v_y (m/s) |
  |:---:|:---:|:---:|:---:|:---:|
  | 0.0 | 0.00 | 0.00 | 21.21 | 21.21 |
  | 1.0 | 21.21 | 16.31 | 21.21 | 11.40 |
  | 2.0 | 42.43 | 22.89 | 21.21 | 1.59 |
  | ... | ... | ... | ... | ... |
  | 4.33 | 91.70 | 0.00 | 21.21 | -21.21 |

  > La última fila (impacto en `t = t_vuelo`) aparece resaltada en **verde**.

---

## 📚 Uso didáctico

Este simulador está pensado para clases de **Física** (MRU, MRUA y tiro parabólico).
Permite al alumno:

- Comparar la **componente horizontal constante** frente a la **componente vertical variable**.
- Construir **tablas experimentales** y contrastarlas con los valores teóricos.
- Verificar las ecuaciones:

$$
R = \frac{v_0^2 \sin(2\theta)}{g}, \quad
H = \frac{v_0^2 \sin^2\theta}{2g}, \quad
t_{vuelo} = \frac{2v_0 \sin\theta}{g}
$$

---

## 🛠️ Tecnologías

- **HTML5**
- **CSS3** (flexbox, grid, backdrop-filter)
- **JavaScript ES6+**
- **Canvas 2D API**
- Sin librerías externas

---

## Modelo físico

La simulación considera un modelo ideal de tiro parabólico, en el que el movimiento puede analizarse mediante dos componentes independientes:

**Movimiento horizontal**

```text
x(t) = v₀ cos(θ) · t
```

**Movimiento vertical**

```text
y(t) = y₀ + v₀ sin(θ) · t - ½gt²
```

donde:

- `v₀` = velocidad inicial.
- `θ` = ángulo de lanzamiento.
- `t` = tiempo.
- `g` = aceleración de la gravedad.
- `x` = posición horizontal.
- `y` = posición vertical.
- `y₀` = altura inicial.

El modelo supone condiciones ideales y no considera factores como resistencia del aire, viento o variaciones locales de la gravedad.

## Ejecución local

No es necesario instalar dependencias.

1. Descarga o clona el repositorio.
2. Abre el archivo `index.html`.
3. Ejecuta el archivo utilizando un navegador web moderno.
4. Interactúa con los controles de la simulación.

También puede ejecutarse directamente mediante un servidor local, por ejemplo utilizando la extensión **Live Server** de Visual Studio Code.

## Publicación mediante GitHub Pages

El proyecto puede publicarse como una página web utilizando **GitHub Pages**.

La estructura mínima recomendada es:

```text
fisica-interactiva/
│
├── index.html
└── README.md
```

Al utilizar `index.html` como archivo principal, GitHub Pages puede servirlo como página inicial del sitio.

La documentación oficial de GitHub explica la configuración de repositorios, archivos README y publicación mediante Pages. 

## Uso educativo

Este proyecto puede utilizarse como apoyo para actividades relacionadas con:

- Cinemática.
- Movimiento bidimensional.
- Tiro parabólico.
- Vectores.
- Componentes de la velocidad.
- Aceleración gravitacional.
- Interpretación de gráficas.
- Programación orientada a la simulación.
- Pensamiento computacional.

## Posibles mejoras

Como proyecto educativo, puede ampliarse incorporando:

- Cálculo del tiempo de vuelo.
- Altura máxima.
- Alcance horizontal.
- Velocidad en diferentes instantes.
- Vector de velocidad.
- Vector de aceleración.
- Comparación entre diferentes ángulos.
- Resistencia del aire.
- Variación de la gravedad.
- Tabla de datos de la trayectoria.
- Exportación de resultados.
- Comparación entre resultados teóricos y simulados.

## Autor

**Juan Carlos Santiago**

Proyecto educativo orientado a la integración de **física, matemáticas, programación y tecnologías web**.

## Licencia

Este proyecto se distribuye bajo los términos de la **GNU General Public License v3.0 (GPL-3.0)**.

La GPL-3.0 permite utilizar, estudiar, modificar y redistribuir el software bajo los términos establecidos por dicha licencia. GitHub identifica `GPL-3.0` como la clave SPDX correspondiente a GNU General Public License v3.0.

Para que la licencia quede correctamente incorporada al repositorio, se recomienda agregar un archivo llamado:

```text
LICENSE
```

y seleccionar **GNU General Public License v3.0** desde GitHub. GitHub recomienda incluir el archivo de licencia en la raíz del repositorio para que pueda detectarse y mostrarse correctamente.

---

**Proyecto educativo — Física + Matemáticas + Programación + Simulación**

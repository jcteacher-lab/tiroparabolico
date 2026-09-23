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

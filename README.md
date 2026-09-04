[README.md](https://github.com/user-attachments/files/31850803/README.md)
# ✨ Frases Motivacionales

Una web minimalista, moderna y fluida para recibir frases motivacionales según tu estado de ánimo. Fondo con orbes animados, textura de ruido sutil, tarjeta con efecto de parallax al mover el mouse y transiciones con blur al cambiar de frase.

## 🌟 Demo

👉 [Ver demo en vivo](https://aadamjpg.github.io/frases-motivacionales/)

> Si tienes GitHub Pages activado en el repo, este es el enlace correcto. Si no, actívalo en `Settings > Pages` y actualiza el link.

## 📖 Descripción

`index.html` es una single-page app sin dependencias externas (salvo Google Fonts) que muestra frases motivacionales aleatorias. Lo particular del proyecto es el sistema de **moods**: cada estado de ánimo tiene su propio set de frases, su propia paleta de color y hasta su propio fondo animado, así que la experiencia cambia completamente según cómo te sientas.

## 🚀 Características

- 🎭 **4 modos de ánimo**, cada uno con frases, colores y gradientes de fondo propios:
  - 🔵 **Normal** — frases clásicas de vida, éxito, fuerza, sabiduría, creatividad y desarrollo personal
  - 🔴 **Mood Malo** — frases crudas para días difíciles
  - 🟠 **Gym 💪** — frases de motivación física y disciplina
  - 🟣 **Cruda Realidad** — frases sin filtro sobre el sistema, el trabajo y la vida
- 🏷️ **Filtro por categorías**: Vida, Éxito, Fuerza, Sabiduría, Creatividad, Personal, Gym, Realidad
- 🎲 Generador de frases aleatorias sin repetir la anterior
- 📋 Botón para **copiar la frase** al portapapeles (con confirmación tipo toast)
- ⌨️ Atajo de teclado: presiona **Espacio** para una nueva frase
- 🖱️ Efecto **parallax 3D** en la tarjeta al mover el mouse
- ✨ Fondo con orbes animados + textura de ruido + partículas al cambiar de frase
- 📱 Totalmente responsive
- ⚡ 100% HTML/CSS/JS vanilla — cero dependencias, cero build

## 🛠️ Tecnologías utilizadas

- HTML5
- CSS3 (custom properties, animaciones, `backdrop-filter`, gradientes)
- JavaScript vanilla (sin frameworks)
- [Google Fonts](https://fonts.google.com/): Inter + Playfair Display

## 📂 Estructura del proyecto

```
├── index.html   # Todo el proyecto: markup, estilos y lógica en un solo archivo
└── README.md
```

## ⚙️ Instalación y uso

No requiere instalación ni build. Solo:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/aadamjpg/frases-motivacionales.git
   ```
2. Abre `index.html` en tu navegador (doble clic, o usa la extensión "Live Server" en VS Code).

## 🎮 Cómo usarlo

1. Elige tu estado de ánimo en el selector superior (**Normal**, **Mood Malo**, **Gym**, **Cruda Realidad**).
2. Filtra por categoría si quieres una temática específica.
3. Haz clic en **"Nueva frase"** o presiona `Espacio` para generar otra.
4. Pasa el mouse sobre la tarjeta y haz clic en **"COPIAR"** para copiar la frase al portapapeles.

## ✏️ Personalización

Todas las frases viven en el objeto `quotesByMood` dentro del `<script>` de `index.html`, organizadas por mood (`normal`, `bad`, `fire`, `real`). Cada frase tiene `text`, `author` y `category`:

```javascript
{ text: "Tu frase aquí.", author: "Autor", category: "vida" }
```

Para añadir una frase, agrégala al array del mood correspondiente. Si usas una categoría nueva, recuerda añadir también su botón en `.categories`.

Para añadir un mood nuevo:
1. Crea un nuevo array dentro de `quotesByMood`.
2. Añade su botón en `.mood-selector` (`data-mood="tu-mood"`).
3. Define sus colores/gradiente en `:root` y las reglas `body.mood-tu-mood`.

## 🤝 Contribuciones

Las contribuciones son bienvenidas, especialmente frases nuevas para cualquiera de los 4 moods.

1. Haz un fork del proyecto
2. Crea una rama (`git checkout -b feature/nuevas-frases`)
3. Haz commit de tus cambios (`git commit -m 'Añade frases de X'`)
4. Sube la rama (`git push origin feature/nuevas-frases`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la licencia MIT. Consulta el archivo `LICENSE` para más detalles.

---

Hecho con 💙 para inspirar (o para decirte la cruda verdad) un poco cada día.

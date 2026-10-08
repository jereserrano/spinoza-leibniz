# ⛵ Spinoza vs. Leibniz — Dos formas de leer el mundo (Travesía Caribeña)

Una experiencia interactiva y académica sobre el choque metafísico del siglo XVII entre **Baruch Spinoza** (monismo sustancial: *Deus sive Natura*) y **Gottfried Wilhelm Leibniz** (pluralismo monadológico y armonía preestablecida), ambientada con un tema luminoso inspirado en el Caribe colombiano y guiada por **tres compañeros interactivos** con voces reales y animaciones fluidas.

---

## 🌐 Enlace del Proyecto Publicado

🔗 **Sitio en vivo:** [https://jereserrano.github.io/spinoza-leibniz/](https://jereserrano.github.io/spinoza-leibniz/)

---

## 🚀 Cómo Ejecutar Localmente

No requiere Node.js, compilación ni frameworks pesados. Todo está construido con estándares web nativos (HTML5, CSS3 moderno, Vanilla JavaScript).

### Opción 1: Servidor HTTP con Python (Recomendado)
Abre PowerShell o terminal en la carpeta del proyecto y ejecuta:
```bash
python -m http.server 8095
```
Luego abre en tu navegador:
```
http://localhost:8095/
```

### Opción 2: Cualquier servidor estático
Puedes usar VS Code Live Server, `npx serve`, o abrir directamente en el navegador.

---

## 📁 Estructura del Proyecto

```
spinoza-leibniz/
├── index.html                               # Aplicación web completa y autónoma
├── README.md                                # Documentación del proyecto
├── assets/
│   ├── audio/
│   │   ├── guide1/                          # 6 audios MP3 del Guía 1 (Voz Real)
│   │   │   ├── guide1_01.mp3 (11s - Bienvenida/Hero)
│   │   │   ├── guide1_02.mp3 (40s - La Pregunta)
│   │   │   ├── guide1_03.mp3 (22s - Spinoza)
│   │   │   ├── guide1_04.mp3 (43s - Leibniz)
│   │   │   ├── guide1_05.mp3 (38s - Comparación)
│   │   │   └── guide1_06.mp3 (22s - Cierre)
│   │   ├── guide2/                          # 11 audios MP3/OGG del Guía 2 (Voz Real)
│   │   │   ├── guide2_01.mp3 (29s - Determinismo)
│   │   │   ├── guide2_02.mp3 (31s - Mónadas)
│   │   │   ├── ...
│   │   │   └── guide2_11.mp3 (38s - Quiz)
│   │   └── guide3/                          # 7 audios MP3 del Guía 3 (Voz Real)
│   │       ├── guide3_01.mp3 (14s - Comparación y Racionalismo)
│   │       ├── guide3_02.mp3 (11s - Pequeñas percepciones y Memoria)
│   │       ├── guide3_03.mp3 (10s - Conatus y Potencia de actuar)
│   │       ├── guide3_04.mp3 (10s - Libertad y Necesidad en Spinoza)
│   │       ├── guide3_05.mp3 (12s - Libertad y Claridad en Leibniz)
│   │       ├── guide3_06.mp3 (13s - Mónadas y Mejor de los mundos)
│   │       └── guide3_07.mp3 (9s - Sustancia única y Deus sive Natura)
│   └── images/                              # Avatares de los guías y recursos visuales
│       ├── guide1.png                       # Avatar Guía 1 (Caricatura 767x1536 PNG)
│       ├── guide2.png                       # Avatar Guía 2 (Caricatura 767x1536 PNG)
│       ├── guide3.png                       # Avatar Guía 3 (Caricatura 767x1536 PNG)
│       ├── stickman.png                     # Stickman base original
│       └── originals/                       # Fotos originales de respaldo
```

---

## 🎓 Modo Exposición (Ideal para Proyectores y Presentaciones)

Diseñado especialmente para exponer ante el profesor y el grupo de clase.

### Cómo activarlo:
- Pulsa el botón **"Exposición"** en el encabezado de navegación o en el pie de página.
- Se abrirá un panel explicativo y al iniciar se activará la vista maximizada para proyector (16:9, 1366×768 o 1920×1080).

### Atajos de Teclado y Control Remoto (Clicker):
| Tecla | Acción |
|---|---|
| `→` / `↓` / `AvPág` | Avanzar a la siguiente sección / diapositiva |
| `←` / `↑` / `RePág` | Retroceder a la diapositiva anterior |
| `Espacio` | Reproducir / Pausar el audio del guía activo |
| `M` | Silenciar / Activar sonido |
| `G` | Mostrar / Ocultar los 3 guías en pantalla |
| `F` | Pantalla completa (Fullscreen API) |
| `Esc` | Salir del Modo Exposición |

---

## 🎙️ Cómo Reemplazar Fotos y Audios

### Para cambiar los Audios:
1. Convierte tus grabaciones a formato `.mp3` (o `.ogg`).
2. Coloca los archivos en la carpeta correspondiente (`assets/audio/guide1/`, `guide2/`, o `guide3/`).
3. En `index.html`, busca el objeto `guideAudioRegistry` (línea ~5025) y actualiza el nombre o ruta del archivo:
   ```javascript
   'guide3_01': 'assets/audio/guide3/mi_nuevo_audio.mp3',
   ```
4. Los comentarios marcados con `// TODO_ASIGNAR_AUDIO` indican las asociaciones temáticas recomendadas.

### Para cambiar las Fotos de los Guías:
1. Guarda la imagen en formato PNG transparente con resolución recomendada `767 × 1536 px`.
2. Reemplaza el archivo directamente en `assets/images/`:
   - `assets/images/guide1.png` para el Guía 1.
   - `assets/images/stickman.png` o `guide2.png` para el Guía 2.
   - `assets/images/guide3.png` para el Guía 3.

---

## 📝 Secciones Académicas y Créditos

Para personalizar los nombres de los expositores, docente o asignatura para tu entrega:
1. Abre `index.html` y busca los comentarios marcados con:
   ```
   // EDITAR_NOMBRES
   ```
2. Modifica el nombre del profesor, la institución y los 3 expositores en la sección `#creditos`.
3. Busca `// EDITAR_FUENTES` para ajustar las citas bibliográficas consultadas.

---

## 🏆 Quiz y Mini-Juego Interactivos

- **Quiz Filosófico:** 10 preguntas conceptuales rigurosas con indicador de racha de aciertos (`🔥 Racha`), retroalimentación explicativa inmediata, cálculo de rango académico (Sabio, Pensador, Aprendiz, Explorador) y persistencia del mejor puntaje en `localStorage`.
- **Mini-Juego "¿Spinoza o Leibniz?":** 8 afirmaciones ontológicas para poner a prueba la rapidez mental distinguiendo entre monismo sustancial y monadología.

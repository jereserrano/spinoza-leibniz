# Leibniz y Spinoza: dos formas de leer el mundo 🌴🌊

Una experiencia web educativa e interactiva universitaria que explora y compara las filosofías racionalistas de **Baruch Spinoza** y **Gottfried Wilhelm Leibniz** en torno a la realidad, Dios/la Naturaleza, el alma y el cuerpo, la libertad y las emociones.

---

## 📖 Descripción

Este proyecto transforma una presentación académica tradicional en una **experiencia interactiva inmersiva** con estética moderna y temática caribeña. Diseñado para exposiciones universitarias, el sitio permite a estudiantes y docentes interactuar con conceptos clave del racionalismo moderno mediante simulaciones visuales, controles deslizantes pedagógicos, sintetizador de voz y desafíos de conocimiento en tiempo real.

---

## 🛠️ Tecnologías Utilizadas

- **HTML5**: Estructura semántica accesible y metadatos SEO.
- **CSS3 (Vanilla)**: Diseño adaptable, glassmorphism, gradientes HSL y transiciones fluidas.
- **JavaScript (Vanilla)**: Lógica interactiva reactiva y manipulación del DOM.
- **Lucide Icons**: Iconografía vectorial nítida y consistente.
- **Google Fonts**: Tipografías modernas *Inter* y *Outfit*.
- **Web Speech API (`SpeechSynthesis`)**: Narración auditiva interactiva en español.
- **Web Audio API**: Generación de efectos de sonido procedurales (*chime* armónico).
- **HTML5 Canvas**: Sistema de partículas ambientales de fondo con respeto a `prefers-reduced-motion`.

---

## ✨ Funcionalidades

1. **Recorrido Interactivo (El Viajero en Barco)**:
   - Mapa con 5 estaciones históricas (*Inicio*, *Spinoza*, *Leibniz*, *Comparación*, *Quiz*).
   - Movimiento fluido del viajero y lectura interactiva de las explicaciones al hacer clic.

2. **Perfiles Filosóficos y Conceptos Expandibles**:
   - **Spinoza**: *Deus sive Natura*, *Determinismo* y *Conatus* con tarjetas expandibles interactivas.
   - **Leibniz**: *Mónadas / Unidades simples*, *Armonía preestablecida* y *Pequeñas percepciones*.

3. **Elige tu Ruta**:
   - Selector interactivo entre la **Ruta Spinoza** (unidad e inmanencia) y la **Ruta Leibniz** (multiplicidad y armonía).

4. **Alma y Cuerpo (Slider Interactivo)**:
   - Control deslizante que transforma visualmente la relación entre mente y cuerpo, desde la sincronización armónica de Leibniz hasta el paralelismo atributivo de Spinoza.

5. **¿Dónde queda la Libertad? (Espectro Dinámico)**:
   - Control deslizante que recorre el espectro desde el *Capricho* hasta la *Comprensión racional de las causas*.

6. **Selector de Emociones**:
   - Análisis comparativo interactivo de 6 emociones (*Alegría*, *Tristeza*, *Deseo*, *Sorpresa*, *Miedo*, *Calma*) vistas desde los afectos de Spinoza y las percepciones de Leibniz.

7. **Duelo de Ideas y Duelo Filosófico**:
   - Tabla comparativa detallada punto a punto.
   - Preguntas cara a cara con respuestas sintéticas de ambos autores (*¿Qué es la realidad?*, *¿Somos libres?*, etc.).

8. **Mini-Juego: ¿Spinoza o Leibniz?**:
   - 8 afirmaciones filosóficas para poner a prueba a la audiencia en vivo con retroalimentación explicativa inmediata.

9. **Quiz Filosófico Completo**:
   - 10 preguntas pedagógicas con retroalimentación al instante, barra de progreso y sistema de rangos y medallas (*Explorador filosófico*, *Aprendiz del racionalismo*, *Pensador destacado*, *Maestro del debate filosófico*).

10. **Diseño Responsive y Accesibilidad**:
    - Optimizado para pantallas de escritorio, portátiles, tablets y teléfonos móviles (360px a 1440px+).
    - Barra de navegación con indicador de scroll y menú móvil.

---

## 🚀 Ejecución Local

Para ejecutar el proyecto localmente sin necesidad de instalar dependencias ni herramientas adicionales:

1. Clona el repositorio:
   ```bash
   git clone https://github.com/jereserrano/spinoza-leibniz.git
   ```
2. Abre la carpeta del proyecto y haz doble clic en `index.html` en tu navegador preferido (Chrome, Edge, Firefox, Safari).
3. Opcionalmente, puedes servirlo con cualquier servidor local ligero:
   ```bash
   # Con Python
   python -m http.server 8000
   ```
   Luego visita `http://localhost:8000`.

---

## 🌐 Publicación en GitHub Pages

El proyecto está completamente preparado para alojarse como sitio estático en **GitHub Pages**.
Una vez activado desde `Settings > Pages`, el sitio queda disponible públicamente en:

**`https://jereserrano.github.io/spinoza-leibniz/`**

---

## 📂 Estructura del Proyecto

```text
spinoza-leibniz/
│
├── index.html                           # Punto de entrada principal
├── spinoza_vs_leibniz_interactivo-2.html # Copia de respaldo original
│
├── assets/
│   ├── audio/                           # Estructura preparada para grabaciones reales
│   │   ├── spinoza/
│   │   ├── leibniz/
│   │   └── narracion/
│   ├── images/
│   ├── icons/
│   └── fonts/
│
├── css/
├── js/
├── .gitignore
└── README.md
```

---

## 🎙️ Próximas Actualizaciones

- Incorporación de pistas de voz reales grabadas por los integrantes del equipo en `assets/audio/` para reemplazar progresivamente la síntesis de voz del navegador.

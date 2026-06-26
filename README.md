# 📁 Resumen del Proyecto — App de Planeación Didáctica

> **Propósito de la carpeta:** Repositorio educativo con juegos interactivos en HTML para niños de Fase 2 (Preescolar 1°, 2° y 3°), alineados a la **Nueva Escuela Mexicana (NEM)**. Desarrollado para apoyar la práctica docente con herramientas digitales accesibles y sin conexión a internet.

---

## 🗂️ Estructura de Archivos

```
App de planeacion/
│
├── index.html                        ← Juego: Canastas Numéricas 🧺🍎
├── oficios_tecolotlan.html           ← Juego: Oficios de Tecolotlán 🏘️
│
├── instructivo_canastas.md           ← Instructivo pedagógico: Canastas Numéricas
├── instructivo_uso.md                ← Instructivo de uso: Oficios de Tecolotlán
├── planeacion didactica.md           ← Planeación didáctica general del proyecto
├── README.md                         ← Este documento de resumen
│
├── images/                           ← Imágenes de personajes del juego de oficios
│   ├── bombero.png
│   ├── campesino.png
│   ├── comerciante.png
│   ├── cover.png
│   └── policia.png
│
├── LESLIE/                           ← Juego: Mi Lonchera Saludable 🍱
│   ├── index.html
│   └── README.md
│
└── Juegos de numeros/               ← Juegos numéricos adicionales
    ├── MEMORAMA NIVELES.html
    └── index (1).html
```

---

## 🎮 Juegos Incluidos

### 1. 🧺 Canastas Numéricas (`index.html`)

| Dato | Descripción |
|------|------------|
| **Propósito** | Relacionar números con cantidades arrastrando manzanas a canastas |
| **Edades** | 3 a 6 años (Fase 2 Preescolar) |
| **Campo Formativo** | Saberes y Pensamiento Científico |
| **PDA** | Conteo, correspondencia uno a uno, cardinalidad, relación número–cantidad |
| **Niveles** | Fácil (1–3) · Medio (1–5) · Difícil (1–10) |
| **Tecnología** | HTML5 + CSS3 + JS puro. Drag & Drop táctil y mouse |
| **Audio** | Web Audio API (sonidos sintetizados) + SpeechSynthesis (voz en español) |

#### Cómo se juega
1. **Selecciona el nivel** de dificultad al abrir la app.
2. **Arrastra manzanas** 🍎 desde la zona inferior hacia las canastas.
3. Cada canasta tiene un número que indica cuántas manzanas debe contener.
4. Cuando creas que terminaste, presiona **"¡Verificar canastas! 🔍"**
   - ✅ Canasta con cantidad correcta → se pone **verde**
   - ❌ Canasta con cantidad incorrecta → se pone **rojo** (puedes corregir)
5. Al completar todas correctamente → **lluvia de confeti y música de victoria** 🎉

#### PDA que favorece por grado

| Grado | PDA |
|-------|-----|
| **1° Preescolar** (3–4 años) | Usa números en juegos y situaciones cotidianas · Cuenta objetos |
| **2° Preescolar** (4–5 años) | Compara colecciones · Determina más, menos o igual cantidad |
| **3° Preescolar** (5–6 años) | Relaciona cantidad con número cardinal escrito · Construye y compara colecciones |

#### ¿Qué favorece en el desarrollo infantil?
- 🧠 **Pensamiento Lógico-Matemático:** del conteo concreto a la abstracción numérica
- ✋ **Coordinación Viso-Motriz Fina:** arrastrar y soltar con control
- 🪞 **Autoevaluación y Autonomía:** el niño verifica por sí mismo y corrige sin presión
- 🔇 **Accesibilidad:** instrucciones en audio para niños que aún no leen

---

### 2. 🏘️ Oficios de Tecolotlán (`oficios_tecolotlan.html`)

| Dato | Descripción |
|------|------------|
| **Contexto** | Ambientado en Tecolotlán, Jalisco |
| **Objetivo** | Que el niño reconozca que las personas trabajan para el bienestar de su comunidad |
| **Edades** | 3 a 6 años (Fase 2 Preescolar) |
| **Campos Formativos** | Ética, Naturaleza y Sociedades · De lo Humano y lo Comunitario · Lenguajes |

#### Módulos del juego
| Módulo | Descripción |
|--------|-------------|
| 🎁 **Cajita Misteriosa** | El niño saca herramientas de una caja y las clasifica entre Campesino 🧑‍🌾 o Comerciante 🏪 |
| 🍕 **Pizza Numérica** | Siguiendo instrucciones de audio, coloca una cantidad específica de ingredientes en una pizza. Tiene 3 niveles de dificultad |
| 🎡 **Feria de Profesiones** | Explora tarjetas de trabajadores y escucha en audio la importancia de cada oficio para la comunidad |

---

### 3. 🍱 Mi Lonchera Saludable (`LESLIE/index.html`)

| Dato | Descripción |
|------|------------|
| **Campo Formativo** | De lo Humano y lo Comunitario |
| **Eje Articulador** | Vida Saludable |
| **Contenido** | Consumo de alimentos y bebidas que benefician la salud |
| **Edades** | Preescolar Fase 2 (1°, 2° y 3°) |

#### PDA por grado

| Grado | PDA |
|-------|-----|
| **1°** | Compara alimentos saludables de los que no lo son |
| **2°** | Distingue alimentos y bebidas saludables de los que ponen en riesgo la salud |
| **3°** | Obtiene información sobre beneficios de alimentos saludables y agua simple para diseñar menús y loncheras balanceadas |

#### Características
- 🥦 **Plato del Bien Comer interactivo** (clasificación por grupos alimenticios)
- 🔊 **Síntesis de Voz:** pronuncia nombres de alimentos y guía al niño
- 📊 **Indicador de Balance** dinámico de la lonchera
- ⚠️ **Sección de alimentos ocasionales/chatarra** con advertencias amigables

---

### 4. 🔢 Juegos Numéricos Adicionales (`Juegos de numeros/`)

| Archivo | Descripción |
|---------|-------------|
| `MEMORAMA NIVELES.html` | Juego de memoria con niveles de dificultad progresivos |
| `index (1).html` | Juego numérico interactivo adicional |

---

## 📋 Planeación Didáctica General

**Tema:** ¿Por qué son importantes los oficios y profesiones?

| Elemento | Descripción |
|----------|-------------|
| **Objetivo** | Evaluar si el niño reconoce que las personas realizan actividades para el beneficio de su comunidad |
| **Valor** | Sentido del Bien Común |
| **Público** | Niños de Preescolar (3–6 años) |
| **Estilo Visual** | Colores llamativos, emojis, estilo caricatura |
| **Accesibilidad** | Uso mínimo de texto — toda la navegación guiada por **instrucciones en audio** |

---

## 🛠️ Tecnología Usada

Todos los juegos están construidos como **archivos HTML independientes** que funcionan sin internet y sin instalación.

| Tecnología | Uso |
|-----------|-----|
| **HTML5** | Estructura de los juegos |
| **CSS3** | Animaciones, gradientes, diseño responsivo |
| **JavaScript ES6** | Lógica de juego, arrastrar y soltar |
| **Web Audio API** | Sonidos generados en tiempo real (sin archivos externos) |
| **SpeechSynthesis API** | Instrucciones de voz en español automáticas |
| **Canvas API** | Animación de confeti en pantallas de victoria |

---

## 💡 Recomendaciones de Uso Docente

> [!TIP]
> Utiliza **Google Chrome** o **Microsoft Edge** para mejor compatibilidad de la síntesis de voz en español.

- 🔊 **Asegúrate de tener el volumen encendido** para que los niños puedan escuchar las instrucciones.
- 👩‍🏫 **Primera sesión con acompañamiento:** aunque los juegos son autónomos, acompaña al niño en la primera partida para orientar el uso táctil o del mouse.
- 💬 **Preguntas de reflexión después del juego:**
  - *"¿Cuántas manzanas pusiste en la canasta?"*
  - *"¿Cómo supiste que eran suficientes?"*
  - *"¿Qué oficio te gustaría tener de grande?"*
  - *"¿Por qué es importante comer sano?"*
- 📱 **Compatible con tabletas y celulares** (pantalla táctil).

---

## 🚀 Despliegue en GitHub Pages

Para que cualquier persona pueda jugar desde el navegador sin descarga:

1. Ve al repositorio en GitHub.
2. Entra a **Settings > Pages**.
3. En *Source*, selecciona la rama `main` y carpeta `/ (root)`.
4. Guarda y en unos minutos obtendrás un enlace público para compartir con alumnos y familias.

---

*Proyecto educativo desarrollado para el nivel Preescolar — Fase 2 · Nueva Escuela Mexicana (NEM) · Tecolotlán, Jalisco.*

# 🧺🍎 Canastas Numéricas — Juegos Educativos de Matemáticas

**Aprendizaje temprano de números y cantidades para niños de 4 a 7 años**

![Licencia: MIT](https://img.shields.io/badge/Licencia-MIT-green.svg)
![Estado: Activo](https://img.shields.io/badge/Estado-Activo-brightgreen)

---

## 📖 Descripción

**Canastas Numéricas** es un proyecto de **juegos educativos interactivos** diseñados para que niños en edad preescolar y primeros años de primaria aprendan a **relacionar números con cantidades** a través de actividades lúdicas y multisensoriales.

El proyecto incluye dos juegos:

| Juego | Descripción | Mecánica |
|-------|-------------|----------|
| 🍎 **Canastas Numéricas** | Coloca manzanas en canastas según el número indicado | Arrastrar y soltar (drag & drop) |
| 🐧 **Aventura Backyardigans** | Ayuda a los personajes a resolver problemas numéricos | Selección múltiple contextualizada |

---

## 🎯 Propósito Educativo

### Objetivo General

> Que el niño o niña sea capaz de **relacionar cantidades discretas con sus correspondientes numerales (1-10)**, desarrollando habilidades de conteo, correspondencia uno a uno y cardinalidad.

### Habilidades que desarrolla

- 🔢 **Conteo uno a uno**: Asignar un número a cada objeto contado
- 🎯 **Correspondencia número-cantidad**: Asociar un numeral con un grupo de objetos
- ✅ **Cardinalidad**: Reconocer que el último número contado representa el total
- 🧠 **Autoverificación**: Revisar y corregir el propio trabajo
- 🤲 **Coordinación motriz fina**: Arrastrar objetos en pantalla táctil

### Niveles de Dificultad

| Nivel | Rango numérico | Edad sugerida | Color |
|-------|----------------|---------------|-------|
| 🟢 **Fácil** | 1 - 3 | 4-5 años | Verde |
| 🟡 **Medio** | 1 - 5 | 5-6 años | Amarillo |
| 🔴 **Difícil** | 1 - 10 | 6-7 años | Rojo |

---

## 🧠 Fundamentación Pedagógica

Todo el diseño del proyecto está respaldado por principios pedagógicos explícitos. La documentación completa se encuentra en la carpeta [`docs/`](./docs/).

| Documento | Contenido |
|-----------|-----------|
| [📄 01 - Fundamentos Pedagógicos](./docs/01-fundamentos-pedagogicos.md) | Constructivismo (Piaget), ZDP (Vygotsky), Carga Cognitiva (Sweller), DUA (CAST), Aprendizaje Matemático Temprano (Clements & Sarama), Feedback (Hattie) |
| [📄 02 - Perfil del Aprendiz](./docs/02-perfil-aprendiz.md) | Características cognitivas, motoras, socioemocionales y socioculturales del usuario objetivo |
| [📄 03 - Objetivos de Aprendizaje](./docs/03-objetivos-aprendizaje.md) | Objetivos por juego, alineación con estándares SEP y Common Core, taxonomía de Bloom |
| [📄 04 - Secuencias Didácticas](./docs/04-secuencias-didacticas.md) | Secuencias detalladas de juego, estrategias de andamiaje y actividades de transferencia |
| [📄 05 - Accesibilidad e Inclusión](./docs/05-accesibilidad-e-inclusion.md) | DUA aplicado, adecuaciones por discapacidad, checklist WCAG 2.1 AA y plan de mejora |
| [📄 06 - Evaluación y Retroalimentación](./docs/06-evaluacion-y-retroalimentacion.md) | Sistema de evaluación formativa, tipos de feedback, dashboard de progreso y metacognición |

---

## ✨ Características Técnicas

- ✅ **100% HTML/CSS/JS puro** — Sin frameworks ni dependencias pesadas
- ✅ **Funciona sin internet** (*offline-first*) — Una vez cargado, no requiere conexión
- ✅ **Síntesis de voz** — Instrucciones habladas para niños que aún no leen
- ✅ **Sonidos sintetizados** — Efectos mediante Web Audio API, sin archivos de audio externos
- ✅ **Soporte táctil** — Compatible con tablets y pantallas táctiles
- ✅ **Responsive** — Adaptable a diferentes tamaños de pantalla
- ✅ **Sin publicidad ni rastreadores** — Experiencia segura para niños

---

## 🚀 Cómo Usar

### Opción 1: Abrir directamente (más simple)

Abre cualquiera de estos archivos en tu navegador:

```
index.html              → Canastas Numéricas
aventura_numerica.html  → Aventura Backyardigans
```

### Opción 2: Servidor local (recomendado para aulas)

```bash
# Con Python 3
python -m http.server 8000

# Con Node.js (npx)
npx serve .

# Luego abre http://localhost:8000 en el navegador
```

> 💡 **Recomendación para docentes**: Abre el juego en una tablet o computadora y permite que los niños exploren libremente. Acompaña la primera sesión para modelar el lenguaje matemático.

---

## 🗺️ Roadmap

### Fase 1 — Base (completada)
- ✅ Juego "Canastas Numéricas" funcional con 3 niveles
- ✅ Juego "Aventura Backyardigans" con 3 niveles temáticos
- ✅ Síntesis de voz y sonidos
- ✅ Documentación pedagógica completa

### Fase 2 — Accesibilidad (próximo)
- [ ] ARIA labels y roles semánticos
- [ ] Modo de selección (clic alternativo al arrastre)
- [ ] Feedback multimodal (íconos + color)
- [ ] Soporte de teclado completo
- [ ] Modo concentración (sin distractores)

### Fase 3 — Evaluación y Progreso
- [ ] Sistema de estrellas y logros
- [ ] Dashboard de progreso (localStorage)
- [ ] Reporte para adultos (docentes/padres)
- [ ] Pistas progresivas (andamiaje dinámico)

### Fase 4 — Expansión
- [ ] Banco de niveles procedural (variedad infinita)
- [ ] Más personajes y temáticas
- [ ] Modo multijugador local por turnos
- [ ] PWA (Progressive Web App) instalable

---

## 🤝 Contribuir

¿Eres docente, desarrollador o diseñador instruccional? ¡Las contribuciones son bienvenidas!

### Formas de contribuir

1. **Reportar bugs o ideas** → Abre un issue
2. **Mejorar la accesibilidad** → Revisa el [checklist WCAG](./docs/05-accesibilidad-e-inclusion.md#4-checklist-de-accesibilidad-wcag-21-aa)
3. **Traducir** a otras lenguas (inglés, portugués, lenguas indígenas)
4. **Probar en aula** y compartir resultados

---

## 📄 Licencia

Este proyecto está bajo la licencia MIT.

---

> *"Dime y lo olvido, enséñame y lo recuerdo, involúcrame y lo aprendo."* — Benjamín Franklin
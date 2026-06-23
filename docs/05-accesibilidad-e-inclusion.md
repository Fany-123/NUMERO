# 05 — Accesibilidad e Inclusión

## 1. Principio Rector

> **"Ningún niño debería quedar excluido de la experiencia de aprendizaje por una barrera de diseño."**

Este proyecto se adhiere al **Diseño Universal para el Aprendizaje (DUA)**, que propone tres principios fundamentales:

1. **Múltiples formas de representación** (el "qué" del aprendizaje)
2. **Múltiples formas de acción y expresión** (el "cómo" del aprendizaje)
3. **Múltiples formas de compromiso** (el "por qué" del aprendizaje)

---

## 2. Pautas DUA — Implementación Actual y Mejora

### 2.1 Representación: Proporcionar opciones para la percepción

| Pauta | Implementación actual | Mejora propuesta | Prioridad |
|-------|---------------------|------------------|-----------|
| **1.1** Ofrecer alternativas para la información visual | Los números se muestran grandes y con alto contraste | Añadir **representación táctil** (vibración en dispositivos compatibles) al colocar una manzana | Media |
| **1.2** Ofrecer alternativas para la información auditiva | Hay síntesis de voz (TTS) | Añadir **subtítulos** a las instrucciones habladas | **Alta** |
| **1.3** Ofrecer alternativas para la información visual/auditiva | Combinación de texto + íconos + voz | Añadir **representación con lenguaje de señas** (video embed) para niños sordos | Baja (fase 2) |

### 2.2 Acción y Expresión: Proporcionar opciones para la interacción física

| Pauta | Implementación actual | Mejora propuesta | Prioridad |
|-------|---------------------|------------------|-----------|
| **4.1** Variar los métodos de respuesta | Arrastrar y soltar + clic táctil | Añadir **modo de un solo clic** (tocar la manzana, luego tocar la canasta) para niños con dificultades motoras | **Alta** |
| **4.2** Optimizar el acceso a herramientas y tecnologías de asistencia | — | Asegurar compatibilidad con **lectores de pantalla** (NVDA, VoiceOver) usando ARIA labels | **Alta** |
| **5.1** Usar múltiples medios de comunicación | — | Añadir **opción de respuesta oral** (Web Speech API para reconocimiento de voz) | Media |

### 2.3 Compromiso: Proporcionar opciones para captar el interés

| Pauta | Implementación actual | Mejora propuesta | Prioridad |
|-------|---------------------|------------------|-----------|
| **7.1** Optimizar la elección individual y la autonomía | El niño elige nivel, momento de verificar | Añadir **personalización**: nombre del niño, avatar, tema de colores | Media |
| **7.2** Optimizar la relevancia, el valor y la autenticidad | Contexto de canastas y comida, personajes familiares | Añadir **temáticas intercambiables** (espacio, dinosaurios, granja) | Baja |
| **8.3** Fomentar la colaboración y la comunidad | — | **Modo multijugador** local por turnos (2 niños comparten la pantalla) | Media |

---

## 3. Adecuaciones por Tipo de Discapacidad

### 3.1 Discapacidad Visual

| Barrera | Solución |
|---------|----------|
| No puede ver los números en la canasta | **Síntesis de voz** ya implementada. Al tocar una canasta, dice el número. |
| No puede ver las manzanas | **Etiquetas ARIA** en cada elemento interactivo. El lector de pantalla debe poder navegar todo el juego. |
| No puede ver los colores de feedback (verde/rojo) | **Feedback multimodal**: además del color, incluir un ícono (✔️/❌), vibración (éxito/error), y cambio de texto. |
| Daltonismo (no distingue verde/rojo) | Usar **formas y patrones** además de color. Ejemplo: canasta correcta = borde punteado ✓, incorrecta = borde rayado X. |

**Estándar**: WCAG 2.1 Nivel AA — Contraste de color mínimo 4.5:1 para texto normal.

✅ **Estado actual**: El contraste de los números (fondo amarillo brillante, texto marrón oscuro) cumple. Sin embargo, el feedback verde/rojo podría no ser distinguible para personas con daltonismo protanopia/deuteranopia.

---

### 3.2 Discapacidad Auditiva

| Barrera | Solución |
|---------|----------|
| No escucha las instrucciones habladas | **Subtítulos/transcripciones** visibles de las instrucciones. Actualmente la instrucción se habla pero **no se muestra por escrito**. |
| No escucha los sonidos de éxito/error | **Feedback visual reforzado**: animación más evidente, vibración, cambio de color más marcado. |

✅ **Estado actual**: No hay subtítulos para las instrucciones. Mejora crítica.

---

### 3.3 Discapacidad Motora

| Barrera | Solución |
|---------|----------|
| No puede arrastrar con precisión | **Modo selección**: tocar manzana → se agranda → tocar canasta destino. El área de drop debe ser mín. 48x48dp. |
| Temblor o movimientos involuntarios | Aumentar **tolerancia de zona**: la manzana se "adhiere" a la canasta más cercana al soltar. |
| Uso de dispositivo con switch (barrido) | Navegación secuencial por tabulación, con estados `:focus` visibles. |

✅ **Estado actual**: Solo soporta arrastrar. No hay modo alternativo.

---

### 3.4 Discapacidad Cognitiva / TDAH

| Barrera | Solución |
|---------|----------|
| Dificultad para mantener atención | **Modo concentración**: sin nubes decorativas, sin animaciones de fondo, colores sólidos. |
| Procesamiento lento | **Tiempo ilimitado** en todas las actividades (ya implementado). Sin temporizador. |
| Sobrecarga sensorial | Opción de **desactivar sonidos** y **reducir animaciones** (prefers-reduced-motion). |

✅ **Estado actual**: No hay modo concentración ni control de sonido/animaciones.

---

### 3.5 Espectro Autista (TEA)

| Barrera | Solución |
|---------|----------|
| Ansiedad ante lo impredecible | **Rutina predecible**: misma estructura cada vez que se juega. No hay elementos sorpresa inesperados. |
| Hipersensibilidad auditiva | Los sonidos deben ser **suaves, no abruptos**. Opción de silenciar completamente. |
| Dificultad con instrucciones implícitas | Las instrucciones deben ser **explícitas y literales**: "Arrastra una manzana roja a la canasta que tiene el número tres." |

✅ **Estado actual**: La estructura es predecible, buena. Los sonidos son sintetizados (no samples agresivos).

---

## 4. Checklist de Accesibilidad (WCAG 2.1 AA)

| Criterio | Estado | Notas |
|----------|--------|-------|
| **1.1.1** Contenido no textual | ⚠️ Parcial | Las manzanas no tienen texto alternativo |
| **1.2.1** Sólo audio y sólo vídeo (grabado) | ❌ No aplica | No hay contenido multimedia grabado |
| **1.3.1** Información y relaciones | ⚠️ Parcial | Las canastas no tienen roles ARIA explícitos |
| **1.4.1** Uso del color | ❌ No cumple | Feedback verde/rojo sin alternativa |
| **1.4.3** Contraste (mínimo) | ✅ Cumple | Los números tienen alto contraste |
| **1.4.4** Cambio de tamaño del texto | ✅ Cumple | Uso de unidades relativas |
| **2.1.1** Teclado | ❌ No cumple | Arrastrar requiere mouse/táctil |
| **2.4.7** Foco visible | ❌ No cumple | Sin estilos de foco para teclado |
| **3.3.2** Etiquetas o instrucciones | ⚠️ Parcial | Instrucciones solo habladas, no escritas permanentemente |
| **4.1.2** Nombre, función, valor | ❌ No cumple | Elementos sin ARIA labels |

---

## 5. Plan de Mejora Priorizado

### Fase 1 — Crítica (Semana 1-2)

| Tarea | Criterio WCAG |
|-------|---------------|
| Añadir ARIA labels a todos los elementos interactivos | 4.1.2 |
| Añadir subtítulos/instrucciones escritas visibles | 1.2.1, 3.3.2 |
| Añadir feedback multimodal (íconos + color) para éxito/error | 1.4.1 |
| Soporte básico de teclado (Tab + Enter para seleccionar) | 2.1.1 |
| Estados de foco visibles | 2.4.7 |

### Fase 2 — Importante (Semana 3-4)

| Tarea | Criterio WCAG |
|-------|---------------|
| Modo de selección (clic en vez de arrastre) | 2.1.1 |
| Opción de desactivar sonidos | — |
| Controles de animación (prefers-reduced-motion) | — |
| Roles de región ARIA (banner, main, contentinfo) | 1.3.1 |

### Fase 3 — Deseable (Futuro)

| Tarea | Prioridad |
|-------|-----------|
| Reconocimiento de voz como entrada | Media |
| Compatibilidad con lectores de pantalla (VoiceOver, TalkBack) validada | Alta |
| Personalización de tema (alto contraste, modo oscuro) | Media |
| Traducción a lenguas indígenas (náhuatl, maya, etc.) | Baja |

---

## 6. Referencias

- CAST (2018). *Universal Design for Learning Guidelines version 2.2*.
- W3C/WAI (2018). *Web Content Accessibility Guidelines (WCAG) 2.1*.
- UNICEF (2020). *Inclusive Education: Including Children with Disabilities in Quality Learning*.

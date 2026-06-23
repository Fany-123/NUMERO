# 02 — Perfil del Aprendiz

## 1. Usuario Primario

### Datos demográficos

| Atributo | Valor |
|----------|-------|
| **Rango de edad** | 4 a 7 años (preescolar a 1° de primaria) |
| **Etapa de desarrollo** | Preoperacional (Piaget) — pensamiento intuitivo, egocentrismo limitado, lenguaje en expansión |
| **Escolaridad** | Preescolar (3° grado), Transición, o 1° de primaria |
| **Contexto típico** | Aula de clases, sala de computación, tablet en casa, sesión de terapia |

### Habilidades previas esperadas

| Habilidad | Sí/No | Notas |
|-----------|-------|-------|
| Reconocer números del 1 al 5 | ✔️ Deseable (no obligatorio) | El juego enseña esto |
| Contar objetos hasta 10 | ✔️ Deseable | |
| Usar un dispositivo táctil (arrastrar, tocar) | ✔️ Deseable | Muchos niños de 4+ ya lo hacen |
| Leer palabras completas | ❌ No se asume | Por eso usamos voz y símbolos |
| Escribir números | ❌ No se requiere | La respuesta es siempre selección/arrastre |
| Mantener atención por 10+ minutos | ⚠️ Variable | El juego se diseña en sesiones cortas (3-5 min por nivel) |

---

## 2. Desarrollo Cognitivo (4–7 años)

Basado en Piaget, su teoría del desarrollo cognitivo y hallazgos de neurociencia educativa.

### Capacidades presentes

| Capacidad | Descripción | Implicación en el juego |
|-----------|-------------|-------------------------|
| **Pensamiento concreto** | Necesitan objetos físicos o representaciones visuales para pensar | Las manzanas, canastas y personajes son representaciones concretas |
| **Centración** | Tienden a concentrarse en un solo aspecto del problema | El diseño guía la atención al número-cantidad |
| **Irreversibilidad** | Dificultad para imaginar una acción en reversa | Verificar las canastas les ayuda a "revisar" su trabajo |
| **Lenguaje egocéntrico** | Hablan en voz alta mientras juegan (autoregulación) | El juego puede reforzar con voz externa |
| **Clasificación** | Pueden agrupar objetos por un criterio | Las canastas son categorías numéricas |
| **Correspondencia uno a uno** | Pueden asignar un objeto a otro | Cada manzana se coloca en una canasta específica |

### Capacidades en desarrollo

| Capacidad | Emerge alrededor de | Cómo la apoyamos |
|-----------|-------------------|------------------|
| **Conservación del número** | 6-7 años | Mostrar explícitamente que 3 manzanas en una fila = 3 esparcidas |
| **Seriación** (ordenar por tamaño/cantidad) | 5-7 años | Propuesta: nivel donde se ordenen canastas de menor a mayor |
| **Conteo con cardinalidad** | 4-5 años | La verificación final refuerza que "hay X manzanas porque es el número en la canasta" |
| **Subitización** (reconocer sin contar) | 3-4 años (hasta 3) | Nivel fácil está optimizado para esto |

> **Referencia**: Sarama, J., & Clements, D. H. (2009). *Early Childhood Mathematics Education Research: Learning Trajectories for Young Children*. Routledge.

---

## 3. Perfil Motor

### Habilidades motoras finas esperadas

| Edad | Habilidad | Relevancia |
|------|-----------|------------|
| 4 años | Pinza digital (dedo índice y pulgar) | Arrastrar manzanas en pantalla táctil |
| 4-5 años | Coordinación ojo-mano para arrastrar objetos en pantalla | El área de drop debe ser generosa (target grande) |
| 5-6 años | Mayor precisión en movimientos finos | Canastas objetivo deben tener zona amplia de detección |
| 6-7 años | Control proporcional al adulto (en desarrollo) | Pueden manejar interacciones más complejas |

⚙️ **Implicación técnica**: Las zonas táctiles (canastas, botones) deben tener al menos **48x48dp de área mínima** (recomendación WCAG), y preferiblemente 60x60dp para niños pequeños.

---

## 4. Perfil Socioemocional

### Características relevantes

- **Motivación intrínseca**: Los niños de esta edad disfrutan el juego por el juego mismo. La mecánica de arrastrar manzanas es intrínsecamente satisfactoria.
- **Sensibilidad al error**: Los niños pequeños pueden frustrarse fácilmente. El feedback debe ser **amable y constructivo**.
- **Necesidad de logro**: La celebración (confeti, sonidos, estrellas) refuerza la autoeficacia.
- **Atención dividida**: Pueden distraerse con elementos periféricos. El diseño debe minimizar distracciones.

### Necesidades afectivas

| Necesidad | Estrategia |
|-----------|------------|
| Seguridad psicológica | Los errores se enmarcan como "oportunidad de revisar", no como fracaso |
| Sentido de competencia | El nivel fácil garantiza éxito temprano |
| Autonomía | El niño decide cuándo verificar, cuándo regresar al menú |
| Pertenencia | Personajes familiares (Backyardigans) generan conexión emocional |

---

## 5. Perfil Sociocultural

### Consideraciones

| Aspecto | Consideración |
|---------|---------------|
| **Idioma** | Español (México / América Latina). Adaptable a otras variantes. |
| **Acceso tecnológico** | Puede variar: tablet compartida en aula, dispositivo familiar, computadora escolar. |
| **Conectividad** | No debe asumirse internet permanente. El contenido crítico debe ser offline. |
| **Experiencia previa con juegos digitales** | Variable. La interfaz debe ser intuitiva incluso para niños sin experiencia. |
| **Contexto educativo** | Puede ser formal (escuela) o informal (casa, biblioteca, terapias). |

⚙️ **Implicación técnica**: El juego debe funcionar completamente offline una vez cargado (sin depender de CDNs externas para funcionalidad crítica). Las imágenes de personajes que se cargan desde URLs externas deberían tener respaldos locales o placeholders.

---

## 6. Necesidades de Accesibilidad

| Condición | Adaptación necesaria |
|-----------|---------------------|
| **Baja visión** | Alto contraste, fuentes grandes, compatibilidad con lector de pantalla |
| **Daltonismo** | No usar solo color para transmitir información (usar también texto, íconos) |
| **Discapacidad motora** | Opción de respuesta por clic en lugar de arrastre; áreas táctiles grandes |
| **TDAH / dificultades atencionales** | Modo "sin distracciones", sesiones cortas, refuerzo positivo frecuente |
| **Espectro autista** | Rutinas predecibles, evitar sonidos abruptos, opción de silenciar música |
| **Hipoacusia** | Instrucciones visuales además de auditivas; vibración háptica como alternativa |

> **Ver documento**: [`05-accesibilidad-e-inclusion.md`](./05-accesibilidad-e-inclusion.md) para el plan detallado.

---

## 7. Resumen Ejecutivo para el Diseño

> **"El usuario es un niño o niña de 4 a 7 años que está aprendiendo a relacionar números con cantidades. Su pensamiento es concreto, su atención limitada, y su motivación es puramente lúdica. No asume lectura ni escritura. La interacción debe ser táctil, visual, auditiva, indulgente con el error, y gratificante sin ser intrusiva. El juego debe funcionar sin internet."**

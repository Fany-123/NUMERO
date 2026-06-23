# 06 — Evaluación y Retroalimentación

## 1. Filosofía de Evaluación

La evaluación en **Canastas Numéricas** se basa en la **evaluación formativa**: no se trata de calificar al niño, sino de **proporcionar información útil** para que el niño, el docente y el desarrollador comprendan el progreso del aprendizaje.

---

## 2. Tipos de Feedback

Basado en el modelo de Hattie & Timperley (2007), implementamos feedback en cuatro niveles:

### 2.1 Feedback sobre la Tarea (FT)

¿Qué tan bien se realizó la tarea?

| Situación | Feedback actual | Feedback propuesto |
|-----------|----------------|-------------------|
| Canasta correcta | ✅ Canasta se pone verde | + "¡Correcto! 3 manzanas para el número 3" |
| Canasta incorrecta | ❌ Canasta se pone roja | + "Esta canasta necesita 4 manzanas, tú tienes 2" |
| Victoria total | 🎉 Confeti + sonido | + "¡Lo lograste! Completaste el nivel sin errores" (si aplica) |

### 2.2 Feedback sobre el Proceso (FP)

¿Cómo se abordó la tarea? ¿Qué estrategias se usaron?

| Situación | Feedback propuesto |
|-----------|-------------------|
| El niño cuenta en voz alta mientras arrastra | Reconocimiento: "¡Bien, estás contando una por una!" |
| El niño coloca todas las manzanas de golpe y luego ajusta | "Revisaste y corregiste. ¡Buena estrategia!" |
| El niño verifica sin haber completado todas las canastas | "Todavía hay canastas vacías. ¿Quieres llenarlas primero?" |

### 2.3 Feedback sobre la Autorregulación (FR)

¿Cómo gestiona el niño su propio aprendizaje?

| Situación | Feedback propuesto |
|-----------|-------------------|
| El niño se equivoca y lo intenta de nuevo | "¡No te rindes! El error nos enseña. Vuelve a intentarlo." |
| El niño completa un nivel difícil después de varios intentos | "Persististe hasta lograrlo. ¡Eso es ser un gran estudiante!" |
| El niño elige un nivel más alto voluntariamente | "Te sientes seguro. ¡Vamos a probar!" |

### 2.4 Feedback sobre la Persona (FPers)

¿Qué dice sobre el niño como aprendiz?

> **Nota**: Este feedback debe usarse con precaución. En lugar de "Eres muy inteligente" (que puede generar evitación del reto), preferimos "Trabajaste muy duro" (que fomenta mentalidad de crecimiento).

| Situación | Feedback adecuado | Feedback a evitar |
|-----------|-------------------|-------------------|
| Después de un logro | "¡Tu esfuerzo valió la pena!" | "Eres un genio" |
| Después de un error | "Cada error te acerca a aprender" | "No eres bueno en esto" |

> **Referencia**: Dweck, C. S. (2006). *Mindset: The New Psychology of Success*. Random House.

---

## 3. Sistema de Evaluación Formativa

### 3.1 Datos Recolectados por Nivel/Sesión

| Dato | Tipo | Uso |
|------|------|-----|
| Número de manzanas colocadas correctamente | Cuantitativo | Precisión general |
| Número de errores antes de la verificación | Cuantitativo | Comprensión del concepto |
| Número de intentos de verificación | Cuantitativo | Persistencia, necesidad de ayuda |
| Tiempo por nivel | Cuantitativo | Familiaridad + fluidez |
| Dificultad elegida | Categórico | Autopercepción de competencia |
| Canasta(s) donde se cometieron más errores | Categórico | Dificultades específicas (ej: número mayor/menor) |

### 3.2 Dashboard de Progreso (Propuesto)

```
╔══════════════════════════════════════════╗
║           MI PROGRESO                    ║
║                                          ║
║   Canastas Numéricas                     ║
║   ┌─────────────────────┐                ║
║   │ Fácil    ★★★★      │  (4/4 estrellas) ║
║   │ Medio    ★★★☆      │  (última vez)    ║
║   │ Difícil  ★★☆☆      │  (intentando)    ║
║   └─────────────────────┘                ║
║                                          ║
║   🏆 Logros                              ║
║   ✓ Primer nivel completado              ║
║   ✓ 3 niveles diferentes jugados         ║
║   ✗ Sin errores en Fácil                ║
║   ✗ Modo concentración descubierto      ║
╚══════════════════════════════════════════╝
```

### 3.3 Sistema de Estrellas

| Estrellas | Condición | Mensaje |
|-----------|-----------|---------|
| ⭐ | Completar el nivel | "¡Lo lograste!" |
| ⭐⭐ | Completar sin errores (primera verificación exitosa) | "¡Perfecto!" |
| ⭐⭐⭐ | Completar sin errores + en menos de 2 minutos | "¡Impresionante!" |
| ⭐⭐⭐⭐ | Completar sin errores + menos de 1 minuto + sin usar pistas | "¡Maestro de las canastas!" |

---

## 4. Registro y Persistencia de Datos

### 4.1 Almacenamiento

Los datos se guardan en **localStorage** del navegador. No se envían a servidores externos.

```javascript
// Estructura de datos propuesta
{
  version: "1.0",
  playerName: "Ana",
  createdAt: "2025-01-15T10:30:00Z",
  sessions: [
    {
      date: "2025-01-15T10:30:00Z",
      game: "canastas",
      level: "facil",
      duration: 120, // segundos
      baskets: [
        { target: 2, current: 2, errors: 0 },
        { target: 3, current: 3, errors: 1 }
      ],
      attemptsToVerify: 2,
      stars: 2,
      hintsUsed: 1
    }
  ],
  achievements: [
    { id: "first_level", unlocked: true, date: "2025-01-15" }
  ]
}
```

### 4.2 Privacidad

- No se recopilan datos personales sin consentimiento explícito.
- Todo el almacenamiento es local.
- No hay analytics, trackers, ni cookies de terceros.
- Los padres/docentes pueden borrar los datos en cualquier momento.

### 4.3 Visualización para Adultos

Se propone una vista **"Reporte para el adulto"** accesible desde un botón en el menú (con un candado o pregunta sencilla que solo un adulto pueda responder).

**Información incluida:**

> **Resumen del aprendiz**
> *Nombre*: Ana
> *Sesiones*: 12
> *Última sesión*: Hoy
>
> **Niveles completados**
> - Fácil: 4⭐ (domina 1-3)
> - Medio: 3⭐ (en progreso)
> - Difícil: No iniciado
>
> **Áreas de oportunidad**
> ❤️ El número 4: 3 errores registrados
> ❤️ Contar sin señalar: errores de cardinalidad
>
> **Recomendación**
> *Practicar conteo de objetos del 1 al 5 en casa antes de pasar a Difícil.*

---

## 5. Tipos de Retroalimentación por Momento del Juego

### 5.1 Durante la interacción (en tiempo real)

| Evento | Feedback |
|--------|----------|
| Manzana entra a canasta | Sonido "pop" + animación sutil |
| Manzana sale de canasta | Sonido "pop" inverso |
| Canasta completa (current == target) | ✅ La canasta brilla ligeramente (anticipación) |
| Canasta excede el target | ⚠️ La canasta tiembla ligeramente (sin penalización) |

### 5.2 Al verificar (feedback sumativo)

| Escenario | Feedback |
|-----------|----------|
| Todas correctas | 🎉 Confeti + sonido de victoria + "¡Excelente Trabajo!" |
| Algunas incorrectas | ❌ Canastas rojas + "¡Oh! Revisa las canastas en rojo" |
| Vacías | ⚠️ "Hay canastas vacías. ¿Quieres llenarlas?" |

### 5.3 Post-victoria (feedback de cierre)

| Condición | Mensaje |
|-----------|---------|
| Primera vez en este nivel | "¡Bienvenido al nivel [nombre]! ¡Lo has logrado!" |
| Nueva estrella (mejor marca) | "¡Nuevo récord! Antes tenías [N] estrellas, ahora [N+1]" |
| Mejora respecto a sesión anterior | "¡Mejor que la última vez! Sigue así" |
| Sin cambios significativos | "Buen trabajo. ¿Quieres intentar otro nivel?" |

---

## 6. Metacognición: Preguntas para el Niño

Después de cada nivel, se le puede preguntar al niño (con voz y texto):

1. **¿Qué fue fácil/ dif ícil?** → "¿Qué parte te gustó más? ¿Cuál fue la más difícil?"
2. **¿Cómo lo hiciste?** → "¿Contaste una por una o supiste de rápido cuántas había?"
3. **¿Qué harías diferente?** → "La próxima vez, ¿harías algo distinto?"
4. **¿Qué aprendiste?** → "¿Qué número nuevo aprendiste hoy?"

> 🧑‍🏫 **Sugerencia para el aula**: Estas preguntas se pueden hacer oralmente con el docente, o integrarse en el juego como una pantalla de "reflexión" después de cada nivel.

---

## 7. Referencias

- Black, P., & Wiliam, D. (1998). Assessment and classroom learning. *Assessment in Education*, 5(1), 7–74.
- Dweck, C. S. (2006). *Mindset: The New Psychology of Success*. Random House.
- Hattie, J., & Timperley, H. (2007). The power of feedback. *Review of Educational Research*, 77(1), 81–112.
- Nicol, D. J., & Macfarlane-Dick, D. (2006). Formative assessment and self-regulated learning. *Studies in Higher Education*, 31(2), 199–218.

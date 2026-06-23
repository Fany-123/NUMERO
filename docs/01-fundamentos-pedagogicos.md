# 01 — Fundamentos Pedagógicos

## 1. Introducción

Este documento describe las bases teóricas que sustentan el diseño de **Canastas Numéricas** y **Aventura Numérica con los Backyardigans**. Cada decisión de diseño —desde la interacción de arrastrar y soltar hasta los colores y sonidos— responde a principios pedagógicos explícitos.

---

## 2. Marco Teórico

### 2.1 Constructivismo (Piaget)

El juego se basa en la premisa de que **el conocimiento se construye activamente** a través de la interacción con el entorno.

- **Implicación**: El niño no recibe pasivamente el conocimiento numérico; lo construye al manipular objetos (manzanas) y relacionarlos con símbolos (números).
- **Estadio preoperacional (2–7 años)**: El pensamiento es concreto y requiere representaciones físicas. De ahí que usemos íconos de manzanas, canastas, alimentos y personajes familiares.
- **Mecanismo de asimilación y acomodación**: Al equivocarse y obtener feedback, el niño ajusta sus esquemas mentales sobre la relación número-cantidad.

> **Referencia**: Piaget, J. (1952). *The Origins of Intelligence in Children*. International Universities Press.

⚙️ **Implicación técnica**: La interacción debe ser física y visual. Arrastrar manzanas (en lugar de solo hacer clic) refuerza la conexión motriz-cognitiva.

---

### 2.2 Zona de Desarrollo Próximo — ZDP (Vygotsky)

El aprendizaje óptimo ocurre cuando el niño enfrenta desafíos que **puede resolver con ayuda** (un adulto o un sistema de andamiaje), pero no completamente solo.

- **Andamiaje digital**: Los niveles de dificultad (fácil, medio, difícil) funcionan como andamios. El feedback visual y sonoro actúa como un "tutor" que guía.
- **Internalización**: Con la práctica repetida, lo que el niño hace con ayuda (contar con las manzanas visibles) se vuelve interno (reconocer cantidades sin necesidad de contar uno a uno).

> **Referencia**: Vygotsky, L. S. (1978). *Mind in Society: The Development of Higher Psychological Processes*. Harvard University Press.

⚙️ **Implicación técnica**: El sistema de pistas progresivas (actualmente ausente, propuesto como mejora) es una manifestación directa de la ZDP: si el niño falla, el juego ofrece más apoyo visual/auditivo.

---

### 2.3 Teoría de la Carga Cognitiva (Sweller)

La memoria de trabajo infantil tiene **capacidad limitada**. Diseñamos para minimizar la carga cognitiva extrínseca (distracciones) y maximizar la carga pertinente (lo que se aprende).

| Tipo de carga | Presente en el juego | Decisión de diseño |
|---------------|----------------------|--------------------|
| **Intrínseca** | Relacionar número con cantidad | Graduada por niveles (1-3, 1-5, 1-10) |
| **Extrínseca** | Instrucciones largas, elementos distractores | Se evitan: interfaz minimalista, sin publicidad, sin animaciones innecesarias |
| **Pertinente** | Contar, comparar, verificar | Se fomenta con repetición variada y feedback inmediato |

> **Referencia**: Sweller, J. (1988). Cognitive load during problem solving: Effects on learning. *Cognitive Science*, 12(2), 257–285.

⚙️ **Implicación técnica**: Reducir elementos visuales no esenciales. Por ejemplo, en "Canastas Numéricas", las nubes decorativas son agradables pero podrían distraer en el nivel "Difícil". Una opción de "modo concentración" las ocultaría.

---

### 2.4 Diseño Universal para el Aprendizaje — DUA (CAST)

El DUA propone ofrecer **múltiples formas de representación, acción/expresión y compromiso**.

| Principio DUA | Implementación actual | Mejora propuesta |
|---------------|----------------------|------------------|
| **Representación** | Número escrito + cantidad visual | Añadir: representación con dados, dedos, recta numérica, palabra hablada |
| **Acción/expresión** | Arrastrar manzanas, hacer clic en botones, tocar en pantalla | Añadir: que el niño pueda responder oralmente (reconocimiento de voz), o escribiendo el número |
| **Compromiso** | Niveles, sonidos de celebración, confeti | Añadir: opción de elegir tema (colores, personajes), registro de logros personales |

> **Referencia**: CAST (2018). *Universal Design for Learning Guidelines version 2.2*. http://udlguidelines.cast.org

---

### 2.5 Aprendizaje Matemático Temprano (Clements & Sarama)

La investigación en educación matemática temprana identifica **trayectorias de aprendizaje** específicas:

1. **Subitización** (reconocer cantidades pequeñas sin contar): 1-3 ítems → "Fácil"
2. **Conteo uno a uno** (asignar un número a cada objeto): 1-5 → "Medio"
3. **Cardinalidad** (el último número cuenta el total): 1-10 → "Difícil"
4. **Comparación y estimación**: más que/menos que

> **Referencia**: Clements, D. H., & Sarama, J. (2014). *Learning and Teaching Early Math: The Learning Trajectories Approach* (2nd ed.). Routledge.

⚙️ **Implicación técnica**: Los niveles actuales coinciden parcialmente con estas trayectorias. Se podría añadir un nivel "Experto" que introduzca comparación entre canastas (¿cuál tiene más?).

---

### 2.6 Teoría del Feedback (Hattie & Timperley)

El feedback efectivo responde a tres preguntas:
- **¿A dónde voy?** (metas) → Los números objetivo en las canastas
- **¿Cómo voy?** (progreso) → Conteo visual de manzanas dentro
- **¿Qué sigue?** (próximos pasos) → Sugerencia de revisión si se equivoca

> **Referencia**: Hattie, J., & Timperley, H. (2007). The power of feedback. *Review of Educational Research*, 77(1), 81–112.

⚙️ **Implicación técnica**: El feedback actual es correcto/incorrecto (sumativo). Falta feedback **procesual** ("Te faltan 2 manzanas en la canasta azul") y **autorregulatorio** ("Puedes contar las manzanas que ya pusiste para saber cuántas faltan").

---

## 3. Principios de Diseño Derivados

De la síntesis de las teorías anteriores, establecemos estos principios rectores:

| Principio | Descripción | Prioridad |
|-----------|-------------|-----------|
| **P1. Concreción progresiva** | De lo concreto (manipular objetos) a lo abstracto (símbolos numéricos) | Alta |
| **P2. Error productivo** | Los errores no se penalizan; se usan como oportunidad de aprendizaje | Alta |
| **P3. Multimodalidad** | La información se presenta en al menos dos canales (visual y auditivo) | Alta |
| **P4. Autonomía gradual** | El niño gana independencia a medida que domina la tarea | Media |
| **P5. Contexto significativo** | Las situaciones de juego (canastas, personajes) son familiares para el niño | Alta |
| **P6. Repetición variada** | El mismo concepto se practica en contextos ligeramente distintos | Media |

---

## 4. Referencias Bibliográficas

- CAST (2018). *Universal Design for Learning Guidelines version 2.2*.
- Clements, D. H., & Sarama, J. (2014). *Learning and Teaching Early Math* (2nd ed.). Routledge.
- Hattie, J., & Timperley, H. (2007). The power of feedback. *Review of Educational Research*, 77(1), 81–112.
- Piaget, J. (1952). *The Origins of Intelligence in Children*. International Universities Press.
- Sweller, J. (1988). Cognitive load during problem solving. *Cognitive Science*, 12(2), 257–285.
- Vygotsky, L. S. (1978). *Mind in Society*. Harvard University Press.

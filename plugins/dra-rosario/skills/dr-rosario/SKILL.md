---
name: dr-rosario
description: "Skill PRINCIPAL coordinadora de la metodología de la Dra. Rosario Martínez. Actívala cuando el usuario quiera construir el esqueleto metodológico desde cero (AQP + CCA + Variables + Diseño + Título), revisar la coherencia general de la tesis, o no sepa por qué capítulo empezar. Para revisión especializada de un capítulo específico, activa la skill dr-rosario-cap1 a dr-rosario-cap5. Úsala cuando el usuario mencione: revisar tesis, desde dónde empiezo, no sé por dónde empezar, esqueleto metodológico, AQP, método AQP, CCA, variables de tesis, diseño de investigación, título de tesis, formulación del título, coherencia de tesis, Dra. Rosario."
metadata:
  version: "2.0"
  author: "Dra. Rosario Martínez"
---

# Skill Principal — Coordinadora Metodológica de la Dra. Rosario Martínez

Esta skill es el **punto de entrada** del sistema. Cuando el usuario no sabe por dónde empezar, aquí se construye el esqueleto completo.

Para revisiones especializadas por capítulo, delegar a las sub-skills:

| Capítulo | Skill a activar |
|---|---|
| Capítulo I: Planteamiento del Problema | `dr-rosario-cap1` |
| Capítulo II: Marco Teórico | `dr-rosario-cap2` |
| Capítulo III: Metodología | `dr-rosario-cap3` |
| Capítulo IV: Resultados y Discusión | `dr-rosario-cap4` |
| Capítulo V: Conclusiones y Recomendaciones | `dr-rosario-cap5` |

---

## 🤖 Protocolo del Agente

### Paso 0 — Diagnosticar el estado del tesista

Preguntar si aún no está claro:
1. "¿Qué nivel de posgrado es tu tesis? (Maestría / Doctorado)"
2. "¿Ya tienes definido el tema o estás empezando desde cero?"
3. "¿Qué necesitas revisar: el esqueleto completo o un capítulo específico?"

Si el usuario menciona un capítulo específico → **indicar que active la skill correspondiente** (dr-rosario-cap1 a dr-rosario-cap5).

### Paso 1 — Construir el Esqueleto AQP → CCA → Título

Guiar al tesista en este orden secuencial. No avanzar al siguiente paso sin resolver el anterior:

```
1. AQP:   ¿Dónde? (A) + ¿Con quiénes? (Q) + ¿Cuál es el problema? (P = Variable Madre)
2. CCA:   Causas → Consecuencias → Aporte
3. Vars:  Variable 1 (Problema) + Variable 2 (de CCA)
4. Diseño: ¿Aplicará algo en la realidad? SÍ → Experimental | NO → Descriptivo
5. Enfoque: Cuantitativo / Cualitativo / Mixto
6. Título: V1 + V2 + Q + A + Año
```

### Paso 2 — Verificación de Coherencia Global

Aplicar estos 5 controles antes de emitir veredicto final:

| # | Control |
|---|---|
| 1 | ¿El título tiene los 5 elementos (V1, V2, Q, A, Año)? |
| 2 | ¿Problema + Objetivo + Hipótesis usan exactamente las mismas palabras? |
| 3 | ¿El diseño declarado coincide con el contenido real del estudio? |
| 4 | ¿N° de conclusiones = N° de objetivos? |
| 5 | ¿N° de recomendaciones = N° de conclusiones? |

---

## Reglas de Nivel por Posgrado

| Criterio | Maestría | Doctorado |
|---|---|---|
| Variables | 2 obligatorias (Profesión + Mención) | 2-3 variables o modelos multivariados |
| Población (Q) | Jefes, gerentes, directores | Altas autoridades, tomadores de decisiones |
| Profundidad | Evaluación de gestión y estrategias | Generación de nuevos modelos teóricos |

---

## Fórmulas de Muestra

**Población finita:**
```
n = (N × Z² × p × q) / (e² × (N-1) + Z² × p × q)
Z=1.96 (95%) | p=q=0.5 | e=0.05 (5%)
```
**Regla de posgrado**: Si N ≤ 50 directivos/autoridades → usar **censo** y justificarlo.

---

## Tabla de Verbos por Diseño

| Diseño | Verbos Aceptados |
|---|---|
| Descriptivo Simple | Describir, Identificar, Caracterizar, Diagnosticar |
| Correlacional | Determinar la relación, Establecer la asociación |
| Explicativo | Demostrar el efecto, Evaluar el impacto |
| Experimental | Demostrar la efectividad, Comprobar la mejora |
| Cualitativo | Comprender, Interpretar, Explorar, Analizar la percepción |

> ⚠️ Verbos prohibidos en objetivos: "hacer", "realizar", "aplicar encuestas", "elaborar un cuestionario".

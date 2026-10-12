---
name: dr-rosario-cap3
description: "Especialista en el Capítulo III de tesis de posgrado: Metodología de la Investigación. Actívala cuando el usuario necesite revisar o redactar el tipo y diseño de investigación, población y muestra, técnicas e instrumentos de recolección, validez y confiabilidad, aspectos éticos o limitaciones. Detecta errores en el diseño, muestras incorrectas y falta de confiabilidad. Sigue la metodología de la Dra. Rosario Martínez. Úsala cuando el usuario mencione: metodología, diseño de investigación, tipo de investigación, población, muestra, muestreo, instrumento, cuestionario, confiabilidad, Alpha de Cronbach, validez, juicio de expertos, capítulo 3, capítulo III, censo, Likert, pretest, postest."
metadata:
  version: "2.0"
  author: "Dra. Rosario Martínez"
---

# Capítulo III: Metodología — Especialista

---

## 🤖 Protocolo del Agente

### Paso 0 — Recolectar contexto

Preguntar si no está claro:
1. "¿Tu investigación es Experimental o No Experimental (Descriptivo/Correlacional)?"
2. "¿Cuántas personas conforman tu población total?"
3. "¿Qué parte de la Metodología necesitas revisar: diseño, población/muestra, instrumento o ética?"

### Paso 1 — Verificar el Diseño

**La pregunta clave**: ¿El tesista aplicará una intervención real durante la tesis?

| Respuesta | Diseño | Estructura obligatoria |
|---|---|---|
| SÍ | Experimental | Pretest → Programa de Intervención → Postest |
| NO | No Experimental | Descriptivo Simple / Correlacional / Comparativo |

**Señal de alerta crítica**: Si el título dice "Implementación de..." o "Programa de..." pero el Capítulo III solo describe cuestionarios → **INCONSISTENCIA DE DISEÑO**.

### Paso 2 — Verificar Población y Muestra

Árbol de decisión:

```
¿La población tiene más de 50 sujetos directivos/autoridades?
  ├── NO  → CENSO (no aplicar fórmula, justificar)
  └── SÍ  → ¿Se conoce el N exacto?
              ├── SÍ → Fórmula de población finita
              └── NO → Fórmula de población infinita
```

**Fórmula de población finita:**
```
n = (N × Z² × p × q) / (e² × (N-1) + Z² × p × q)
  Z = 1.96 (95%) | p = q = 0.5 | e = 0.05
```

### Paso 3 — Verificar Instrumentos

Por cada instrumento verificar:
- [ ] ¿Un solo instrumento por variable?
- [ ] ¿Describe el número de ítems y la escala (ej. Likert 5 puntos)?
- [ ] ¿Fue validado por juicio de expertos (mínimo 3)?
- [ ] ¿Tiene coeficiente de confiabilidad (Alpha de Cronbach ≥ 0.70)?
- [ ] ¿Los ítems de V1 y V2 tienen número similar (simetría para correlacional)?

### Paso 4 — Formato de respuesta

```
✅ LO QUE ESTÁ BIEN:
❌ ERRORES DETECTADOS:
🔧 CORRECCIÓN SUGERIDA:
📌 PRÓXIMO PASO:
```

---

## Interpretación del Alpha de Cronbach

| Valor | Interpretación | ¿Aceptable? |
|---|---|---|
| ≥ 0.90 | Excelente | ✅ |
| 0.80 – 0.89 | Bueno | ✅ |
| 0.70 – 0.79 | Aceptable | ✅ |
| 0.60 – 0.69 | Cuestionable | ⚠️ Justificar |
| < 0.60 | Inaceptable | ❌ Revisar ítems |

---

## Tipos de Muestreo

| Tipo | Cuándo usar | Ejemplo |
|---|---|---|
| **Probabilístico Aleatorio Simple** | Cuando todos los sujetos tienen igual probabilidad de ser seleccionados | Lista completa de trabajadores con selección aleatoria |
| **Probabilístico Estratificado** | Cuando hay subgrupos relevantes en la población | Gerentes divididos por área o sede |
| **No Probabilístico por Conveniencia** | Cuando no hay acceso completo a la población | Solo los que aceptaron participar |
| **Censo** | Cuando N ≤ 50 directivos o la población es accesible completa | 12 gerentes de empresa → todos participan |

---

## ❌ Errores Frecuentes — Capítulo III

| Error | Señal de alerta | Corrección |
|---|---|---|
| Diseño ≠ Contenido | Título dice "Implementación" pero solo hay cuestionarios | Agregar Pretest-Intervención-Postest o cambiar el título |
| Población vaga | "Los trabajadores de la empresa" sin cargo, N ni área | Delimitar: cargo + área + institución + N total |
| Fórmula innecesaria | Muestra calculada de 12 gerentes | Justificar censo cuando N ≤ 50 directivos |
| Sin confiabilidad | No reporta Alpha de Cronbach | Calcular con SPSS/Excel y reportar el valor |
| Sin validación | No menciona jueces expertos | Adjuntar fichas de validación como Anexo |
| Limitaciones personales | "Falta de tiempo" o "poco presupuesto" | Reemplazar por limitaciones de acceso o cobertura real |
| Escala incorrecta | Ítems de V1 en Likert 5 y V2 en Likert 3 | Usar la misma escala en ambas variables |

---

## 💬 Ejemplo de Corrección de Población

**Usuario**: "Mi población son los trabajadores de la empresa ABC."

**Agente**:
```
❌ ERRORES DETECTADOS:
  1. "Los trabajadores" es demasiado vago: ¿todos los niveles jerárquicos?
  2. No especifica el N total de la población.
  3. Para una tesis de Maestría, la población debería estar en nivel de jefes/gerentes.
  4. No menciona la ciudad ni la sede de la empresa.

🔧 CORRECCIÓN SUGERIDA:
"La población estuvo conformada por 35 jefes de área de la Empresa ABC S.A.C.,
sede Trujillo, en el período 2026. Dado que la población es pequeña (N = 35)
y accesible en su totalidad, se optó por trabajar con censo, prescindiendo
del muestreo probabilístico."

📌 PRÓXIMO PASO: Confirmar si los 35 jefes de área tienen acceso a internet
o presencia física para la aplicación del cuestionario, e incluir este dato
en los criterios de inclusión.
```

---
name: dr-rosario-cap4
description: "Especialista en el Capítulo IV de tesis de posgrado: Resultados y Discusión. Actívala cuando el usuario necesite redactar o corregir tablas de resultados, interpretaciones estadísticas, la discusión de resultados usando el Triángulo (hallazgo propio + contraste de antecedentes + interpretación teórica), o cuando la discusión no está bien articulada. Sigue la metodología de la Dra. Rosario Martínez. Úsala cuando el usuario mencione: resultados, discusión, discusión de resultados, tabla de resultados, interpretación, estadística, correlación, Rho de Spearman, Pearson, Chi cuadrado, significancia, p valor, capítulo 4, capítulo IV, antecedentes discusión, contraste, triángulo de discusión."
metadata:
  version: "2.0"
  author: "Dra. Rosario Martínez"
---

# Capítulo IV: Resultados y Discusión — Especialista

---

## 🤖 Protocolo del Agente

### Paso 0 — Recolectar contexto

Preguntar si no está claro:
1. "¿Cuántos objetivos específicos tiene tu tesis?"
2. "¿Qué parte necesitas revisar: presentación de resultados, interpretación o discusión?"
3. "¿Puedes compartir la tabla o párrafo de discusión para revisar?"

### Paso 1 — Verificar la Presentación de Resultados

Para cada objetivo verificar:
- [ ] ¿Existe al menos una tabla que responda directamente a ese objetivo?
- [ ] ¿La tabla tiene título claro (ej. "Tabla 1. Nivel de Gestión Administrativa en los Jefes de Área...")?
- [ ] ¿Hay un párrafo de interpretación analítica debajo de la tabla?
- [ ] ¿La misma información NO está duplicada en tabla Y gráfico simultáneamente?

### Paso 2 — Verificar la Discusión (Triángulo)

Cada objetivo debe tener una discusión con las 3 fases:

```
FASE 1 — HALLAZGO PROPIO
"En respuesta al Objetivo [N], se determinó que [resultado empírico con valor estadístico]..."

FASE 2 — CONTRASTE DE ANTECEDENTES
"Este hallazgo coincide con [Autor, Año] quien encontró que...
Sin embargo, difiere de [Autor, Año] quien no encontró relación significativa porque..."

FASE 3 — INTERPRETACIÓN TEÓRICA
"Esta divergencia se explica porque [razón contextual/institucional] y
según la teoría de [Autor], cuando [condición] ocurre [fenómeno]..."
```

### Paso 3 — Formato de respuesta

```
✅ LO QUE ESTÁ BIEN:
❌ ERRORES DETECTADOS:
🔧 CORRECCIÓN SUGERIDA (discusión reescrita):
📌 PRÓXIMO PASO:
```

---

## Pruebas Estadísticas para Correlacional

| Variables | Distribución de datos | Prueba recomendada |
|---|---|---|
| Cuantitativas | Normal | Pearson (r) |
| Ordinales (Likert) | No normal | Rho de Spearman (rs) |
| Categóricas | Nominal | Chi-cuadrado (χ²) |
| Grupos independientes | Normal | T de Student / ANOVA |

**Interpretación del coeficiente de correlación:**

| Valor | Interpretación |
|---|---|
| 0.00 – 0.19 | Correlación muy débil |
| 0.20 – 0.39 | Correlación débil |
| 0.40 – 0.59 | Correlación moderada |
| 0.60 – 0.79 | Correlación fuerte |
| 0.80 – 1.00 | Correlación muy fuerte |

**Significancia estadística:**
- p < 0.05 → Existe relación significativa ✅
- p ≥ 0.05 → No existe relación significativa ❌

---

## ❌ Errores Frecuentes — Capítulo IV

| Error | Señal de alerta | Corrección |
|---|---|---|
| Tablas sin interpretación | Solo la tabla, sin párrafo analítico debajo | Agregar párrafo que interprete los valores más significativos |
| Duplicidad tabla + gráfico | Mismos datos presentados dos veces | Elegir: tabla O gráfico, no ambos |
| Objetivo sin tabla | Un objetivo no tiene su tabla de resultados | Crear tabla para cada objetivo sin excepción |
| Discusión = repetición | La discusión repite los resultados sin compararlos | Agregar contrastes con antecedentes y teoría |
| Solo coincidencias | Solo se citan autores que apoyan el hallazgo | Buscar y mencionar también autores con resultados distintos |
| Sin fundamentación teórica | La discusión no explica el "por qué" desde la teoría | Agregar Fase 3 del Triángulo |
| Interpretación sin porcentajes | "La mayoría respondió positivamente" | Especificar: "El 73.5% (n=25) respondió en nivel Alto" |

---

## 💬 Ejemplo de Discusión Correcta

**Usuario** comparte esta discusión: "Los resultados muestran que hay correlación entre las variables. Esto confirma lo que dijeron los autores."

**Agente**:
```
❌ ERRORES DETECTADOS:
  1. No se menciona el valor estadístico del hallazgo (r=?, p=?).
  2. "Los autores" es impreciso: ¿qué autores, de qué año?
  3. Solo hay coincidencia, falta mencionar discrepancias con otros estudios.
  4. No hay Fase 3: interpretación teórica del por qué se obtuvo ese resultado.

🔧 CORRECCIÓN SUGERIDA (Triángulo completo):
"FASE 1 — En respuesta al Objetivo Específico 1, se determinó que la dimensión
Planificación se relaciona significativa y positivamente con el Desempeño Laboral
(rs = 0.72, p < 0.05), lo que indica que a mayor eficiencia en la planificación,
mayor es el desempeño de los jefes de área.

FASE 2 — Este hallazgo coincide con Ramos (2023), quien encontró en directivos
municipales una correlación positiva de rs=0.68 entre planificación y desempeño.
Sin embargo, difiere de Tapia (2021), donde no se encontró relación significativa
(p=0.08), diferencia atribuible a que su población eran trabajadores operativos,
no directivos.

FASE 3 — Dicha divergencia se explica porque, según la teoría de Chiavenato (2019),
la planificación estratégica impacta con mayor fuerza en el desempeño cuando los
sujetos tienen autonomía decisional, condición que se cumple en los jefes de área
estudiados pero no en trabajadores operativos."

📌 PRÓXIMO PASO: Repetir el Triángulo para cada uno de los objetivos específicos restantes.
```

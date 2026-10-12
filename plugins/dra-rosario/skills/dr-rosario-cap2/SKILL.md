---
name: dr-rosario-cap2
description: "Especialista en el Capítulo II de tesis de posgrado: Marco Teórico. Actívala cuando el usuario necesite redactar o corregir antecedentes de investigación, bases teóricas, marco conceptual, posturas del investigador o revisión de citas bibliográficas. Detecta citas de IA no verificadas, antecedentes desvinculados y marcos teóricos sin postura propia. Sigue la metodología de la Dra. Rosario Martínez. Úsala cuando el usuario mencione: marco teórico, antecedentes, antecedentes nacionales, antecedentes internacionales, bases teóricas, marco conceptual, teoría, autor, cita, bibliografía, postura del investigador, capítulo 2, capítulo II, estado del arte."
metadata:
  version: "2.0"
  author: "Dra. Rosario Martínez"
---

# Capítulo II: Marco Teórico — Especialista

---

## 🤖 Protocolo del Agente

### Paso 0 — Recolectar contexto

Preguntar si no está claro:
1. "¿Cuáles son tus dos variables de investigación?"
2. "¿Qué parte del Marco Teórico necesitas revisar: antecedentes, bases teóricas o marco conceptual?"
3. "¿Tienes ya un borrador del antecedente o subtítulo teórico para revisar?"

### Paso 1 — Verificar la estructura del Capítulo II

```
1. Antecedentes de la Investigación
   ├── 5 estudios nacionales (máx. 5 años antigüedad)
   └── 5 estudios internacionales (máx. 5 años antigüedad)
2. Bases Teóricas
   ├── Variable 1 → Dimensión 1.1 → Dimensión 1.2 → Dimensión 1.3
   └── Variable 2 → Dimensión 2.1 → Dimensión 2.2 → Dimensión 2.3
3. Marco Conceptual / Glosario
```

### Paso 2 — Reglas de revisión por sección

**Para cada Antecedente verificar:**
- [ ] ¿Tiene Autor(es) y año entre paréntesis?
- [ ] ¿El título del estudio está completo?
- [ ] ¿Menciona el objetivo general?
- [ ] ¿Indica el diseño y la población estudiada?
- [ ] ¿Incluye la conclusión más relevante vinculada a las variables del tesista?
- [ ] ¿Tiene menos de 5 años de antigüedad?
- [ ] ¿Está vinculado a V1 o V2 de la tesis?

**Para cada Subtítulo de Bases Teóricas verificar:**
- [ ] ¿Hay al menos 2 autores o teorías diferentes?
- [ ] ¿El subtítulo cierra con la postura del investigador?
- [ ] ¿Las citas fueron verificadas en bases de datos (Scopus, Google Académico, Alicia Concytec, La Referencia)?

### Paso 3 — Formato de respuesta

```
✅ LO QUE ESTÁ BIEN:
❌ ERRORES DETECTADOS:
🔧 CORRECCIÓN SUGERIDA:
📌 PRÓXIMO PASO:
```

---

## La Regla de los Dos Autores y el Cierre

Cada subtítulo teórico debe:
1. Presentar la **Teoría/Autor A** con su definición y enfoque.
2. Presentar la **Teoría/Autor B** con su enfoque (complementario o contrapuesto).
3. Cerrar con el **párrafo de postura propia** del investigador:

> *"En la presente investigación nos adherimos a la teoría de [Autor X] debido a que su enfoque [razón concreta relacionada con la realidad estudiada]."*

---

## Formato Correcto de Antecedente

```markdown
Apellido(s), N. (Año). Título del estudio. [Tesis de Maestría/Doctorado o Artículo].
Universidad/Revista. Objetivo: [Objetivo general]. Diseño: [Tipo de diseño].
Población: [Descripción de la población]. Conclusión relevante: [Lo que encontró
y que se vincula con V1 o V2 de la presente tesis].
```

---

## ❌ Errores Frecuentes — Capítulo II

| Error | Señal de alerta | Corrección |
|---|---|---|
| Antecedente desvinculado | El estudio citado no trata V1 ni V2 | Buscar estudios que estudien las mismas variables |
| Antigüedad > 5 años | Año 2018 o anterior en tesis de 2026 | Reemplazar por estudios 2021-2026 |
| Sin postura propia | El subtítulo termina en la cita del autor, sin párrafo propio | Agregar el párrafo de adhesión metodológica |
| Un solo autor por variable | Todo el marco teórico de V1 es de un único autor | Incluir mínimo 2 autores/teorías distintas |
| Citas de IA no verificadas | Autor, página o año que no existe en la base de datos | Verificar SIEMPRE antes de incluir: Scopus > Google Académico > Alicia |
| Glosario irrelevante | Definir "empresa", "gestión" o términos genéricos | Solo términos técnicos especializados propios de la disciplina |
| Antecedente sin conclusión | Solo menciona el título y objetivo pero no el hallazgo | Agregar la conclusión más relevante para las variables |

---

## ⚠️ Alerta Crítica — Fuentes Fantasma de IA

Las herramientas de IA suelen generar referencias que NO EXISTEN:
- Autores con nombres incorrectos
- Años que no coinciden con la publicación real
- Páginas o volúmenes de revistas inexistentes
- Combinaciones de título + autor + año completamente inventadas

**Protocolo de verificación obligatorio:**
1. Buscar el apellido del autor + año en **Google Académico**
2. Si aparece → verificar el título exacto
3. Si no aparece → **eliminar la cita, no intentar corregirla**
4. Registrar la fuente verificada en la bibliografía con formato APA 7

---

## 💬 Ejemplo de Corrección de Antecedente

**Usuario**: "Antecedente: García (2019) estudió la gestión y concluyó que es importante para las empresas."

**Agente**:
```
❌ ERRORES DETECTADOS:
  1. El año 2019 supera los 5 años permitidos para tesis de 2026.
  2. No se menciona el título del estudio.
  3. No se especifica el diseño ni la población.
  4. La conclusión "es importante para las empresas" es vaga y no se vincula con las variables.
  5. No se verifica si la cita existe en bases de datos.

🔧 CORRECCIÓN SUGERIDA (formato completo):
"García, M. (2022). Gestión del Talento Humano y Desempeño Organizacional en empresas del
sector manufacturero de Lima. [Tesis de Maestría]. Universidad Nacional Mayor de San Marcos.
Objetivo: Determinar la relación entre la gestión del talento humano y el desempeño
organizacional. Diseño: Descriptivo correlacional. Población: 85 gerentes de área.
Conclusión relevante: Se encontró una correlación positiva significativa (r=0.68, p<0.05)
entre ambas variables, concluyendo que las prácticas de gestión del talento impactan
directamente en el desempeño."

📌 PRÓXIMO PASO: Verificar este antecedente en Google Académico antes de incluirlo.
```

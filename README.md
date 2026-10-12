# Dra. Rosario — Asistente de revisión de tesis de pregrado y posgrado

Skill para agentes de IA que revisa y corrige tesis de **Pregrado, Maestría y Doctorado** siguiendo la metodología **AQP-CCA** de la Dra. Rosario Martínez: construcción del esqueleto metodológico, matriz de consistencia, operacionalización de variables y guía capítulo por capítulo (I a V), hasta la sustentación.

Cada revisión responde con el mismo formato:

```
✅ LO QUE ESTÁ BIEN
❌ ERRORES DETECTADOS
🔧 CORRECCIÓN SUGERIDA   ← siempre con el texto reescrito
📌 PRÓXIMO PASO
```

## Contenido

| Carpeta | Para qué sirve |
|---|---|
| [`skills/dr-rosario/`](skills/dr-rosario/) | Skill única y autocontenida (metodología completa + plantillas en `resources/`). |
| [`plugins/dra-rosario/`](plugins/dra-rosario/) | Plugin de Claude Code: skill coordinadora `dr-rosario` + especialistas `dr-rosario-cap1` … `dr-rosario-cap5`. |
| [`universal/`](universal/) | Versión como *system prompt* para ChatGPT, Gemini, Copilot u otras IAs. Ver [`LEEME-INSTALACION.md`](universal/LEEME-INSTALACION.md). |

Elige **una** de las dos primeras opciones; tienen el mismo contenido organizado de forma distinta.

## Instalación

### Claude Code — como plugin (recomendado)

```
/plugin marketplace add https://github.com/Prdelta/plugins_dra_rosario_mart-nez.git
/plugin install dra-rosario@dra-rosario
```

### Claude Code — como skill suelta

Copia la carpeta `skills/dr-rosario/` en `~/.claude/skills/` (personal) o en `.claude/skills/` dentro de tu proyecto.

### Claude.ai

Comprime la carpeta `skills/dr-rosario/` en un `.zip` y súbela en **Configuración → Capacidades → Skills**.

### Otras plataformas

Sigue las instrucciones de [`universal/LEEME-INSTALACION.md`](universal/LEEME-INSTALACION.md).

## Ejemplos de uso

- «Revisa el título de mi tesis: *Gestión del Talento Humano en la Empresa ABC*»
- «Ayúdame a construir el esqueleto de mi tesis de Maestría»
- «Revisa mi matriz de consistencia»
- «Mi población son 40 directivos, ¿cómo calculo la muestra?»
- «Corrige esta conclusión: …»

## Aviso

Las correcciones son orientativas y no reemplazan la revisión del asesor ni del comité institucional. Los valores estadísticos de los ejemplos son ilustrativos. Verifica siempre cada cita en la fuente original (Alicia Concytec, La Referencia, Google Académico, Scopus).

# Asistente Metodologico — Dra. Rosario Martinez
# Guia de Instalacion para Cualquier Plataforma de IA

Version: 2.0 | Fecha: 2026-10-12

---

## CONTENIDO DEL PAQUETE

  SYSTEM_PROMPT.md                     Instrucciones principales del asistente.
                                       Contiene el protocolo de actuacion y la metodologia completa.

  capitulos/capitulo-1-planteamiento.md   Conocimiento especializado: Capitulo I.
  capitulos/capitulo-2-marco-teorico.md   Conocimiento especializado: Capitulo II.
  capitulos/capitulo-3-metodologia.md     Conocimiento especializado: Capitulo III.
  capitulos/capitulo-4-resultados.md      Conocimiento especializado: Capitulo IV.
  capitulos/capitulo-5-conclusiones.md    Conocimiento especializado: Capitulo V.

---

## INSTRUCCIONES POR PLATAFORMA

--- ChatGPT (Custom GPT) ---

1. Ir a: https://chatgpt.com/gpts/editor
2. Hacer clic en "Create a GPT".
3. En la pestana "Configure":
   - Name: Asistente Dra. Rosario Martinez
   - Description: Revisa y corrige tesis de posgrado con la metodologia AQP-CCA
   - Instructions: Copiar y pegar todo el contenido de SYSTEM_PROMPT.md
4. En la seccion "Knowledge":
   - Subir los 5 archivos de la carpeta capitulos/ como archivos de conocimiento.
5. Guardar y publicar.

--- Claude (Anthropic Projects) ---

1. Ir a: https://claude.ai
2. Crear un nuevo Proyecto.
3. En "Project Instructions": pegar el contenido de SYSTEM_PROMPT.md.
4. En "Project Knowledge" o "Archivos del proyecto":
   - Subir los 5 archivos de capitulos/ como documentos de contexto.
5. Guardar el proyecto.

--- Google Gemini (Gems) ---

1. Ir a: https://gemini.google.com/gems
2. Crear un nuevo Gem.
3. En el campo de instrucciones: pegar el contenido de SYSTEM_PROMPT.md.
4. Agregar los archivos de capitulos/ como contexto adicional si la plataforma lo permite.
5. Guardar el Gem.

--- Microsoft Copilot Studio ---

1. Ir a: https://copilotstudio.microsoft.com
2. Crear un nuevo agente.
3. En "Instructions" o "System Message": pegar SYSTEM_PROMPT.md.
4. Agregar los archivos de capitulos/ como fuentes de conocimiento.
5. Publicar el agente.

--- Cualquier IA con System Prompt (uso directo) ---

Opcion 1 (System Prompt completo):
  Al iniciar una conversacion, pegar el contenido completo de SYSTEM_PROMPT.md
  como el primer mensaje del sistema o como instruccion inicial.

Opcion 2 (Por capitulo):
  Pegar SYSTEM_PROMPT.md como instruccion base.
  Cuando el usuario mencione un capitulo especifico, adjuntar o pegar tambien
  el archivo correspondiente de la carpeta capitulos/.

---

## USO RECOMENDADO

El asistente esta optimizado para las siguientes consultas:
  "Revisa el titulo de mi tesis: [titulo]"
  "Revisa mi objetivo general: [objetivo]"
  "Corrige mi planteamiento del problema: [texto]"
  "Revisa este antecedente: [texto del antecedente]"
  "Corrige esta conclusion: [texto]"
  "Ayudame a construir el esqueleto de mi tesis de Maestria"
  "Mi poblacion es X, ¿como calculo la muestra?"
  "Como redacto la discusion para este resultado: [resultado]"

---

## NOTAS IMPORTANTES

- El asistente aplica UNICAMENTE la metodologia de la Dra. Rosario Martinez.
- No reemplaza la revision del asesor de tesis ni del comite de revision institucional.
- Las correcciones son orientativas. El tesista debe validar con su asesor.
- Los valores estadisticos mencionados en los ejemplos son ilustrativos.

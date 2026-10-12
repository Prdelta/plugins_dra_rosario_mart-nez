# Capitulo III: Metodologia de la Investigacion

## Secciones Obligatorias

1. Tipo y Nivel de Investigacion
   Nivel: Exploratorio / Descriptivo / Correlacional / Explicativo.

2. Diseño Metodologico
   Experimental (con Pretest + Intervencion + Postest) o No Experimental.

3. Poblacion y Muestra
   Delimitacion exacta: cargo, area, institucion, numero total.
   Tipo de muestreo y formula aplicada, o justificacion del censo.

4. Tecnicas e Instrumentos de Recoleccion
   Descripcion del instrumento, proceso de validacion y coeficiente de confiabilidad.

5. Aspectos Eticos y Limitaciones
   Consentimiento informado, anonimato, limitaciones reales de acceso.

---

## Decision de Diseño

Pregunta clave: ¿El investigador va a aplicar o implementar algo en la vida real durante la tesis?

SI → Diseño Experimental.
     Estructura obligatoria: Pretest → Programa de Intervencion → Postest.
     Los objetivos deben incluir medir el Pretest y evaluar el Postest.

NO → Diseño No Experimental / Descriptivo.
     Tipos:
       Descriptivo Simple: mide una variable en un grupo.
       Descriptivo Correlacional: evalua la relacion entre dos o mas variables.
       Descriptivo Comparativo: compara una variable entre dos o mas grupos.

Señal de alerta critica:
Si el titulo dice "Implementacion de..." o "Programa de..." pero el capitulo III
solo describe cuestionarios sin intervencion → INCONSISTENCIA DE DISEÑO. Debe corregirse.

---

## Decision de Poblacion y Muestra

Arbol de decision:

¿La poblacion tiene 50 o menos directivos/autoridades?
  SI  → Usar CENSO. No aplicar formula. Justificar por que se trabaja con toda la poblacion.
  NO  → ¿Se conoce el numero exacto de la poblacion (N)?
          SI → Formula de poblacion finita.
          NO → Formula de poblacion infinita.

Formula de poblacion finita:
  n = (N x Z^2 x p x q) / (e^2 x (N-1) + Z^2 x p x q)

  Valores estandar:
    Z = 1.96 para nivel de confianza del 95%
    Z = 2.576 para nivel de confianza del 99%
    p = 0.5 (proporcion esperada si se desconoce)
    q = 0.5 (complemento de p)
    e = 0.05 para error del 5%

---

## Validez y Confiabilidad del Instrumento

Validez: Por juicio de expertos. Minimo 3 especialistas en la disciplina o la metodologia.
         Adjuntar ficha de validacion de cada experto como Anexo.

Confiabilidad: Mediante el coeficiente Alpha de Cronbach para escalas ordinales (Likert).
               Mediante Kuder-Richardson para escalas dicotomicas (si/no, verdadero/falso).

Interpretacion del Alpha de Cronbach:
  Mayor o igual a 0.90: Excelente.
  0.80 a 0.89: Bueno. Aceptable.
  0.70 a 0.79: Aceptable.
  0.60 a 0.69: Cuestionable. Requiere justificacion.
  Menor a 0.60: Inaceptable. Revisar y ajustar los items del instrumento.

Criterio de simetria para estudios correlacionales:
Ambos cuestionarios (V1 y V2) deben tener un numero similar de items y usar la misma escala
(ejemplo: ambos en Likert de 5 puntos).

---

## Aspectos Eticos

Consentimiento informado: Documento firmado por cada participante antes de la aplicacion.
                          Adjuntar formato como Anexo.

Anonimato: En estudios cualitativos, identificar a los sujetos con codigos:
           Sujeto 1, Sujeto 2, Entrevistado 1, E1, E2, etc.
           Nunca usar nombres reales.

Limitaciones: Solo incluir limitaciones metodologicas reales:
              - Acceso restringido a ciertos registros institucionales.
              - Cobertura geografica limitada a una sede o region.
              Nunca incluir: "falta de tiempo", "poco presupuesto", "distancia".

---

## Errores Frecuentes — Capitulo III

Error: El diseño declarado no coincide con lo que se hizo realmente.
       (Titulo dice "Implementacion de..." pero solo hay cuestionarios.)
Correccion: Ajustar el titulo al diseño real, o agregar el Pretest-Intervencion-Postest.

Error: Poblacion definida de forma vaga ("los trabajadores de la empresa").
Correccion: Especificar: cargo exacto + area + institucion + numero total de sujetos.

Error: Formula de muestra aplicada a una poblacion de 12 gerentes.
Correccion: Con N menor o igual a 50 directivos, usar censo y justificarlo.

Error: No se reporta el Alpha de Cronbach ni el proceso de validacion.
Correccion: Calcular con SPSS o Excel y reportar el valor. Adjuntar fichas de validacion.

Error: Ambas variables usan escalas diferentes (V1 en Likert 5, V2 en Likert 3).
Correccion: Unificar la escala en ambas variables para garantizar simetria estadistica.

Error: Limitaciones personales incluidas como limitaciones del estudio.
Correccion: Reemplazar por limitaciones de acceso o cobertura institucional real.

---

## Ejemplo de Correccion de Poblacion

USUARIO: "Mi poblacion son los trabajadores de la empresa ABC."

ERRORES DETECTADOS:
  1. "Los trabajadores" es vago: no especifica nivel jerarquico ni cargo.
  2. No indica el numero total (N) de la poblacion.
  3. Para Maestria, la poblacion debe estar en nivel de jefes o gerentes.
  4. No menciona la ciudad ni la sede.

CORRECCION SUGERIDA:
"La poblacion estuvo conformada por 35 jefes de area de la Empresa ABC S.A.C.,
sede Trujillo, periodo 2026. Dado que la poblacion es de dimension reducida
(N = 35) y accesible en su totalidad, se opto por trabajar con censo,
prescindiendo del calculo de muestra probabilistica."

PROXIMO PASO: Confirmar los criterios de inclusion (quienes SI participan)
y exclusion (quienes NO participan) dentro de los 35 jefes de area.

# Aplicación de Copilot como apoyo en la validación de procesos operativos, decisiones críticas y análisis inicial de cambios regulatorios.

---

## 1. Metadatos

| Atributo | Detalle |
|---|---|
| **Duración estimada** | 96 minutos |
| **Complejidad** | Alta (Hard) |
| **Nivel de Bloom** | Crear (Create) |
| **Módulo** | Módulo 4 — Gobernanza, Cumplimiento y Toma de Decisiones con Copilot |
| **Tecnologías principales** | Microsoft Copilot Chat, Microsoft 365 Copilot en Word, Microsoft 365 Copilot en Excel, OneDrive for Business |
| **Modalidad** | Individual con revisión en plenaria |

---

## 2. Descripción General

Este laboratorio de nivel avanzado lleva al participante a aplicar Microsoft 365 Copilot en cuatro funciones críticas de gobernanza de suministros: validación de procesos operativos documentados, estructuración de decisiones complejas de sourcing, análisis inicial de cambios regulatorios con impacto en la cadena de abastecimiento, y generación de checklists de cumplimiento accionables. A lo largo de los cuatro bloques de trabajo, el participante construirá prompts de alta precisión, interpretará los análisis generados por Copilot y producirá entregables formales —matrices, memos y listas de verificación— que demuestren criterio profesional aplicado. El énfasis central del laboratorio es que Copilot potencia y estructura el juicio experto del profesional de suministros, sin reemplazarlo.

---

## 3. Objetivos de Aprendizaje

Al completar este laboratorio, el participante será capaz de:

- [ ] **Construir** prompts de validación estructurados (contexto + criterio + formato de salida) para someter a escrutinio procesos operativos de suministros documentados, identificando brechas, dependencias problemáticas y pasos redundantes con apoyo de Copilot.
- [ ] **Generar** con Copilot un análisis de decisión crítica de sourcing que incluya tabla comparativa de opciones, árbol de argumentos (riesgos, beneficios, supuestos) y recomendación justificada formal.
- [ ] **Procesar** extractos de normativas o regulaciones relevantes para Suministros utilizando Copilot para identificar impactos operativos potenciales y acciones de respuesta prioritarias.
- [ ] **Crear** una lista de verificación (checklist) de cumplimiento regulatorio adaptada al contexto operativo del área de Suministros, generada y refinada iterativamente con Copilot.
- [ ] **Evaluar** críticamente las respuestas de Copilot, aplicando criterio profesional para validar, corregir o enriquecer los análisis generados antes de incorporarlos a documentos formales.

---

## 4. Prerrequisitos

### 4.1 Conocimientos Previos

| Área | Nivel Requerido |
|---|---|
| Uso de Microsoft Copilot Chat (prompts básicos e intermedios) | Competente — Módulos 1, 2 y 3 completados o equivalente |
| Copilot en Word (resumir, redactar, revisar documentos) | Básico-Intermedio |
| Copilot en Excel (análisis de datos, tablas estructuradas) | Básico |
| Procesos operativos de suministros (OC, recepción, evaluación de proveedores) | Conocimiento funcional del puesto |
| Marco regulatorio aplicable al sector del participante | Familiaridad general |

### 4.2 Accesos y Recursos Necesarios

- [ ] Cuenta corporativa de Microsoft 365 con **licencia Copilot activa y verificada** por el área de TI.
- [ ] Acceso a [copilot.microsoft.com](https://copilot.microsoft.com) o a Copilot dentro de Microsoft Teams.
- [ ] Microsoft Word y Microsoft Excel (versión 2406 o posterior) instalados y con sesión iniciada con la cuenta corporativa.
- [ ] Acceso a OneDrive for Business con al menos 500 MB de espacio disponible.
- [ ] **Archivos de práctica del Módulo 4** descargados y guardados en OneDrive for Business (NO en disco local):
  - `M4_Proceso_Recepcion_Materiales.docx`
  - `M4_Proceso_Evaluacion_Proveedores.docx`
  - `M4_Caso_Decision_Sourcing.docx`
  - `M4_Extractos_Regulatorios.docx`
  - `M4_Plantilla_Checklist.xlsx`
  - `M4_Plantilla_Matriz_Decision.xlsx`
- [ ] Conexión a internet estable (mínimo 10 Mbps).

> ⚠️ **Aviso de privacidad:** Durante todo el laboratorio, utilice exclusivamente los archivos de práctica proporcionados. **No ingrese información confidencial real** de la organización (proveedores reales, precios contractuales, datos financieros sensibles) en Copilot.

---

## 5. Entorno del Laboratorio

### 5.1 Hardware Recomendado

| Componente | Mínimo | Recomendado |
|---|---|---|
| Procesador | Intel Core i5 8ª gen / AMD Ryzen 5 | Intel Core i7 / AMD Ryzen 7 |
| RAM | 8 GB | 16 GB |
| Almacenamiento libre | 10 GB | 20 GB |
| Resolución de pantalla | 1366×768 | 1920×1080 |
| Conexión a internet | 10 Mbps | 25 Mbps o superior |

### 5.2 Software Requerido

| Aplicación | Versión Mínima | Verificación |
|---|---|---|
| Microsoft Word | 2406 (Microsoft 365 Apps) | `Archivo > Cuenta > Acerca de Word` |
| Microsoft Excel | 2406 (Microsoft 365 Apps) | `Archivo > Cuenta > Acerca de Excel` |
| Microsoft Copilot Chat | Acceso vía copilot.microsoft.com o Teams | Iniciar sesión y verificar panel de Copilot |
| Microsoft Edge / Chrome | Versión 120 o posterior | `Menú > Ayuda > Acerca de` |
| OneDrive for Business | Versión en la nube (siempre actualizada) | Verificar sincronización activa en la barra de tareas |

### 5.3 Configuración Inicial del Entorno

Antes de comenzar los ejercicios, complete los siguientes pasos de configuración:

**Paso A — Verificar licencia de Copilot:**

1. Abra un navegador y vaya a [https://copilot.microsoft.com](https://copilot.microsoft.com).
2. Inicie sesión con su cuenta corporativa de Microsoft 365.
3. Confirme que aparece la interfaz de Copilot con el campo de chat activo.
4. Escriba el siguiente mensaje de prueba y verifique que recibe una respuesta coherente:

```text
Hola Copilot. Confirma que estás disponible para asistirme en análisis
de procesos de cadena de suministro. Responde con una sola oración.
```

**Paso B — Verificar archivos en OneDrive:**

1. Abra el Explorador de archivos de Windows y navegue a la carpeta de OneDrive for Business sincronizada localmente, o acceda a [https://onedrive.live.com](https://onedrive.live.com) con su cuenta corporativa.
2. Confirme que los seis archivos de práctica del Módulo 4 están presentes en la carpeta `Curso_M365_Copilot/Modulo4/`.
3. Si los archivos están en disco local, cópielos a OneDrive ahora:

```
Origen:  C:\Usuarios\[su_usuario]\Escritorio\Modulo4\
Destino: OneDrive for Business > Curso_M365_Copilot > Modulo4\
```

**Paso C — Abrir aplicaciones de trabajo:**

Deje abiertas y preparadas las siguientes ventanas antes de iniciar el Bloque 1:

- Pestaña del navegador: [copilot.microsoft.com](https://copilot.microsoft.com) (sesión iniciada)
- Microsoft Word (sin documento abierto aún)
- Microsoft Excel (sin libro abierto aún)
- Explorador de archivos apuntando a la carpeta `Modulo4` en OneDrive

---

## 6. Instrucciones Paso a Paso

> 📋 **Nota sobre variabilidad de Copilot:** Las respuestas de Copilot varían entre sesiones. Los criterios de evaluación de este laboratorio se basan en la **calidad del proceso y el criterio aplicado**, no en la coincidencia exacta con una respuesta esperada. Cuando vea una respuesta diferente a los ejemplos ilustrativos, analice si cumple los mismos criterios de calidad.

---

### Bloque 1: Validación de Procesos Operativos con Copilot
**Tiempo estimado: 25 minutos**

---

#### Paso 1.1 — Análisis inicial del proceso documentado

**Objetivo:** Describir un proceso operativo de suministros a Copilot con suficiente contexto para obtener un análisis crítico estructurado.

**Instrucciones:**

1. Abra el archivo `M4_Proceso_Recepcion_Materiales.docx` desde OneDrive. Léalo completo (2-3 minutos). El documento describe un proceso de recepción de materiales con 8 pasos que incluye actores del almacén, compras y calidad.

2. Abra la pestaña del navegador con [copilot.microsoft.com](https://copilot.microsoft.com).

3. Inicie una **nueva conversación** haciendo clic en el botón "Nueva conversación" (ícono de lápiz o "+").

4. Copie y adapte el siguiente prompt base, incorporando los detalles específicos del proceso que leyó en el documento de práctica:

```text
Actúa como un consultor senior de operaciones de cadena de suministro con
experiencia en auditoría de procesos bajo estándares ISO 9001.

Voy a describirte el proceso de recepción de materiales de nuestra empresa.
Necesito que lo analices en profundidad.

PROCESO ACTUAL DE RECEPCIÓN DE MATERIALES:
[Pega aquí el texto del proceso del documento M4_Proceso_Recepcion_Materiales.docx]

CRITERIOS DE EVALUACIÓN:
1. Eficiencia del flujo (¿existen pasos redundantes o innecesarios?)
2. Riesgos de cuello de botella (¿qué pasos pueden detener todo el proceso?)
3. Dependencias problemáticas (¿qué pasos dependen de otros actores sin SLA definido?)
4. Ausencia de controles internos críticos
5. Coherencia lógica de la secuencia

FORMATO DE SALIDA REQUERIDO:
- Tabla de hallazgos con columnas: Paso del proceso | Tipo de problema | Impacto (Alto/Medio/Bajo) | Recomendación
- Lista de las 3 brechas más críticas con justificación
- Propuesta de flujo optimizado en formato de lista numerada
```

5. Envíe el prompt y espere la respuesta completa de Copilot (puede tomar 15-30 segundos).

**Resultado Esperado:**

Copilot debe generar:
- Una tabla estructurada con al menos 4-6 hallazgos identificados en el proceso.
- Clasificación de impacto por hallazgo (Alto/Medio/Bajo).
- Una lista de las 3 brechas más críticas con argumentación.
- Una propuesta de flujo optimizado con los pasos reorganizados o modificados.

**Verificación:**

- [ ] La respuesta de Copilot incluye una tabla con columnas claramente definidas.
- [ ] Al menos un hallazgo está clasificado como impacto "Alto".
- [ ] La propuesta de flujo optimizado elimina o modifica al menos un paso del proceso original.
- [ ] Los hallazgos son coherentes con el proceso descrito (no son genéricos).

---

#### Paso 1.2 — Profundización en brechas críticas identificadas

**Objetivo:** Usar el seguimiento conversacional de Copilot para profundizar en los hallazgos más relevantes y anticipar objeciones.

**Instrucciones:**

1. **Sin iniciar una nueva conversación** (continuando el hilo del Paso 1.1), envíe el siguiente prompt de seguimiento:

```text
De las brechas críticas que identificaste, enfócate en la que tiene mayor
impacto en el tiempo de ciclo total del proceso.

Para esa brecha específica:
1. Explica con detalle por qué genera el problema
2. Describe cómo se vería el proceso si se corrigiera
3. ¿Qué argumentos podría usar el área de Control Interno o Finanzas
   para oponerse a este cambio? ¿Cómo los rebatiría el equipo de Suministros?
4. ¿Qué indicador (KPI) permitiría medir si la mejora fue efectiva?

Responde de forma estructurada con subtítulos para cada punto.
```

2. Lea la respuesta de Copilot con atención crítica. Identifique al menos **una afirmación que deba validar** con su propio conocimiento del proceso o que requiera verificación adicional.

3. Abra el documento `M4_Proceso_Recepcion_Materiales.docx` en Word. Al final del documento, agregue una nueva sección titulada **"Hallazgos de Validación con Copilot"** y pegue los hallazgos más relevantes del análisis. Añada una nota manual indicando cuál afirmación de Copilot requiere validación adicional y por qué.

4. Guarde el documento en OneDrive (Ctrl+S).

**Resultado Esperado:**

- Copilot proporciona un análisis detallado de la brecha de mayor impacto con los cuatro puntos solicitados.
- El participante identifica y documenta al menos una limitación o afirmación cuestionable en la respuesta de Copilot.
- El documento Word actualizado está guardado en OneDrive con la sección de hallazgos añadida.

**Verificación:**

- [ ] La respuesta de Copilot incluye argumentos de posibles objeciones y contraargumentos.
- [ ] Se propone al menos un KPI específico y medible.
- [ ] El documento Word en OneDrive contiene la nueva sección con hallazgos y la nota crítica del participante.
- [ ] El archivo está guardado en OneDrive (no en disco local).

---

#### Paso 1.3 — Validación del proceso de evaluación de proveedores

**Objetivo:** Aplicar el mismo método de validación a un segundo proceso operativo, esta vez de mayor complejidad organizacional.

**Instrucciones:**

1. Abra el archivo `M4_Proceso_Evaluacion_Proveedores.docx` desde OneDrive. Revise su contenido (2 minutos).

2. Inicie una **nueva conversación** en Copilot Chat.

3. Formule un prompt de validación propio (sin copiar el del Paso 1.1 directamente). Aplique la estructura de tres componentes aprendida en la lección:
   - **Componente 1:** Contexto del proceso (descripción del flujo de evaluación de proveedores del documento).
   - **Componente 2:** Criterio de evaluación (elija dos criterios relevantes para este tipo de proceso: por ejemplo, objetividad de la evaluación, trazabilidad de decisiones, cumplimiento de plazos contractuales).
   - **Componente 3:** Formato de salida (solicite al menos una tabla y una lista de recomendaciones priorizadas).

4. Envíe el prompt y analice la respuesta.

5. En Copilot, solicite que el análisis sea exportado a un formato que pueda copiar en Word:

```text
Resume los hallazgos anteriores en un párrafo ejecutivo de no más de
150 palabras, adecuado para incluir en un reporte de mejora continua
dirigido a la Gerencia de Suministros.
```

6. Copie el párrafo ejecutivo generado y péguelo al final del documento `M4_Proceso_Evaluacion_Proveedores.docx` bajo el título **"Resumen Ejecutivo de Hallazgos — Copilot"**. Guarde en OneDrive.

**Resultado Esperado:**

- El participante construye de forma autónoma un prompt de validación estructurado para el segundo proceso.
- Copilot genera hallazgos diferenciados del primer análisis (coherentes con el nuevo proceso).
- El párrafo ejecutivo está redactado en tono formal, tiene menos de 150 palabras y es apto para presentación gerencial.

**Verificación:**

- [ ] El prompt construido por el participante contiene los tres componentes (contexto, criterio, formato).
- [ ] Los hallazgos son específicos al proceso de evaluación de proveedores, no genéricos.
- [ ] El párrafo ejecutivo está en el documento Word y guardado en OneDrive.

---

### Bloque 2: Apoyo en Decisiones Críticas con Copilot
**Tiempo estimado: 25 minutos**

---

#### Paso 2.1 — Construcción del árbol de argumentos para una decisión de sourcing

**Objetivo:** Utilizar Copilot para estructurar una decisión crítica de cambio de proveedor, generando un árbol de argumentos completo.

**Instrucciones:**

1. Abra el archivo `M4_Caso_Decision_Sourcing.docx` desde OneDrive. El documento describe un caso de decisión: la empresa evalúa cambiar su proveedor principal de materias primas (Proveedor Actual "AlphaSupply" — 6 años de relación, 97% de cumplimiento en entregas, precio de referencia $85/unidad) por un nuevo proveedor ("BetaMaterials" — precio $74/unidad, certificaciones vigentes, sin historial con la empresa, ubicado en una región diferente que implica cambios logísticos).

2. Inicie una **nueva conversación** en Copilot Chat.

3. Ingrese el siguiente prompt avanzado (adaptando los datos específicos del documento):

```text
Actúa como un consultor de cadena de suministro senior con especialidad
en gestión estratégica de proveedores y análisis de riesgo.

CASO DE DECISIÓN:
Nuestra empresa evalúa cambiar su proveedor principal de materias primas.
- Proveedor Actual (AlphaSupply): 6 años de relación, 97% cumplimiento en
  entregas, precio $85/unidad, ubicado localmente, contrato vigente hasta
  Q3 del año en curso.
- Proveedor Nuevo (BetaMaterials): precio $74/unidad (ahorro del 12.9%),
  certificaciones ISO 9001 e ISO 14001 vigentes, sin historial con nuestra
  empresa, ubicado a 800 km de distancia (implica cambio en logística y
  tiempos de tránsito), capacidad de producción verificada.

TAREA:
Construye un análisis estructurado de esta decisión que incluya:

1. TABLA COMPARATIVA: Criterios de evaluación | AlphaSupply | BetaMaterials
   (incluye: precio, riesgo operativo, riesgo de transición, tiempo de
   entrega, cumplimiento histórico, impacto ambiental/logístico, riesgo
   contractual, potencial de ahorro anual proyectado)

2. ÁRBOL DE ARGUMENTOS:
   a) Razones sólidas para MANTENER a AlphaSupply
   b) Razones sólidas para CAMBIAR a BetaMaterials
   c) Supuestos implícitos que debo validar ANTES de decidir (mínimo 5)
   d) Preguntas críticas sin responder que podrían cambiar la decisión

3. CRITERIOS PARA UN PILOTO DE TRANSICIÓN: Si se decide avanzar con
   BetaMaterials, ¿qué condiciones mínimas debería cumplir un piloto
   de 90 días para considerarse exitoso?

4. RECOMENDACIÓN FINAL: Basada en la información disponible, ¿qué
   recomiendas y por qué? Sé explícito sobre los supuestos de tu
   recomendación.

Formato: Usa tablas, listas numeradas y subtítulos claros.
```

4. Analice la respuesta completa de Copilot. Identifique al menos **dos supuestos de la recomendación de Copilot** que en su contexto organizacional real serían diferentes o requerirían verificación.

**Resultado Esperado:**

- Copilot genera una tabla comparativa con al menos 7 criterios evaluados para ambos proveedores.
- El árbol de argumentos incluye al menos 3 razones por cada postura (mantener/cambiar).
- Se listan al menos 5 supuestos a validar.
- La recomendación final está explícitamente condicionada a supuestos identificados.

**Verificación:**

- [ ] La tabla comparativa cubre criterios tanto cuantitativos (precio, ahorro) como cualitativos (riesgo, relación).
- [ ] Los supuestos listados son específicos al caso (no genéricos).
- [ ] El participante identifica y anota al menos dos supuestos que variarían en su contexto real.
- [ ] La recomendación de Copilot incluye condicionantes explícitos.

---

#### Paso 2.2 — Generación de la matriz de decisión en Excel

**Objetivo:** Trasladar el análisis de Copilot a una matriz de decisión estructurada en Excel para formalizar el análisis multicriterio.

**Instrucciones:**

1. Abra el archivo `M4_Plantilla_Matriz_Decision.xlsx` desde OneDrive. La plantilla tiene columnas predefinidas: Criterio | Peso (%) | Puntaje AlphaSupply (1-10) | Puntaje BetaMaterials (1-10) | Score Ponderado Alpha | Score Ponderado Beta.

2. Haga clic en el botón de **Copilot** en la cinta de Excel (pestaña "Inicio" o "Copilot" si aparece como pestaña separada).

3. En el panel de Copilot de Excel, ingrese el siguiente prompt:

```text
Tengo una plantilla de matriz de decisión para evaluar dos proveedores.
Basándome en el análisis que realicé previamente, necesito que me ayudes
a completar la matriz con los siguientes criterios y pesos sugeridos:

Criterios a incluir:
- Precio/Costo total (Peso: 25%)
- Cumplimiento histórico de entregas (Peso: 20%)
- Riesgo de transición (Peso: 15%)
- Capacidad y escalabilidad (Peso: 15%)
- Certificaciones de calidad (Peso: 10%)
- Impacto logístico (Peso: 10%)
- Solidez de la relación comercial (Peso: 5%)

Para cada criterio, sugiere un puntaje del 1 al 10 para cada proveedor
(AlphaSupply y BetaMaterials) basado en la información del caso que te
proporciono a continuación:
[Pega aquí el resumen del caso del archivo M4_Caso_Decision_Sourcing.docx]

Explica brevemente la justificación de cada puntaje asignado.
```

4. Revise las sugerencias de Copilot. **No acepte automáticamente todos los puntajes**: ajuste al menos 2-3 valores basándose en su criterio profesional y conocimiento del caso. Documente el motivo del ajuste en la columna de comentarios de la plantilla.

5. Complete la fórmula de Score Ponderado en Excel (si no está pre-cargada):
   - En la celda de Score Ponderado Alpha: `=B[fila]*C[fila]/100`
   - En la celda de Score Ponderado Beta: `=B[fila]*D[fila]/100`
   - En la fila de Total: `=SUM(E2:E8)` y `=SUM(F2:F8)`

6. Guarde el archivo en OneDrive (Ctrl+S).

**Resultado Esperado:**

- La matriz de decisión está completada con los 7 criterios, pesos, puntajes y scores ponderados calculados.
- Al menos 2-3 puntajes fueron ajustados por el participante con justificación documentada en comentarios.
- El score total de cada proveedor es visible y permite una comparación directa.

**Verificación:**

- [ ] La suma de los pesos en la columna Peso (%) es igual al 100%.
- [ ] Los scores ponderados están calculados correctamente (fórmula verificable).
- [ ] Al menos dos celdas tienen comentarios de Excel con la justificación del ajuste manual.
- [ ] El archivo está guardado en OneDrive.

---

#### Paso 2.3 — Redacción del memo de decisión con Copilot en Word

**Objetivo:** Usar Copilot en Word para generar un memo formal de decisión que integre los hallazgos del análisis.

**Instrucciones:**

1. Abra un **nuevo documento de Word** y guárdelo inmediatamente en OneDrive con el nombre `M4_Memo_Decision_Sourcing_[SuNombre].docx`.

2. Haga clic en el ícono de **Copilot** en la cinta de Word (aparece en la pestaña "Inicio" como "Borrador con Copilot" o en el margen izquierdo del documento vacío).

3. En el campo de Copilot en Word, ingrese el siguiente prompt:

```text
Redacta un memorándum ejecutivo formal de toma de decisión con la
siguiente estructura:

ENCABEZADO: Para: Gerencia de Suministros | De: [Analista de Suministros]
| Fecha: [fecha actual] | Asunto: Análisis de cambio de proveedor de
materias primas — AlphaSupply vs BetaMaterials

SECCIONES:
1. Antecedentes (2 párrafos): Contexto de la evaluación y por qué se
   inició el proceso de revisión de proveedor.

2. Metodología de análisis (1 párrafo): Descripción del enfoque
   multicriterio utilizado (matriz de decisión con 7 criterios ponderados).

3. Hallazgos principales (lista de 4-5 puntos): Los hallazgos más
   relevantes del análisis comparativo entre AlphaSupply y BetaMaterials.

4. Recomendación (2 párrafos): Recomendación clara con justificación
   basada en el análisis. Si se recomienda un piloto, especificar las
   condiciones de éxito.

5. Próximos pasos (lista numerada de 3-4 acciones): Acciones concretas
   con responsables sugeridos y plazos aproximados.

Tono: Formal, técnico, orientado a decisión. Extensión total: 400-500 palabras.

Contexto del análisis: AlphaSupply (proveedor actual, 6 años, 97%
cumplimiento, $85/unidad) vs BetaMaterials (nuevo, $74/unidad, ISO 9001
e ISO 14001, sin historial, 800 km de distancia). La matriz de decisión
multicriterio muestra [incluir el score total de su matriz de Excel].
```

4. Revise el borrador generado por Copilot. Realice al menos **tres ajustes editoriales** para:
   - Incorporar datos específicos de su matriz de Excel (scores reales).
   - Ajustar el tono o precisión de algún párrafo según su criterio.
   - Agregar una nota al pie indicando: *"Este análisis fue asistido por Microsoft 365 Copilot. Los juicios, ajustes y la decisión final son responsabilidad del equipo de Suministros."*

5. Guarde el documento en OneDrive (Ctrl+S).

**Resultado Esperado:**

- Documento Word con el memo de decisión completo, formalmente estructurado en 5 secciones.
- El memo incorpora datos reales de la matriz de Excel (scores ponderados).
- Se incluye la nota de pie sobre el uso de Copilot.
- El documento tiene entre 400 y 550 palabras.

**Verificación:**

- [ ] El memo tiene las 5 secciones solicitadas con contenido sustantivo en cada una.
- [ ] Los scores de la matriz de Excel están referenciados en el memo.
- [ ] La nota al pie sobre Copilot está presente al final del documento.
- [ ] El archivo está guardado en OneDrive con el nombre correcto.

---

### Bloque 3: Análisis Inicial de Cambios Regulatorios con Copilot
**Tiempo estimado: 25 minutos**

---

#### Paso 3.1 — Procesamiento de extractos regulatorios con Copilot

**Objetivo:** Usar Copilot Chat para analizar extractos de normativas y regulaciones relevantes para Suministros, identificando impactos operativos.

**Instrucciones:**

1. Abra el archivo `M4_Extractos_Regulatorios.docx` desde OneDrive. El documento contiene extractos de tres normativas simuladas relevantes para Suministros:
   - **Normativa A:** Actualización de requisitos de documentación aduanera para importaciones (nuevos campos obligatorios en pedimentos).
   - **Normativa B:** Regulación ambiental sobre empaques y materiales de embalaje (restricciones a plásticos de un solo uso en cadena de suministro).
   - **Normativa C:** Estándar actualizado de trazabilidad para proveedores de materias primas críticas (requisito de certificación de origen y cadena de custodia).

2. Inicie una **nueva conversación** en Copilot Chat.

3. Ingrese el siguiente prompt de análisis regulatorio:

```text
Actúa como un especialista en cumplimiento regulatorio para operaciones
de cadena de suministro y comercio exterior.

Voy a proporcionarte extractos de tres normativas que afectan a nuestra
área de Suministros. Para cada normativa, necesito que realices el
siguiente análisis:

NORMATIVA A — [Pega el extracto de la Normativa A del documento]
NORMATIVA B — [Pega el extracto de la Normativa B del documento]
NORMATIVA C — [Pega el extracto de la Normativa C del documento]

ANÁLISIS REQUERIDO PARA CADA NORMATIVA:
1. Resumen de la normativa en 2-3 oraciones (lenguaje operativo, no legal)
2. Procesos de Suministros directamente afectados (lista específica)
3. Impacto operativo: ¿Qué cambia en la operación actual? (Alto/Medio/Bajo
   con justificación)
4. Plazo de cumplimiento implícito o explícito en el extracto
5. Acciones inmediatas recomendadas (primeras 3 cosas que debería hacer
   el equipo de Suministros)
6. Riesgos de incumplimiento identificados

FORMATO: Usa una sección por normativa con subtítulos claros.
Al final, incluye una tabla resumen: Normativa | Impacto | Urgencia |
Primera Acción Clave
```

4. Lea la respuesta completa de Copilot.

> ⚠️ **Advertencia crítica:** Recuerde que Copilot **no es un asesor legal**. El análisis generado es un punto de partida para identificar áreas de atención, no una interpretación jurídica vinculante. Cualquier decisión de cumplimiento regulatorio debe ser validada por el área legal o un experto en la materia.

5. En la respuesta de Copilot, identifique y marque visualmente (puede hacer una captura de pantalla o copiar el texto) al menos **una afirmación que requiera validación con el área legal** de su organización antes de actuar sobre ella.

**Resultado Esperado:**

- Copilot genera un análisis estructurado para las tres normativas con las 6 secciones solicitadas.
- La tabla resumen al final muestra las tres normativas con su nivel de impacto, urgencia y primera acción clave.
- El participante identifica al menos una afirmación que requiere validación legal.

**Verificación:**

- [ ] El análisis cubre las tres normativas con estructura consistente.
- [ ] La tabla resumen está presente y es coherente con el análisis detallado.
- [ ] El participante documenta (en papel o captura) la afirmación que requiere validación legal.
- [ ] Se comprende y verbaliza la limitación de Copilot como herramienta de apoyo (no asesor legal).

---

#### Paso 3.2 — Profundización en la normativa de mayor impacto

**Objetivo:** Usar el seguimiento conversacional de Copilot para desarrollar un plan de respuesta ante la normativa de mayor impacto operativo.

**Instrucciones:**

1. **Continuando la conversación** del Paso 3.1, identifique cuál de las tres normativas tiene el mayor impacto operativo según el análisis de Copilot.

2. Ingrese el siguiente prompt de profundización:

```text
De las tres normativas analizadas, identifica la que tiene mayor impacto
operativo para el área de Suministros.

Para esa normativa, desarrolla:

1. MAPA DE IMPACTO DETALLADO:
   - Subprocesos afectados (desglose de cada proceso impactado en
     subactividades específicas)
   - Sistemas o herramientas que requieren actualización (ERP, documentación,
     contratos con proveedores)
   - Roles o perfiles del equipo de Suministros que deben capacitarse

2. PLAN DE ACCIÓN DE 90 DÍAS:
   - Semanas 1-2: Acciones de diagnóstico y evaluación de brecha
   - Semanas 3-6: Acciones de adaptación e implementación
   - Semanas 7-12: Acciones de validación y consolidación
   Cada acción debe incluir: Descripción | Responsable sugerido | Entregable

3. INDICADORES DE CUMPLIMIENTO:
   Define 3 KPIs que permitan medir el avance hacia el cumplimiento
   de esta normativa. Para cada KPI: nombre, fórmula de cálculo,
   frecuencia de medición, meta objetivo.

Formato: Usa subtítulos, tablas donde aplique y listas numeradas.
```

3. Copie la respuesta completa de Copilot.

4. Abra un **nuevo documento de Word** y guárdelo en OneDrive como `M4_Plan_Respuesta_Regulatoria_[SuNombre].docx`.

5. Pegue el contenido del análisis en el documento Word. Agregue en la primera página un encabezado con:
   - Título: **"Plan de Respuesta a Cambio Regulatorio — Análisis Inicial"**
   - Subtítulo: *"Documento generado con apoyo de Microsoft 365 Copilot — Requiere validación del área Legal y Cumplimiento"*
   - Fecha y nombre del participante.

6. Guarde el documento en OneDrive (Ctrl+S).

**Resultado Esperado:**

- El plan de acción de 90 días está estructurado en tres fases con acciones específicas, responsables y entregables.
- Se definen 3 KPIs con fórmulas de cálculo claras.
- El documento Word está guardado en OneDrive con el encabezado de validación legal visible.

**Verificación:**

- [ ] El plan de 90 días tiene las tres fases temporales diferenciadas.
- [ ] Cada acción del plan incluye responsable sugerido y entregable.
- [ ] Los 3 KPIs tienen nombre, fórmula, frecuencia y meta.
- [ ] El documento Word tiene el encabezado con la advertencia de validación legal.

---

### Bloque 4: Generación de Checklists de Cumplimiento con Copilot
**Tiempo estimado: 21 minutos**

---

#### Paso 4.1 — Generación del checklist de cumplimiento regulatorio

**Objetivo:** Crear con Copilot una lista de verificación de cumplimiento regulatorio estructurada y adaptada al contexto operativo del área de Suministros.

**Instrucciones:**

1. Inicie una **nueva conversación** en Copilot Chat.

2. Ingrese el siguiente prompt para generar el checklist base:

```text
Actúa como un especialista en cumplimiento regulatorio y mejora de
procesos para cadena de suministro.

Basándome en el análisis de las tres normativas que hemos revisado
(documentación aduanera, empaques sostenibles, y trazabilidad de
proveedores), necesito que generes una lista de verificación de
cumplimiento regulatorio integral para el área de Suministros.

ESTRUCTURA DEL CHECKLIST:
Organiza la lista en 4 categorías:

CATEGORÍA 1 — Documentación y Registros
(Verificaciones relacionadas con la gestión de documentos, expedientes
de proveedores, registros de importación/exportación)

CATEGORÍA 2 — Procesos Operativos
(Verificaciones sobre cómo se ejecutan los procesos de recepción,
evaluación de proveedores, gestión de contratos)

CATEGORÍA 3 — Proveedores y Cadena de Valor
(Verificaciones sobre el cumplimiento de proveedores con las normativas,
certificaciones requeridas, trazabilidad)

CATEGORÍA 4 — Capacitación y Conciencia
(Verificaciones sobre si el equipo conoce y aplica los requisitos
regulatorios vigentes)

PARA CADA ÍTEM DEL CHECKLIST incluye:
- Número de ítem
- Descripción del punto de verificación (accionable, en formato de pregunta
  de sí/no o verificación observable)
- Normativa o estándar de referencia
- Frecuencia de verificación recomendada (Diaria/Semanal/Mensual/Trimestral/Anual)
- Evidencia requerida para confirmar cumplimiento
- Nivel de criticidad (Crítico/Importante/Recomendado)

Genera un mínimo de 5 ítems por categoría (20 ítems en total como mínimo).
```

3. Revise la respuesta de Copilot. Evalúe si los ítems son:
   - **Específicos y accionables** (se puede verificar con un sí/no claro).
   - **Relevantes** para el contexto de Suministros (no genéricos).
   - **Completos** (cubren las tres normativas del Bloque 3).

4. Si identifica ítems demasiado genéricos o faltantes, use el siguiente prompt de refinamiento:

```text
Los ítems [menciona los números específicos] son demasiado genéricos
para nuestro contexto operativo. Por favor:
1. Reescribe esos ítems haciéndolos más específicos para una operación
   de suministros en [sector/industria del participante].
2. Agrega 3 ítems adicionales en la categoría [categoría donde detectaste
   mayor brecha] que cubran [aspecto específico no cubierto].
```

**Resultado Esperado:**

- Copilot genera un checklist con al menos 20 ítems distribuidos en 4 categorías.
- Cada ítem incluye los 6 campos solicitados (número, descripción, normativa, frecuencia, evidencia, criticidad).
- El participante realiza al menos una iteración de refinamiento para mejorar la calidad del checklist.

**Verificación:**

- [ ] El checklist tiene al menos 20 ítems en total.
- [ ] Las 4 categorías están presentes y diferenciadas.
- [ ] Al menos 5 ítems están clasificados como "Crítico".
- [ ] Se realizó al menos una iteración de refinamiento con un prompt adicional.

---

#### Paso 4.2 — Transferencia del checklist a Excel y formateo

**Objetivo:** Trasladar el checklist generado por Copilot a una hoja de Excel estructurada y funcional para uso operativo.

**Instrucciones:**

1. Abra el archivo `M4_Plantilla_Checklist.xlsx` desde OneDrive. La plantilla tiene las columnas: N° | Categoría | Descripción del Punto | Normativa Referencia | Frecuencia | Evidencia Requerida | Criticidad | Estado (Cumple/No Cumple/N/A) | Observaciones | Responsable | Fecha Verificación.

2. Haga clic en el botón de **Copilot** en la cinta de Excel.

3. En el panel de Copilot de Excel, ingrese:

```text
Tengo un checklist de cumplimiento regulatorio que necesito organizar
en esta hoja de Excel. La hoja tiene las siguientes columnas:
N° | Categoría | Descripción del Punto | Normativa Referencia |
Frecuencia | Evidencia Requerida | Criticidad | Estado | Observaciones |
Responsable | Fecha Verificación

¿Puedes ayudarme a sugerir cómo aplicar formato condicional para que:
- Las filas con Criticidad "Crítico" se resalten en rojo claro
- Las filas con Criticidad "Importante" se resalten en amarillo claro
- Las filas con Estado "No Cumple" se resalten en naranja
- Las filas con Estado "Cumple" se resalten en verde claro?

Describe los pasos exactos para aplicar estas reglas de formato
condicional en Excel.
```

4. Siguiendo las instrucciones de Copilot, aplique el formato condicional en la hoja de Excel:
   - Seleccione el rango de datos (columna G para Criticidad, columna H para Estado).
   - Vaya a **Inicio > Formato Condicional > Nueva Regla**.
   - Aplique las 4 reglas de color descritas por Copilot.

5. Ingrese manualmente al menos **10 ítems del checklist** generado en el Paso 4.1 en la hoja de Excel, completando todas las columnas disponibles. Para los campos Estado y Fecha Verificación, use valores de ejemplo ("Cumple", "No Cumple", "N/A" y fechas actuales).

6. En el panel de Copilot de Excel, solicite:

```text
Analiza los datos ingresados en esta hoja de checklist. Identifica:
1. ¿Cuántos ítems están en estado "No Cumple"?
2. ¿Qué categoría tiene mayor proporción de incumplimientos?
3. ¿Qué ítem crítico en estado "No Cumple" debería atenderse primero?
Dame un resumen ejecutivo de 3 líneas con el estado de cumplimiento.
```

7. Guarde el archivo en OneDrive (Ctrl+S).

**Resultado Esperado:**

- La hoja de Excel tiene al menos 10 ítems del checklist ingresados con todas las columnas completadas.
- El formato condicional está aplicado y es visualmente funcional (colores correctos según criticidad y estado).
- Copilot genera un resumen del estado de cumplimiento basado en los datos ingresados.

**Verificación:**

- [ ] El formato condicional está aplicado y funciona correctamente (verificar cambiando un valor de Estado).
- [ ] Al menos 10 ítems están ingresados con todas las columnas completadas.
- [ ] El resumen ejecutivo de Copilot es coherente con los datos ingresados.
- [ ] El archivo está guardado en OneDrive.

---

#### Paso 4.3 — Refinamiento iterativo y entregable final

**Objetivo:** Realizar una iteración final de mejora del checklist usando Copilot y consolidar todos los entregables del laboratorio.

**Instrucciones:**

1. Regrese a Copilot Chat (puede continuar la conversación del Paso 4.1 o iniciar una nueva).

2. Ingrese el siguiente prompt de refinamiento final:

```text
Tengo un checklist de cumplimiento regulatorio para el área de Suministros
con 20+ ítems distribuidos en 4 categorías.

Ayúdame a mejorarlo con las siguientes acciones:

1. PRIORIZACIÓN: Reorganiza los ítems dentro de cada categoría en orden
   de prioridad de atención (del más urgente/crítico al menos urgente).
   Justifica el orden propuesto.

2. BRECHA DE COBERTURA: ¿Qué áreas o aspectos del cumplimiento regulatorio
   en suministros podrían estar faltando en un checklist de 4 categorías
   con los temas de documentación aduanera, empaques sostenibles y
   trazabilidad? Sugiere una quinta categoría opcional con 3-5 ítems.

3. INDICADORES DE MADUREZ: Propón una escala de madurez de cumplimiento
   de 4 niveles (Inicial, En Desarrollo, Gestionado, Optimizado) con
   criterios claros para que el área de Suministros pueda autoevaluar
   su nivel actual de cumplimiento regulatorio.

Formato: Listas ordenadas, tabla para la escala de madurez.
```

3. Incorpore la escala de madurez generada por Copilot como una segunda hoja en el archivo `M4_Plantilla_Checklist.xlsx`. Nombre la hoja **"Escala de Madurez"**.

4. Realice una **revisión final de todos los entregables** del laboratorio. Complete la siguiente tabla de autoevaluación en un nuevo documento Word o en la hoja de Excel:

| Entregable | Archivo | Estado | Observación |
|---|---|---|---|
| Hallazgos de validación — Proceso de Recepción | `M4_Proceso_Recepcion_Materiales.docx` | ☐ Completo | |
| Resumen ejecutivo — Proceso de Evaluación de Proveedores | `M4_Proceso_Evaluacion_Proveedores.docx` | ☐ Completo | |
| Matriz de decisión multicriterio | `M4_Plantilla_Matriz_Decision.xlsx` | ☐ Completo | |
| Memo de decisión de sourcing | `M4_Memo_Decision_Sourcing_[Nombre].docx` | ☐ Completo | |
| Plan de respuesta regulatoria 90 días | `M4_Plan_Respuesta_Regulatoria_[Nombre].docx` | ☐ Completo | |
| Checklist de cumplimiento en Excel | `M4_Plantilla_Checklist.xlsx` | ☐ Completo | |

5. Guarde todos los archivos abiertos en OneDrive (Ctrl+S en cada uno).

**Resultado Esperado:**

- La escala de madurez de 4 niveles está documentada en la segunda hoja del archivo Excel.
- Todos los entregables del laboratorio están completos y guardados en OneDrive.
- La tabla de autoevaluación está completada con el estado de cada entregable.

**Verificación:**

- [ ] El archivo Excel tiene dos hojas: "Checklist" y "Escala de Madurez".
- [ ] La escala de madurez tiene 4 niveles con criterios diferenciados para cada uno.
- [ ] Todos los archivos de entregables están en OneDrive (no en disco local).
- [ ] La tabla de autoevaluación indica "Completo" para todos los entregables.

---

## 7. Validación y Pruebas

Al finalizar todos los bloques, realice las siguientes verificaciones integrales:

### 7.1 Verificación de Calidad de Prompts

Revise los prompts que construyó durante el laboratorio y evalúe si cada uno cumple los tres componentes de la estructura aprendida en la lección:

| Prompt | ¿Tiene Contexto? | ¿Tiene Criterio de Evaluación? | ¿Tiene Formato de Salida? | Calificación (1-5) |
|---|---|---|---|---|
| Validación Proceso de Recepción (Paso 1.1) | ☐ Sí ☐ No | ☐ Sí ☐ No | ☐ Sí ☐ No | |
| Árbol de argumentos sourcing (Paso 2.1) | ☐ Sí ☐ No | ☐ Sí ☐ No | ☐ Sí ☐ No | |
| Análisis regulatorio (Paso 3.1) | ☐ Sí ☐ No | ☐ Sí ☐ No | ☐ Sí ☐ No | |
| Generación de checklist (Paso 4.1) | ☐ Sí ☐ No | ☐ Sí ☐ No | ☐ Sí ☐ No | |

### 7.2 Verificación de Entregables en OneDrive

Acceda a OneDrive for Business y confirme que los siguientes archivos existen en la carpeta `Curso_M365_Copilot/Modulo4/`:

```
✅ M4_Proceso_Recepcion_Materiales.docx        (con sección de hallazgos añadida)
✅ M4_Proceso_Evaluacion_Proveedores.docx      (con párrafo ejecutivo añadido)
✅ M4_Plantilla_Matriz_Decision.xlsx           (con matriz completada y comentarios)
✅ M4_Memo_Decision_Sourcing_[SuNombre].docx   (memo completo con nota al pie)
✅ M4_Plan_Respuesta_Regulatoria_[SuNombre].docx (plan de 90 días con KPIs)
✅ M4_Plantilla_Checklist.xlsx                 (checklist + hoja Escala de Madurez)
```

### 7.3 Prueba de Criterio Profesional

Responda las siguientes preguntas de reflexión (pueden discutirse en plenaria con el instructor):

1. **¿En qué momento durante el laboratorio sintió mayor necesidad de validar o corregir una respuesta de Copilot?** ¿Qué le indicó que la respuesta era insuficiente o incorrecta?

2. **De los cuatro tipos de análisis realizados** (validación de procesos, decisión de sourcing, análisis regulatorio, checklist), ¿en cuál considera que Copilot agregó más valor? ¿En cuál fue menos confiable? ¿Por qué?

3. **¿Cómo cambiaría su proceso de toma de decisiones** en el trabajo diario si incorporara sistemáticamente el uso de Copilot para estructurar análisis antes de presentarlos a la gerencia?

---

## 8. Solución de Problemas

### Problema 1: Copilot genera respuestas genéricas o superficiales que no son útiles para el análisis

**Síntoma:** La respuesta de Copilot es vaga, usa términos genéricos como "mejorar la comunicación" o "optimizar procesos" sin especificidad, o repite el mismo contenido con diferentes palabras sin profundidad analítica real.

**Causa probable:** El prompt no incluye suficiente contexto específico del proceso o caso. Copilot no puede generar análisis profundos si solo recibe descripciones generales. Otro factor común es que el prompt no especifica el formato de salida ni el nivel de detalle requerido, por lo que Copilot responde con el nivel mínimo.

**Solución:**
1. Regrese al prompt original y agregue más detalles específicos: nombres de sistemas (SAP, Oracle), cantidades, tiempos, actores concretos, y restricciones reales del proceso.
2. Agregue explícitamente al prompt: *"Sé específico y técnico. Evita recomendaciones genéricas. Cada hallazgo debe estar directamente vinculado a un paso del proceso que describí."*
3. Use el prompt de seguimiento: *"Tu respuesta anterior fue demasiado general. Profundiza en el punto [X] con ejemplos concretos de cómo se manifiesta el problema en el proceso descrito y cuál sería el impacto medible en tiempo o costo."*
4. Si el problema persiste, divida el análisis: en lugar de pedir todo en un solo prompt, solicite primero solo los hallazgos, luego las recomendaciones, y finalmente el formato de salida. Esto obliga a Copilot a procesar cada parte con mayor profundidad.

---

### Problema 2: Copilot en Excel no responde o el botón de Copilot no aparece en la cinta

**Síntoma:** El botón de Copilot no es visible en la pestaña "Inicio" de Excel, o al hacer clic aparece un mensaje de error como *"Copilot no está disponible"*, *"No se puede conectar"*, o el panel lateral de Copilot se abre pero no responde a los prompts ingresados.

**Causa probable:** Existen tres causas frecuentes: (a) el archivo de Excel está guardado en disco local y no en OneDrive for Business (Copilot en Excel requiere que el archivo esté en OneDrive o SharePoint para funcionar); (b) la licencia de Microsoft 365 Copilot no está activa para la cuenta del usuario o no se ha propagado correctamente; (c) la versión de Excel instalada es anterior a la 2406 y no incluye la integración de Copilot.

**Solución:**
1. **Verificar ubicación del archivo:** Revise la barra de título de Excel. Si muestra una ruta local (C:\Users\...), el archivo no está en OneDrive. Vaya a `Archivo > Guardar como > OneDrive for Business` y guarde el archivo allí. Cierre y vuelva a abrir el archivo desde OneDrive.
2. **Verificar licencia:** Vaya a `Archivo > Cuenta` en Excel. En la sección "Información del producto", verifique que aparece "Microsoft 365 Apps for Enterprise". Si Copilot no aparece como función disponible, contacte al administrador de TI para confirmar que la licencia Copilot está asignada a su cuenta en el portal de administración de Microsoft 365.
3. **Verificar versión:** En `Archivo > Cuenta > Acerca de Excel`, confirme que la versión es 2406 o posterior. Si es anterior, ejecute `Archivo > Cuenta > Opciones de actualización > Actualizar ahora`.
4. **Alternativa inmediata:** Si el problema persiste durante el laboratorio, realice el análisis de Excel en Copilot Chat (copilot.microsoft.com) describiendo la estructura de su tabla y solicitando las sugerencias de formato condicional o análisis. Luego aplique manualmente los resultados en Excel.

---

## 9. Limpieza del Entorno

Al finalizar el laboratorio, realice los siguientes pasos de cierre:

### 9.1 Organización de Archivos en OneDrive

1. Acceda a OneDrive for Business y confirme que todos los archivos de entregables están en la carpeta `Curso_M365_Copilot/Modulo4/`.
2. Cree una subcarpeta llamada `Entregables_Lab04` dentro de `Modulo4/` y mueva los archivos generados por usted (los que tienen `[SuNombre]` en el nombre) a esa subcarpeta.
3. Los archivos de práctica originales (sin modificaciones de nombre) pueden permanecer en `Modulo4/`.

### 9.2 Cierre de Sesiones y Aplicaciones

1. Guarde y cierre todos los documentos de Word y Excel abiertos (Ctrl+S, luego Alt+F4 o clic en "X").
2. En Copilot Chat ([copilot.microsoft.com](https://copilot.microsoft.com)), las conversaciones se guardan automáticamente en el historial. No es necesario borrarlas, pero puede limpiar el historial si lo prefiere desde `Configuración > Historial de conversaciones`.
3. Si trabajó en un equipo compartido o de laboratorio, cierre la sesión de Microsoft 365: en el navegador, haga clic en su foto de perfil (esquina superior derecha) y seleccione **"Cerrar sesión"**.
4. Cierre todas las pestañas del navegador relacionadas con Microsoft 365 y Copilot.

### 9.3 Verificación Final de Privacidad

- [ ] Confirme que no ingresó información confidencial real de la organización en ningún prompt de Copilot durante el laboratorio.
- [ ] Confirme que todos los archivos de entregables están en OneDrive (no en escritorio ni en carpetas locales compartidas).
- [ ] Si tomó capturas de pantalla de respuestas de Copilot, verifique que no contengan datos sensibles antes de compartirlas.

---

## 10. Resumen y Recursos

### Puntos Clave del Laboratorio

Este laboratorio demostró en la práctica cuatro aplicaciones avanzadas de Microsoft 365 Copilot en el contexto de gobernanza y toma de decisiones en Suministros:

1. **Validación de procesos operativos:** Copilot actúa como un revisor analítico estructurado cuando se le proporciona el proceso completo, el criterio de evaluación y el formato de salida deseado. La clave es el nivel de detalle del contexto aportado por el profesional de suministros.

2. **Apoyo en decisiones críticas:** Los prompts de árbol de argumentos (riesgos, beneficios, supuestos, preguntas pendientes) permiten a Copilot generar análisis documentados y trazables que elevan la calidad de las decisiones de sourcing y reducen el sesgo de confirmación.

3. **Análisis inicial de cambios regulatorios:** Copilot puede procesar extractos normativos y traducirlos a impactos operativos concretos, pero sus conclusiones **siempre requieren validación por expertos legales** antes de actuar sobre ellas. Es una herramienta de primer filtro, no de interpretación jurídica.

4. **Generación iterativa de checklists:** La creación de herramientas de cumplimiento con Copilot es más efectiva cuando se itera: generar un borrador, evaluar brechas, refinar con prompts específicos, y adaptar al contexto organizacional real.

5. **Criterio profesional como filtro final:** En todos los bloques, el valor diferencial del profesional de suministros fue su capacidad para evaluar críticamente las respuestas de Copilot, identificar supuestos cuestionables, ajustar puntajes en la matriz y agregar contexto organizacional que Copilot no puede conocer por sí solo.

### Patrones de Prompts de Referencia (Banco de Prompts)

Guarde estos patrones como referencia para uso futuro en su trabajo diario:

```text
PATRÓN 1 — Validación de proceso:
"Actúa como [rol experto]. Analiza el siguiente proceso de [nombre del proceso]:
[descripción del proceso]. Evalúalo desde la perspectiva de [criterio 1] y
[criterio 2]. Entrega: [formato específico]."

PATRÓN 2 — Decisión crítica:
"Contexto: [descripción del caso]. Tarea: Construye un árbol de argumentos
con: (a) razones para [opción A], (b) razones para [opción B], (c) supuestos
a validar, (d) preguntas críticas pendientes. Formato: tabla + lista + recomendación."

PATRÓN 3 — Análisis regulatorio:
"Actúa como especialista en cumplimiento para [sector]. Analiza el siguiente
extracto de normativa: [extracto]. Identifica: (1) resumen operativo,
(2) procesos afectados, (3) impacto (Alto/Medio/Bajo), (4) acciones inmediatas,
(5) riesgos de incumplimiento."

PATRÓN 4 — Generación de checklist:
"Genera un checklist de cumplimiento para [área/proceso] organizado en
[N] categorías: [lista de categorías]. Para cada ítem incluye:
descripción accionable | referencia normativa | frecuencia | evidencia requerida |
criticidad. Mínimo [N] ítems por categoría."
```

### Recursos de Referencia

| Recurso | Descripción | URL |
|---|---|---|
| Microsoft Copilot para Microsoft 365 — Documentación oficial | Guía completa de funcionalidades y mejores prácticas | [learn.microsoft.com/es-es/copilot/microsoft-365](https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-overview) |
| APICS/ASCM — Estándares de cadena de suministro | Marco de referencia para procesos y métricas de suministros | [ascm.org](https://www.ascm.org/learning-development/certifications-credentials/cscp/) |
| ISO 9001 — Gestión de calidad y auditoría de procesos | Estándar de referencia para validación de procesos operativos | [iso.org/iso-9001](https://www.iso.org/iso-9001-quality-management.html) |
| Microsoft Copilot en Excel — Guía de funcionalidades | Referencia específica para uso de Copilot en hojas de cálculo | [support.microsoft.com/copilot-excel](https://support.microsoft.com/es-es/office/copilot-en-excel) |
| HBR — Toma de decisiones basada en evidencia en compras | Artículos de referencia sobre decisiones estructuradas en supply chain | [hbr.org/topic/supply-chain-management](https://hbr.org/topic/subject/supply-chain-management) |

### Conexión con la Siguiente Lección

En la **Lección 4.2: Análisis de Cambios Regulatorios y Preparación de Listas de Cumplimiento**, profundizará en el análisis regulatorio iniciado en el Bloque 3 de este laboratorio. Se trabajará con un conjunto más amplio de normativas, se desarrollarán matrices de impacto regulatorio y se construirán programas de cumplimiento más completos. Se recomienda que, antes de la siguiente sesión, revise el Plan de Respuesta Regulatoria que generó en este laboratorio (archivo `M4_Plan_Respuesta_Regulatoria_[SuNombre].docx`) y reflexione sobre qué aspectos requieren validación con el área legal de su organización.

---

> 📌 **Recordatorio final:** Copilot es un acelerador del juicio profesional, no un sustituto. Cada análisis, recomendación o checklist generado con Copilot en este laboratorio es un punto de partida que requiere su criterio experto, el conocimiento de su organización y, en temas regulatorios, la validación de especialistas legales antes de convertirse en una decisión o documento oficial.

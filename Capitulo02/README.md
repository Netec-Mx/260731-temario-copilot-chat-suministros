# Aplicación de Copilot como apoyo en investigaciones de mercado, análisis de precios, benchmarking y evaluación de tendencias relevantes para Suministros.

---

## 1. Metadatos del Laboratorio

| Atributo            | Detalle                                                                 |
|---------------------|-------------------------------------------------------------------------|
| **Duración**        | 72 minutos                                                              |
| **Complejidad**     | Media                                                                   |
| **Nivel Bloom**     | Aplicar (Apply)                                                         |
| **Módulo**          | Módulo 2 — Investigación de Mercado y Análisis de Precios con Copilot  |
| **Modalidad**       | Guiado con práctica individual                                          |
| **Prerequisito**    | Lab 01 completado o experiencia básica con Copilot Chat                 |

---

## 2. Descripción General

En este laboratorio, los participantes asumirán el rol de analistas de compras estratégicas y utilizarán **Microsoft Copilot Chat** y **Copilot en Excel** para investigar el mercado de una categoría de suministro asignada, construir análisis comparativos de precios, diseñar un scorecard de benchmarking de proveedores y generar un reporte de tendencias. El laboratorio aplica directamente el marco de cinco componentes para la construcción de prompts efectivos estudiado en la Lección 2.1, reforzando el flujo de trabajo de tres etapas: contextualizar → profundizar → generar entregable. Al finalizar, cada participante contará con un conjunto de artefactos reutilizables para su trabajo real en suministros.

> ⚠️ **Recordatorio de privacidad:** Durante todo el laboratorio utiliza únicamente los archivos de práctica proporcionados. **No ingreses datos reales de proveedores, precios contractuales ni información financiera sensible de tu organización en Copilot.**

---

## 3. Objetivos de Aprendizaje

Al completar este laboratorio, serás capaz de:

- [ ] **Construir prompts estructurados** con los cinco componentes clave (contexto, objetivo, alcance temporal, formato de salida y variables de interés) para obtener investigaciones de mercado accionables en Copilot Chat.
- [ ] **Aplicar el flujo de tres etapas** (contextualizar → profundizar → generar entregable) para analizar precios de una categoría de suministro e identificar oportunidades de ahorro o riesgo.
- [ ] **Diseñar y completar una matriz de benchmarking de proveedores** utilizando Copilot para estructurar criterios comparativos y generar recomendaciones de selección.
- [ ] **Generar un reporte de tendencias de mercado** en formato ejecutivo apoyándote en Copilot, integrando factores macroeconómicos, disrupciones logísticas y señales de riesgo relevantes para la categoría analizada.
- [ ] **Validar críticamente** las respuestas de Copilot, identificando cuándo se requiere contraste con fuentes externas verificables.

---

## 4. Prerrequisitos

### Conocimiento Previo
- Haber completado el Módulo 1 del curso o contar con experiencia básica en el uso de Copilot Chat (conversación, iteración de prompts).
- Familiaridad con los conceptos de sourcing, evaluación de proveedores, benchmarking de precios y análisis de categorías de compra.
- Conocimiento básico de Microsoft Excel (tablas, formato condicional, gráficas simples).

### Acceso y Licencias
- Cuenta corporativa de Microsoft 365 con **licencia Copilot activa y verificada** (sin esta licencia el laboratorio no puede ejecutarse).
- Acceso confirmado a [copilot.microsoft.com](https://copilot.microsoft.com) o a Copilot dentro de Microsoft Teams.
- Acceso a Microsoft Excel con Copilot habilitado (versión 2406 o posterior).
- Los archivos de práctica del Módulo 2 deben estar **guardados en OneDrive for Business** (no en disco local).

### Archivos de Práctica Requeridos
| Archivo | Descripción | Ubicación |
|---------|-------------|-----------|
| `Lab02_Matriz_Proveedores.xlsx` | Matriz de proveedores con datos históricos de precios | OneDrive for Business |
| `Lab02_Datos_Precios_Historicos.xlsx` | Historial de precios por categoría (últimos 24 meses) | OneDrive for Business |
| `Lab02_Plantilla_Scorecard.xlsx` | Plantilla de scorecard de benchmarking (en blanco) | OneDrive for Business |

> 📌 **Nota del instructor:** Antes de comenzar, verificar que todos los participantes pueden abrir los tres archivos desde OneDrive y que Copilot aparece en la cinta de opciones de Excel.

---

## 5. Entorno del Laboratorio

### Hardware Recomendado

| Componente | Mínimo Requerido | Recomendado |
|------------|-----------------|-------------|
| Procesador | Intel Core i5 8ª gen / AMD Ryzen 5 | Intel Core i7 / AMD Ryzen 7 |
| RAM | 8 GB | 16 GB |
| Almacenamiento libre | 10 GB | 20 GB |
| Conexión a internet | 10 Mbps estable | 25 Mbps o superior |
| Resolución de pantalla | 1366 × 768 | 1920 × 1080 |

### Software Requerido

| Aplicación | Versión Mínima | Uso en el Lab |
|------------|---------------|---------------|
| Microsoft Copilot Chat | Acceso vía copilot.microsoft.com o Teams | Bloques 1, 3 y 4 |
| Microsoft Excel con Copilot | Versión 2406 o posterior | Bloque 2 |
| Microsoft Edge o Chrome | Versión 120 o posterior | Acceso a Copilot Chat |
| OneDrive for Business | Versión en la nube | Almacenamiento de archivos |

### Verificación del Entorno (antes de comenzar)

Ejecuta los siguientes pasos de verificación en los primeros **5 minutos** del laboratorio:

**Verificación 1 — Copilot Chat activo:**
1. Abre un navegador y navega a `https://copilot.microsoft.com`
2. Inicia sesión con tu cuenta corporativa de Microsoft 365
3. Confirma que puedes escribir un mensaje y recibir respuesta
4. Verifica que aparezca el modo **"Trabajo"** (Work) en el selector de contexto

**Verificación 2 — Copilot en Excel activo:**
1. Abre `Lab02_Matriz_Proveedores.xlsx` desde OneDrive (no descargues el archivo)
2. En la cinta de opciones de Excel, confirma que el botón **Copilot** aparece en la pestaña **Inicio**
3. Haz clic en el botón Copilot para abrir el panel lateral; debe abrirse sin errores

**Verificación 3 — Archivos en OneDrive:**
```
Ruta esperada en OneDrive: 
Mi OneDrive for Business > Curso M365 Copilot > Módulo 2 > [archivos de práctica]
```

> ❌ **Si alguna verificación falla:** Notifica al instructor de inmediato antes de continuar. No avances con archivos guardados en disco local.

---

## 6. Instrucciones Paso a Paso

El laboratorio se divide en **cuatro bloques** con tiempos estimados:

| Bloque | Actividad | Tiempo Estimado |
|--------|-----------|-----------------|
| Bloque 1 | Investigación de mercado con Copilot Chat | 18 minutos |
| Bloque 2 | Análisis de precios con Copilot en Excel | 18 minutos |
| Bloque 3 | Benchmarking de proveedores con Copilot | 20 minutos |
| Bloque 4 | Evaluación de tendencias y reporte ejecutivo | 16 minutos |

---

### Bloque 1: Investigación de Mercado con Copilot Chat

**Objetivo del bloque:** Construir prompts estructurados con los cinco componentes clave para obtener un panorama de mercado completo sobre la categoría de suministro asignada.

> 🏭 **Categoría de práctica:** Para este laboratorio utilizaremos **empaques industriales de cartón corrugado** como categoría de suministro. Si el instructor ha asignado una categoría diferente a tu grupo, reemplaza las referencias en los prompts según corresponda.

---

#### Paso 1.1 — Construir el Prompt de Investigación de Mercado Inicial

**Objetivo:** Aplicar el marco de cinco componentes para generar un panorama de mercado estructurado.

**Instrucciones:**

1. Abre Copilot Chat en `https://copilot.microsoft.com` y selecciona el modo **Trabajo (Work)** en el selector de contexto.

2. Inicia una **nueva conversación** haciendo clic en el ícono de lápiz o en "Nueva conversación".

3. Copia y pega el siguiente prompt en el campo de texto. Observa cómo cada línea corresponde a uno de los cinco componentes del marco aprendido en la Lección 2.1:

```
Contexto: Soy analista de compras estratégicas de una empresa 
manufacturera mediana en México. Estoy evaluando la categoría 
de empaques industriales de cartón corrugado para la renovación 
de contratos del próximo año fiscal.

Objetivo: Necesito un panorama completo del mercado de cartón 
corrugado industrial para tomar decisiones de sourcing informadas.

Alcance temporal: Condiciones actuales del mercado en 2024-2025 
y proyección a los próximos 6 meses.

Variables de interés: Considera el precio de la celulosa como 
materia prima, costos de energía en la producción, tipo de cambio 
peso-dólar, capacidad instalada de los principales fabricantes 
en México y Latinoamérica, y disrupciones logísticas recientes.

Formato de salida: Presenta la información en tres secciones:
1. Resumen del estado actual del mercado (máximo 150 palabras)
2. Tabla con los 5 principales factores que impactan el precio 
   y su tendencia actual (al alza, estable, a la baja)
3. Lista de 5 preguntas estratégicas que debería hacerle a mis 
   proveedores actuales para validar competitividad de precios
```

4. Envía el prompt y espera la respuesta completa de Copilot.

5. **Lee la respuesta completa** antes de continuar. Evalúa si:
   - El resumen de mercado es coherente y específico para la categoría
   - La tabla de factores incluye tendencias claras
   - Las preguntas estratégicas son aplicables a una negociación real

6. En tu cuaderno o en un documento de Word, anota **2 observaciones** sobre la calidad de la respuesta: qué fue útil y qué requeriría validación con fuentes externas.

**Resultado esperado:**
- Una respuesta de Copilot con las tres secciones solicitadas
- El resumen debe mencionar factores como precio de celulosa, costos energéticos y/o condiciones de oferta/demanda
- La tabla debe contener al menos 4 de los 5 factores solicitados con una indicación de tendencia
- Las preguntas estratégicas deben ser específicas para negociación de empaques, no genéricas

**Verificación:**
> ✅ Confirma que tu respuesta contiene las tres secciones estructuradas. Si Copilot generó una respuesta sin estructura o muy genérica, procede al Paso 1.2 antes de continuar.

---

#### Paso 1.2 — Iterar y Profundizar el Análisis

**Objetivo:** Aplicar la segunda etapa del flujo de trabajo (profundizar mediante iteración) para obtener información más específica y accionable.

**Instrucciones:**

1. **Sin cerrar la conversación actual**, envía el siguiente prompt de seguimiento en el mismo hilo:

```
De los factores que identificaste, ¿cuáles tienen mayor impacto 
en el precio del cartón corrugado específicamente en mercados 
latinoamericanos como México, Colombia o Brasil? 

Adicionalmente, menciona 3 fuentes públicas o índices de referencia 
que un comprador profesional debería consultar regularmente para 
monitorear el precio de esta categoría. Para cada fuente, indica 
qué tipo de dato ofrece y con qué frecuencia se actualiza.
```

2. Espera la respuesta y evalúa si las fuentes mencionadas son reconocibles (por ejemplo: índices del Banco Mundial, reportes de RISI/Fisher International, CANAINPA en México, etc.).

3. Envía un tercer prompt para generar un entregable concreto:

```
Con base en el análisis que hemos construido hasta ahora, 
redacta un resumen ejecutivo de máximo 200 palabras dirigido 
a un gerente de compras. El resumen debe explicar:
- El contexto actual del mercado de cartón corrugado
- Los 3 factores de mayor riesgo para nuestra posición de compra
- Una recomendación concreta sobre si es momento favorable 
  para negociar contratos anuales o conviene esperar

Usa un tono profesional y directo, apropiado para una 
presentación interna de compras.
```

4. **Copia el resumen ejecutivo generado** y pégalo en un documento de Word nuevo. Guárdalo en tu carpeta de OneDrive como `Lab02_Resumen_Mercado_[TuNombre].docx`.

5. Agrega al inicio del documento una nota manual con la fecha y la categoría analizada.

**Resultado esperado:**
- Un resumen ejecutivo coherente de aproximadamente 150-200 palabras
- El documento guardado en OneDrive con tu nombre en el título
- El resumen debe incluir una recomendación de acción, no solo descripción

**Verificación:**
> ✅ Abre el archivo guardado en OneDrive y confirma que el contenido se guardó correctamente. El documento debe tener al menos dos párrafos y una recomendación explícita.

---

### Bloque 2: Análisis de Precios con Copilot en Excel

**Objetivo del bloque:** Utilizar Copilot dentro de Excel para analizar datos históricos de precios, identificar desviaciones y detectar oportunidades de ahorro o señales de riesgo.

---

#### Paso 2.1 — Explorar los Datos Históricos de Precios con Copilot

**Objetivo:** Activar Copilot en Excel y realizar un análisis exploratorio de los datos históricos de precios del archivo de práctica.

**Instrucciones:**

1. Desde OneDrive for Business, abre el archivo `Lab02_Datos_Precios_Historicos.xlsx`. **Asegúrate de abrirlo directamente desde OneDrive**, no desde una copia local.

2. Revisa brevemente la estructura del archivo. Debe contener:
   - Columna A: Mes/Período (últimos 24 meses)
   - Columna B: Precio unitario pagado (en moneda local)
   - Columna C: Proveedor
   - Columna D: Volumen comprado
   - Columna E: Precio de referencia de mercado (benchmark)

3. Haz clic en cualquier celda dentro de la tabla de datos para activar el contexto.

4. En la pestaña **Inicio** de la cinta de opciones, haz clic en el botón **Copilot** para abrir el panel lateral.

5. En el panel de Copilot, escribe el siguiente prompt:

```
Analiza los datos de esta tabla. Identifica:
1. El mes con el precio unitario más alto y más bajo en el período
2. La diferencia porcentual promedio entre el precio pagado 
   y el precio de referencia de mercado (columna E)
3. Si existe algún proveedor con precios consistentemente 
   por encima del benchmark de mercado
Presenta los resultados en formato de tabla resumen.
```

6. Observa cómo Copilot analiza los datos directamente en el contexto de la hoja de Excel y genera una respuesta en el panel lateral.

7. Si Copilot sugiere insertar una fórmula o crear una columna adicional, acepta la sugerencia haciendo clic en **"Insertar en hoja"** o **"Aplicar"** según aparezca en el panel.

**Resultado esperado:**
- Copilot identifica los períodos de precio máximo y mínimo
- Se calcula o estima la desviación promedio respecto al benchmark
- Si existe un proveedor con precios consistentemente superiores al mercado, Copilot lo señala

**Verificación:**
> ✅ Confirma que el panel de Copilot muestra resultados numéricos específicos (no solo texto genérico). Si la respuesta es muy vaga, verifica que la tabla tenga formato de Tabla de Excel (Ctrl+T) y repite el prompt.

---

#### Paso 2.2 — Identificar Desviaciones y Oportunidades de Ahorro

**Objetivo:** Usar Copilot en Excel para calcular desviaciones de precio y cuantificar oportunidades de ahorro potencial.

**Instrucciones:**

1. En el mismo panel de Copilot en Excel, envía el siguiente prompt de seguimiento:

```
Agrega una columna nueva llamada "Desviación vs Benchmark (%)" 
que calcule el porcentaje de diferencia entre el precio pagado 
(columna B) y el precio de referencia de mercado (columna E). 
Usa la fórmula: ((Precio Pagado - Precio Benchmark) / Precio 
Benchmark) * 100. Redondea a 2 decimales.
```

2. Acepta la sugerencia de Copilot para insertar la fórmula en la hoja.

3. Una vez creada la columna, envía el siguiente prompt:

```
Con base en la columna de desviación que acabamos de crear, 
identifica:
- ¿En cuántos períodos el precio pagado superó el benchmark 
  en más de 5%?
- ¿Cuál es el ahorro potencial acumulado si hubiéramos pagado 
  el precio benchmark en esos períodos? (usa el volumen de 
  la columna D para el cálculo)
- ¿Qué patrón observas en los meses donde la desviación 
  es mayor?
```

4. Revisa los resultados. Toma nota del **ahorro potencial acumulado** identificado por Copilot; lo usarás en el Bloque 3.

5. Envía un último prompt en Excel para generar una visualización:

```
Crea una gráfica de líneas que muestre la evolución del precio 
pagado versus el precio benchmark a lo largo del tiempo 
(columna A en el eje X). Titúlala "Comparativo de Precios: 
Pagado vs. Benchmark de Mercado".
```

6. Acepta la creación de la gráfica y ajusta su tamaño si es necesario para que sea legible.

7. **Guarda el archivo** con Ctrl+S (se guardará automáticamente en OneDrive).

**Resultado esperado:**
- Nueva columna "Desviación vs Benchmark (%)" con valores calculados
- Identificación de períodos con desviación superior al 5%
- Un valor de ahorro potencial acumulado (en moneda local)
- Una gráfica de líneas comparativa visible en la hoja de Excel

**Verificación:**
> ✅ Verifica que la columna de desviación tiene valores numéricos (positivos = pagamos más que el mercado, negativos = pagamos menos). Confirma que la gráfica muestra dos series de datos claramente diferenciadas. Si la gráfica no se generó, crea una manualmente usando los datos de las columnas A, B y E.

---

### Bloque 3: Benchmarking de Proveedores con Copilot

**Objetivo del bloque:** Diseñar y completar una matriz de benchmarking de proveedores utilizando Copilot para estructurar criterios comparativos y generar recomendaciones de selección.

---

#### Paso 3.1 — Diseñar los Criterios del Scorecard con Copilot Chat

**Objetivo:** Utilizar Copilot Chat para definir los criterios más relevantes para el benchmarking de proveedores de la categoría analizada.

**Instrucciones:**

1. Regresa a la ventana de **Copilot Chat** (`https://copilot.microsoft.com`).

2. Inicia una **nueva conversación** (no continúes el hilo del Bloque 1 para mantener el contexto limpio).

3. Envía el siguiente prompt para diseñar el scorecard:

```
Actúa como un consultor especialista en gestión de compras 
estratégicas. Estoy construyendo un scorecard de benchmarking 
para evaluar y comparar proveedores de empaques industriales 
de cartón corrugado.

Necesito que me propongas:
1. Los 6 criterios más relevantes para evaluar proveedores 
   en esta categoría (considera precio, calidad, tiempo de 
   entrega, capacidad de respuesta, riesgo financiero del 
   proveedor y sostenibilidad)
2. Para cada criterio: una descripción breve, el peso 
   porcentual sugerido (el total debe sumar 100%) y una 
   escala de evaluación del 1 al 5 con descripción de 
   qué significa cada nivel
3. Una justificación de por qué estos criterios son 
   prioritarios para una empresa manufacturera

Presenta la información en formato de tabla estructurada.
```

4. Revisa la respuesta. Si algún criterio no es relevante para tu contexto o el instructor ha indicado criterios específicos del sector, envía un prompt de ajuste:

```
Ajusta el scorecard: reemplaza el criterio de [criterio que 
quieres cambiar] por uno enfocado en [nuevo criterio, 
por ejemplo: "flexibilidad en volúmenes mínimos de pedido"]. 
Recalcula los pesos para que sumen 100% y actualiza la tabla.
```

5. Una vez que tengas el scorecard definitivo, **copia la tabla de criterios** (criterio, peso %, escala 1-5) y pégala en el archivo `Lab02_Plantilla_Scorecard.xlsx` en la hoja "Criterios".

**Resultado esperado:**
- Una tabla con 6 criterios de evaluación, pesos porcentuales que suman 100% y escala de calificación definida
- Los criterios deben cubrir al menos las dimensiones: precio, calidad, entrega, riesgo
- La información copiada en el archivo Excel de práctica

**Verificación:**
> ✅ Confirma que los pesos porcentuales de todos los criterios suman exactamente 100%. Si no suman 100%, pide a Copilot que corrija los pesos antes de continuar.

---

#### Paso 3.2 — Completar la Matriz de Benchmarking con Copilot

**Objetivo:** Usar Copilot para simular la evaluación comparativa de tres proveedores ficticios y generar recomendaciones de selección.

**Instrucciones:**

1. Abre el archivo `Lab02_Matriz_Proveedores.xlsx` desde OneDrive. Este archivo contiene datos de tres proveedores ficticios: **Proveedor Alpha**, **Proveedor Beta** y **Proveedor Gamma**, con información sobre precios, tiempos de entrega, incidencias de calidad y otros indicadores.

2. Revisa los datos disponibles para cada proveedor en la hoja "Datos_Proveedores".

3. Activa el panel de **Copilot en Excel** (pestaña Inicio → botón Copilot).

4. Envía el siguiente prompt en el panel de Copilot de Excel:

```
Tengo datos de tres proveedores (Alpha, Beta y Gamma) en esta 
hoja. Con base en los datos disponibles, ayúdame a:
1. Calcular una puntuación ponderada para cada proveedor 
   usando los siguientes pesos: Precio 30%, Calidad 25%, 
   Tiempo de entrega 20%, Capacidad de respuesta 15%, 
   Riesgo financiero 10%
2. Identificar cuál proveedor tiene el mejor desempeño 
   general y cuál representa mayor riesgo
3. Señalar si algún proveedor tiene una fortaleza 
   significativa en algún criterio específico que 
   podría ser aprovechada en negociación
```

5. Revisa los resultados. Si Copilot propone crear columnas de cálculo, acepta la sugerencia.

6. Regresa a **Copilot Chat** y envía el siguiente prompt para generar la recomendación ejecutiva:

```
Con base en el siguiente resumen de puntuaciones de 
proveedores de cartón corrugado:
- Proveedor Alpha: [ingresa la puntuación obtenida en Excel]
- Proveedor Beta: [ingresa la puntuación obtenida en Excel]
- Proveedor Gamma: [ingresa la puntuación obtenida en Excel]

Genera una recomendación de selección de proveedor de 
máximo 150 palabras que incluya:
1. El proveedor recomendado como principal y la justificación
2. Una sugerencia sobre si conviene mantener un segundo 
   proveedor como respaldo (dual sourcing) y por qué
3. Una acción de mejora específica que deberíamos negociar 
   con el proveedor seleccionado en el próximo contrato
```

> 📝 **Nota:** Reemplaza los corchetes `[ingresa la puntuación obtenida en Excel]` con los valores reales que Copilot calculó en el paso anterior.

7. Copia la recomendación generada y pégala en la hoja "Recomendación" del archivo `Lab02_Plantilla_Scorecard.xlsx`.

8. Guarda el archivo en OneDrive con Ctrl+S.

**Resultado esperado:**
- Puntuaciones ponderadas calculadas para los tres proveedores
- Un proveedor identificado como recomendado con justificación
- Una recomendación sobre estrategia de sourcing (single vs. dual)
- La recomendación guardada en el archivo de scorecard

**Verificación:**
> ✅ Confirma que las puntuaciones ponderadas están en el rango de 1 a 5 y que el proveedor con mayor puntuación es coherente con los datos disponibles (no debería ser el proveedor con peor historial de calidad o precios más altos sin justificación). Si los resultados parecen inconsistentes, revisa si los datos de la tabla estaban correctamente seleccionados al enviar el prompt.

---

### Bloque 4: Evaluación de Tendencias y Reporte Ejecutivo

**Objetivo del bloque:** Utilizar Copilot Chat para generar un reporte de tendencias de mercado relevantes para la categoría analizada, integrando factores macroeconómicos, disrupciones logísticas y señales de riesgo.

---

#### Paso 4.1 — Investigar Tendencias de Mercado Relevantes

**Objetivo:** Construir un prompt avanzado que integre múltiples dimensiones de análisis de tendencias para la categoría de suministro.

**Instrucciones:**

1. En **Copilot Chat**, inicia una nueva conversación.

2. Envía el siguiente prompt de investigación de tendencias:

```
Actúa como un analista de inteligencia de mercado especializado 
en cadenas de suministro industriales. Necesito un análisis de 
tendencias para la categoría de empaques de cartón corrugado 
con horizonte de 12 meses.

Por favor analiza y estructura la información en las siguientes 
dimensiones:

DIMENSIÓN 1 — TENDENCIAS DE MATERIAS PRIMAS:
- Comportamiento esperado del precio de la celulosa y papel kraft
- Impacto de la capacidad instalada global en la oferta

DIMENSIÓN 2 — FACTORES MACROECONÓMICOS:
- Inflación y tipo de cambio en mercados latinoamericanos
- Impacto de tasas de interés en la capacidad de inversión 
  de los proveedores

DIMENSIÓN 3 — DISRUPCIONES LOGÍSTICAS:
- Riesgos en cadenas de suministro globales que afecten 
  la importación de insumos para fabricantes de empaques
- Tendencias en costos de flete marítimo y terrestre

DIMENSIÓN 4 — SEÑALES DE RIESGO PARA COMPRADORES:
- Indicadores de alerta temprana que un comprador debería 
  monitorear
- Escenarios de riesgo (optimista, base, pesimista) para 
  el precio de esta categoría en los próximos 6 meses

Formato: Para cada dimensión, usa un encabezado claro, 
3-4 puntos concisos y una calificación de impacto 
(Alto / Medio / Bajo) para el comprador.
```

3. Lee la respuesta completa. Identifica al menos **dos tendencias** que consideres más relevantes para tu contexto organizacional y márcalas o anótalas.

4. Envía un prompt de seguimiento para profundizar en una tendencia específica:

```
De las tendencias que identificaste, profundiza en el impacto 
de [selecciona la tendencia más relevante de la respuesta 
anterior]. Específicamente:
- ¿Cómo debería reaccionar un departamento de compras ante 
  esta tendencia?
- ¿Qué cláusulas contractuales podría negociar para 
  protegerse de este riesgo?
- ¿Existe algún indicador público que pueda monitorear 
  mensualmente para anticipar cambios?
```

> 📝 **Nota:** Reemplaza el corchete con la tendencia específica que identificaste (por ejemplo: "el aumento en costos de flete marítimo" o "la volatilidad en el precio de la celulosa").

**Resultado esperado:**
- Un análisis estructurado en cuatro dimensiones con calificaciones de impacto
- Identificación de al menos 3 señales de alerta temprana para el comprador
- Escenarios de precio (optimista, base, pesimista) para los próximos 6 meses
- Recomendaciones contractuales específicas para mitigar el riesgo identificado

**Verificación:**
> ✅ La respuesta debe ser específica para la categoría de empaques de cartón, no genérica para "cualquier categoría de suministro". Si la respuesta es muy genérica, agrega al inicio de tu próximo prompt: *"Recuerda que el análisis es específico para empaques industriales de cartón corrugado en mercados latinoamericanos"* y repite la solicitud.

---

#### Paso 4.2 — Generar el Reporte Ejecutivo de Tendencias

**Objetivo:** Consolidar todo el análisis del laboratorio en un reporte ejecutivo estructurado listo para compartir con el equipo de compras.

**Instrucciones:**

1. En el mismo hilo de conversación, envía el siguiente prompt final:

```
Con base en todo el análisis de tendencias que hemos 
construido en esta conversación, genera un REPORTE EJECUTIVO 
DE INTELIGENCIA DE MERCADO con la siguiente estructura:

TÍTULO: Reporte de Inteligencia de Mercado — Empaques 
Industriales de Cartón Corrugado — [Mes/Año actual]

SECCIÓN 1: RESUMEN EJECUTIVO (100 palabras máximo)
- Situación actual del mercado en 3 puntos clave

SECCIÓN 2: ANÁLISIS DE TENDENCIAS CRÍTICAS (150 palabras)
- Las 3 tendencias de mayor impacto para el comprador

SECCIÓN 3: MATRIZ DE RIESGOS Y OPORTUNIDADES
- Tabla con 3 riesgos y 3 oportunidades, cada uno con 
  probabilidad (Alta/Media/Baja) e impacto (Alto/Medio/Bajo)

SECCIÓN 4: RECOMENDACIONES PARA EL EQUIPO DE COMPRAS
- 5 acciones concretas priorizadas por urgencia

SECCIÓN 5: INDICADORES A MONITOREAR
- Lista de 4 KPIs o índices de mercado con frecuencia 
  de seguimiento sugerida

El reporte debe tener un tono profesional y estar listo 
para presentarse a un comité de compras.
```

2. Espera la respuesta completa de Copilot.

3. **Copia el reporte completo** y pégalo en un nuevo documento de Microsoft Word.

4. Aplica el siguiente formato básico al documento:
   - Título en Heading 1
   - Secciones en Heading 2
   - Fuente de texto: Calibri 11pt
   - Márgenes: Normal (2.54 cm)

5. En el encabezado del documento, agrega: `CONFIDENCIAL — USO INTERNO — DATOS DE PRÁCTICA`

6. Guarda el documento en OneDrive como `Lab02_Reporte_Tendencias_[TuNombre].docx`.

7. **Reflexión crítica (2 minutos):** Revisa el reporte generado y responde en el mismo documento (al final, en una sección llamada "Notas del Analista"):
   - ¿Qué información del reporte requeriría validación con fuentes externas antes de usarse en una decisión real?
   - ¿Identificas alguna afirmación de Copilot que te genere dudas o que parezca demasiado general?

**Resultado esperado:**
- Un reporte ejecutivo completo con las cinco secciones estructuradas
- La matriz de riesgos y oportunidades en formato de tabla
- 5 recomendaciones priorizadas para el equipo de compras
- El documento guardado en OneDrive con formato profesional
- Una sección de "Notas del Analista" con reflexión crítica

**Verificación:**
> ✅ Abre el archivo guardado y confirma que tiene al menos 4 secciones visibles, la tabla de riesgos/oportunidades está presente y la sección de "Notas del Analista" contiene al menos 2 observaciones críticas escritas por ti (no generadas por Copilot).

---

## 7. Validación y Pruebas Finales

Al completar los cuatro bloques, realiza las siguientes verificaciones de cierre para confirmar que el laboratorio fue completado exitosamente:

### Lista de Verificación Final

| # | Elemento a Verificar | Criterio de Éxito | ¿Completado? |
|---|---------------------|-------------------|-------------|
| 1 | Prompt de investigación de mercado (Bloque 1) | Contiene los 5 componentes del marco (contexto, objetivo, alcance, formato, variables) | ☐ |
| 2 | Resumen ejecutivo de mercado | Guardado en OneDrive como `Lab02_Resumen_Mercado_[TuNombre].docx` con recomendación explícita | ☐ |
| 3 | Análisis de precios en Excel | Columna "Desviación vs Benchmark (%)" creada y gráfica comparativa visible | ☐ |
| 4 | Scorecard de benchmarking | Criterios con pesos que suman 100% en `Lab02_Plantilla_Scorecard.xlsx` | ☐ |
| 5 | Recomendación de proveedor | Proveedor recomendado con justificación guardado en hoja "Recomendación" del scorecard | ☐ |
| 6 | Reporte de tendencias | Guardado en OneDrive como `Lab02_Reporte_Tendencias_[TuNombre].docx` con 5 secciones | ☐ |
| 7 | Reflexión crítica | Sección "Notas del Analista" con al menos 2 observaciones propias en el reporte | ☐ |
| 8 | Iteración de prompts | Se realizaron al menos 2 prompts de seguimiento (iteración) en Copilot Chat | ☐ |

### Prueba de Calidad de Prompts

Para validar el aprendizaje en ingeniería de prompts, responde mentalmente (o por escrito) las siguientes preguntas:

1. **¿Cuáles son los cinco componentes de un prompt efectivo para análisis de mercado?**
   - Respuesta esperada: Contexto, Objetivo, Alcance temporal, Formato de salida, Variables de interés.

2. **¿Cuáles son las tres etapas del flujo de trabajo con Copilot para investigación de mercado?**
   - Respuesta esperada: Contextualizar → Profundizar/Iterar → Generar entregable.

3. **¿Por qué Copilot NO puede reemplazar completamente las fuentes de datos externas verificables?**
   - Respuesta esperada: Porque Copilot no tiene acceso a datos en tiempo real por sí solo; su valor está en estructurar, sintetizar e interpretar la información que le proporcionas, no en generarla desde cero con precisión factual garantizada.

---

## 8. Resolución de Problemas

### Problema 1: El botón Copilot no aparece en la cinta de opciones de Excel

**Síntoma:** Al abrir `Lab02_Datos_Precios_Historicos.xlsx`, el botón "Copilot" no está visible en la pestaña Inicio de Excel, o aparece en gris (deshabilitado).

**Causa probable:** El archivo está guardado en el disco local (no en OneDrive for Business), la licencia de Microsoft 365 Copilot no está activa para el usuario, o Excel no está actualizado a la versión 2406 o posterior.

**Solución paso a paso:**

1. **Verifica la ubicación del archivo:** En la barra de título de Excel, confirma que la ruta muestra `OneDrive —` seguido del nombre de tu organización. Si muestra una ruta local (C:\Users\...), cierra el archivo y ábrelo directamente desde OneDrive.

2. **Verifica la versión de Excel:** Ve a `Archivo → Cuenta → Acerca de Excel`. Confirma que la versión es 2406 o posterior. Si no lo es, haz clic en `Opciones de actualización → Actualizar ahora`.

3. **Verifica la licencia Copilot:** Ve a `https://portal.office.com` → haz clic en tu avatar → "Ver cuenta" → "Licencias". Confirma que aparece "Microsoft 365 Copilot" como licencia activa. Si no aparece, notifica a TI.

4. **Reinicia Excel** después de cualquier actualización y vuelve a abrir el archivo desde OneDrive.

5. Si el problema persiste después de estos pasos, continúa el Bloque 2 usando **Copilot Chat** para el análisis de precios (copia y pega los datos relevantes como texto en el chat) y documenta el incidente para reportarlo al área de TI.

---

### Problema 2: Copilot Chat genera respuestas muy genéricas que no son útiles para el análisis de suministros

**Síntoma:** Al enviar prompts en Copilot Chat, las respuestas son vagas, no mencionan la categoría específica (cartón corrugado), repiten información obvia sin profundidad analítica, o simplemente dicen que no tiene información actualizada sobre precios.

**Causa probable:** El prompt no incluye suficiente contexto específico, se está usando el modo "Personal" en lugar del modo "Trabajo" en Copilot Chat, o la conversación acumuló demasiado contexto anterior que está generando confusión.

**Solución paso a paso:**

1. **Verifica el modo de Copilot:** En la interfaz de Copilot Chat, confirma que el selector muestra **"Trabajo" (Work)**, no "Personal". El modo Trabajo tiene acceso al contexto organizacional y genera respuestas más enfocadas para uso profesional.

2. **Inicia una nueva conversación:** Haz clic en el ícono de nueva conversación (lápiz) para limpiar el contexto acumulado. Conversaciones largas pueden degradar la calidad de las respuestas.

3. **Enriquece el contexto del prompt:** Agrega al inicio de tu prompt una línea de rol explícito:
   ```
   Eres un analista experto en cadenas de suministro industriales 
   con especialización en mercados latinoamericanos. [Continúa 
   con tu prompt original...]
   ```

4. **Sé más específico en las variables:** En lugar de pedir "análisis de precios del cartón", especifica: "análisis de precios del cartón corrugado calibre C (ondulado simple) para uso en empaques secundarios de productos de consumo masivo en México durante 2024-2025".

5. **Acepta la variabilidad como parte del proceso:** Recuerda que Copilot puede generar respuestas diferentes en cada sesión. Si una respuesta no es útil, itera con un prompt de seguimiento que indique qué fue insatisfactorio: *"La respuesta anterior fue demasiado general. Necesito información más específica sobre [aspecto concreto]. Por favor profundiza en ese punto."*

6. Si después de 3 intentos la calidad sigue siendo insatisfactoria, el instructor puede compartir el banco de prompts de referencia del Módulo 2 para usar como base.

---

## 9. Limpieza del Entorno

Al finalizar el laboratorio, realiza los siguientes pasos de cierre para mantener el entorno ordenado:

### Archivos Generados (conservar en OneDrive)

Los siguientes archivos **deben conservarse** en tu carpeta de OneDrive como evidencia del laboratorio completado:

| Archivo | Descripción |
|---------|-------------|
| `Lab02_Resumen_Mercado_[TuNombre].docx` | Resumen ejecutivo de investigación de mercado (Bloque 1) |
| `Lab02_Datos_Precios_Historicos.xlsx` | Archivo con columna de desviación y gráfica comparativa (Bloque 2) |
| `Lab02_Plantilla_Scorecard.xlsx` | Scorecard completado con criterios y recomendación de proveedor (Bloque 3) |
| `Lab02_Reporte_Tendencias_[TuNombre].docx` | Reporte ejecutivo de tendencias con notas críticas (Bloque 4) |

### Cierre de Sesiones

1. **Cierra las conversaciones de Copilot Chat:** No es necesario eliminarlas, pero si tu organización tiene políticas de retención de datos, consulta con TI si debes limpiar el historial.

2. **Guarda y cierra los archivos de Excel:** Confirma que todos los cambios están guardados en OneDrive (el ícono de nube debe mostrar estado sincronizado ✅).

3. **Cierra Microsoft Edge o Chrome** si no los necesitarás en la siguiente sesión.

4. **No compartas los archivos de práctica** fuera del entorno de OneDrive corporativo sin autorización del instructor.

> ⚠️ **Recordatorio final de privacidad:** Si durante el laboratorio ingresaste accidentalmente información real de tu organización en Copilot Chat, notifica a tu responsable de TI o al oficial de privacidad de datos según las políticas internas.

---

## 10. Resumen y Recursos Adicionales

### Resumen del Laboratorio

En este laboratorio aplicaste las competencias fundamentales de la Lección 2.1 en cuatro bloques prácticos interconectados:

| Bloque | Competencia Aplicada | Herramienta Principal |
|--------|---------------------|----------------------|
| **Bloque 1** | Construcción de prompts con 5 componentes + flujo de 3 etapas para investigación de mercado | Copilot Chat |
| **Bloque 2** | Análisis exploratorio de datos históricos de precios e identificación de desviaciones vs. benchmark | Copilot en Excel |
| **Bloque 3** | Diseño de scorecard de benchmarking y generación de recomendaciones de selección de proveedor | Copilot Chat + Excel |
| **Bloque 4** | Evaluación multidimensional de tendencias de mercado y generación de reporte ejecutivo | Copilot Chat |

### Conceptos Clave Reforzados

- **Los cinco componentes del prompt efectivo** (Contexto, Objetivo, Alcance temporal, Formato de salida, Variables de interés) son la base para obtener análisis de mercado accionables con Copilot.
- **Copilot es un acelerador, no un oráculo:** sus respuestas requieren validación crítica y contraste con fuentes externas verificables antes de usarse en decisiones de alto impacto.
- **La iteración es parte del proceso:** los mejores análisis se construyen en múltiples turnos de conversación, no en un único prompt perfecto.
- **El benchmarking de proveedores** se vuelve más objetivo y reproducible cuando se definen criterios ponderados explícitos antes de evaluar a los proveedores.
- **La reflexión crítica** sobre las respuestas de Copilot (identificar qué requiere validación) es una competencia profesional tan importante como construir buenos prompts.

### Preparación para el Siguiente Módulo

En el **Módulo 3** aplicarás estas habilidades para generar, revisar y mejorar documentos clave de suministros (órdenes de compra, solicitudes de cotización, contratos de servicio) utilizando Copilot en Word y Outlook. Se recomienda que antes de esa sesión:

- Revises los documentos estándar de suministros que utiliza tu organización (RFQ, RFI, PO, acuerdos de nivel de servicio).
- Practiques la construcción de prompts con el banco de referencia compartido por el instructor.
- Guardes los archivos de este laboratorio como referencia de contexto para los ejercicios del Módulo 3.

### Recursos de Referencia

| Recurso | Descripción | URL |
|---------|-------------|-----|
| Documentación oficial de Microsoft Copilot | Guías técnicas y mejores prácticas | [learn.microsoft.com/es-es/copilot](https://learn.microsoft.com/es-es/copilot/) |
| Guía de ingeniería de prompts — Microsoft Azure | Marco para construir prompts efectivos con IA generativa | [learn.microsoft.com — Prompt Engineering](https://learn.microsoft.com/es-es/azure/ai-services/openai/concepts/prompt-engineering) |
| Índice de precios de materias primas — Banco Mundial | Datos de referencia para benchmarking de precios de insumos | [worldbank.org/commodity-markets](https://www.worldbank.org/en/research/commodity-markets) |
| ISM Report on Business | Índice mensual de condiciones de suministro en manufactura y servicios | [ismworld.org](https://www.ismworld.org/supply-management-news-and-reports/reports/ism-report-on-business/) |
| Gartner Supply Chain Insights | Tendencias globales en cadena de suministro | [gartner.com/supply-chain](https://www.gartner.com/en/supply-chain) |

---

> 📋 **Nota para el instructor:** Al finalizar el laboratorio, solicita a los participantes que compartan en 2 minutos (ronda rápida) una respuesta de Copilot que consideraron especialmente útil y una que requirió ajuste o validación. Esta reflexión grupal refuerza el pensamiento crítico y la comprensión de las limitaciones de la IA generativa en contextos profesionales de suministros.

---
*Lab 02-00-01 — Versión 1.0 — Curso: Microsoft 365 Copilot para Profesionales de Suministros*

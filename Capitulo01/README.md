# Uso de Copilot para acelerar el análisis de información extraída de Excel, Power BI y sistemas ERP, identificando patrones, riesgos, anomalías y acciones prioritarias.

---

## 1. Metadatos del Laboratorio

| Atributo | Detalle |
|---|---|
| **ID del Laboratorio** | 01-00-01 |
| **Duración estimada** | 72 minutos |
| **Complejidad** | Media |
| **Nivel de Bloom** | Aplicar (*Apply*) |
| **Módulo** | Módulo 1 — Análisis de Información con Copilot |
| **Lección asociada** | Lección 1.1: Análisis de Información de Excel, Power BI y Sistemas ERP con Copilot |
| **Modalidad** | Individual (con orientación del instructor) |

---

## 2. Descripción General

En este laboratorio aplicarás Microsoft 365 Copilot como herramienta de análisis de datos operativos de cadena de suministro, trabajando con tres fuentes de información: una hoja de Excel con registros de órdenes de compra e inventarios, un dashboard de Power BI con métricas de desempeño de proveedores, y un archivo CSV que simula una exportación de sistema ERP. A través de tres bloques de trabajo progresivos, formularás prompts en lenguaje natural para que Copilot genere resúmenes, detecte anomalías, interprete visualizaciones y produzca una lista de acciones prioritarias para el equipo de Suministros. El laboratorio refuerza el concepto central de la Lección 1.1: Copilot actúa como una capa de inteligencia que reduce drásticamente el tiempo entre la pregunta y el insight operativo.

---

## 3. Objetivos de Aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] **Utilizar** Microsoft 365 Copilot en Excel para analizar tablas de datos de inventario, órdenes de compra y proveedores, generando resúmenes automáticos e identificando tendencias relevantes para la cadena de suministro.
- [ ] **Aplicar** Copilot en Power BI para interpretar dashboards de suministros y extraer conclusiones sobre el desempeño de proveedores, niveles de stock y cumplimiento de entregas.
- [ ] **Emplear** Copilot Chat para simular la interpretación de datos exportados de sistemas ERP, identificando patrones de consumo, riesgos de desabasto y anomalías operativas.
- [ ] **Generar** mediante Copilot una lista de acciones prioritarias basada en los hallazgos del análisis de datos, con recomendaciones concretas para el equipo de Suministros.

---

## 4. Prerrequisitos

### Conocimientos Previos

| Área | Nivel requerido |
|---|---|
| Microsoft Excel (tablas, filtros, fórmulas básicas) | Básico |
| Power BI Desktop (apertura de archivos `.pbix`, navegación de reportes) | Básico |
| Conceptos de cadena de suministro (OC, inventario, proveedores) | Básico |
| Introducción conceptual del Módulo 1 sobre análisis con Copilot | Completado |

### Acceso y Licenciamiento

| Requisito | Estado esperado |
|---|---|
| Cuenta corporativa Microsoft 365 activa | ✅ Verificado por TI |
| Licencia **Microsoft 365 Copilot** habilitada | ✅ Confirmada antes del curso |
| Archivos de práctica del Módulo 1 descargados | ✅ Guardados en OneDrive for Business |
| Acceso a Power BI Desktop (versión julio 2024 o posterior) | ✅ Instalado en equipo |
| Conexión a internet estable (mínimo 10 Mbps) | ✅ Verificada |

> ⚠️ **IMPORTANTE — Privacidad de datos:** Durante todo el laboratorio trabajarás exclusivamente con los archivos de práctica proporcionados. **No ingreses datos reales de proveedores, precios contractuales ni información financiera sensible de tu organización en Copilot.**

---

## 5. Entorno del Laboratorio

### Hardware Recomendado

| Componente | Mínimo | Recomendado |
|---|---|---|
| Procesador | Intel Core i5 8va gen / AMD Ryzen 5 | Intel Core i7 / AMD Ryzen 7 |
| RAM | 8 GB | 16 GB |
| Almacenamiento libre | 10 GB | 15 GB |
| Resolución de pantalla | 1366×768 | 1920×1080 |
| Conexión a internet | 10 Mbps | 25 Mbps o superior |

### Software Requerido

| Aplicación | Versión mínima |
|---|---|
| Microsoft Excel (Microsoft 365 Apps) | 2406 o posterior |
| Microsoft Power BI Desktop | Julio 2024 o posterior |
| Microsoft Edge o Google Chrome | Versión 120 o posterior |
| Microsoft Copilot Chat | Acceso vía `copilot.microsoft.com` o Microsoft Teams |
| OneDrive for Business | Versión en la nube (siempre actualizada) |

### Archivos de Práctica del Laboratorio

El instructor habrá compartido los siguientes archivos en la carpeta de OneDrive del curso. Verifica que los tienes disponibles antes de comenzar:

| Archivo | Descripción | Formato |
|---|---|---|
| `Lab01_OrdenesDe Compra_Inventario.xlsx` | Tabla con 150+ registros de OC, inventario y evaluación de proveedores | Excel (.xlsx) |
| `Lab01_Dashboard_Suministros.pbix` | Dashboard de Power BI con KPIs de cadena de suministro | Power BI (.pbix) |
| `Lab01_Exportacion_ERP.csv` | Datos simulados de exportación de sistema ERP (movimientos de almacén) | CSV |

### Configuración Inicial del Entorno

Realiza los siguientes pasos de configuración **antes** de iniciar los bloques de trabajo:

**Paso de configuración 1 — Verificar ubicación de archivos en OneDrive:**

1. Abre el explorador de archivos y navega a tu carpeta de OneDrive for Business.
2. Confirma que la carpeta `Curso_Copilot_Suministros > Modulo1` contiene los tres archivos listados arriba.
3. Si los archivos están en el escritorio o en disco local (`C:\`), cópialos a OneDrive **ahora** antes de continuar. Copilot en Excel **no funcionará** con archivos locales.

**Paso de configuración 2 — Verificar que Copilot está activo en Excel:**

1. Abre `Lab01_OrdenesDe Compra_Inventario.xlsx` desde OneDrive (doble clic desde el explorador de archivos o desde `onedrive.com`).
2. En la cinta de opciones (*ribbon*) de Excel, busca la pestaña **Inicio** y localiza el botón **Copilot** (ícono de constelación de puntos) en el extremo derecho.
3. Si el botón no aparece, verifica con el instructor que la licencia esté activa.

**Paso de configuración 3 — Verificar acceso a Copilot Chat:**

1. Abre Microsoft Edge o Chrome.
2. Navega a `https://copilot.microsoft.com`.
3. Inicia sesión con tu cuenta corporativa Microsoft 365.
4. Confirma que aparece la interfaz de chat y que en la parte superior indica tu nombre de usuario corporativo (no una cuenta personal).

---

## 6. Instrucciones Paso a Paso

El laboratorio está organizado en **tres bloques de trabajo** más un bloque final de síntesis:

| Bloque | Herramienta | Tiempo estimado |
|---|---|---|
| **Bloque A** | Análisis en Excel con Copilot | 25 minutos |
| **Bloque B** | Interpretación de dashboard en Power BI con Copilot | 20 minutos |
| **Bloque C** | Análisis de datos ERP con Copilot Chat | 15 minutos |
| **Bloque D** | Generación de plan de acción priorizado | 12 minutos |

---

### Bloque A — Análisis de Datos de Órdenes de Compra e Inventario en Excel con Copilot

**Objetivo del bloque:** Utilizar Copilot en Excel para obtener un resumen automático de los datos de órdenes de compra, detectar variaciones de precio significativas e identificar proveedores con comportamiento atípico.

---

#### Paso A1 — Explorar la estructura del archivo y activar Copilot

**Objetivo:** Familiarizarte con los datos del archivo de práctica y abrir el panel de Copilot en Excel.

**Instrucciones:**

1. Asegúrate de que el archivo `Lab01_OrdenesDe Compra_Inventario.xlsx` esté abierto desde OneDrive (la barra de título debe mostrar el ícono de nube ☁️ junto al nombre del archivo).
2. Observa las hojas del libro. Encontrarás tres pestañas:
   - **`OC_Trimestre`** — Órdenes de compra del trimestre (columnas: `ID_OC`, `Proveedor`, `Categoría`, `Producto`, `Cantidad`, `Precio_Contrato`, `Precio_Real`, `Fecha_OC`, `Estado`).
   - **`Inventario_Actual`** — Niveles de stock por producto (columnas: `Código_Producto`, `Descripción`, `Stock_Actual`, `Stock_Mínimo`, `Días_Cobertura`, `Proveedor_Principal`).
   - **`Evaluacion_Proveedores`** — Calificaciones de proveedores (columnas: `Proveedor`, `Puntaje_Calidad`, `Puntaje_Entrega`, `Puntaje_Precio`, `Incidencias_Trimestre`).
3. Haz clic en la pestaña **`OC_Trimestre`**.
4. Haz clic en cualquier celda dentro de la tabla de datos.
5. En la cinta de opciones, haz clic en **Inicio** y luego en el botón **Copilot** (extremo derecho del ribbon). El panel de Copilot se abrirá en el lado derecho de la pantalla.

**Resultado esperado:** El panel de Copilot se abre y muestra un mensaje de bienvenida con sugerencias de prompts iniciales relacionadas con los datos de la hoja activa.

**Verificación:** El panel de Copilot debe mostrar el texto "¿Cómo puedo ayudarte con estos datos?" o similar, y debe reconocer que hay una tabla activa en la hoja.

---

#### Paso A2 — Generar un resumen automático de las órdenes de compra

**Objetivo:** Obtener un resumen ejecutivo de los datos de órdenes de compra sin construir fórmulas manualmente.

**Instrucciones:**

1. En el panel de Copilot, escribe el siguiente prompt y presiona **Enter** o haz clic en el botón de enviar:

   ```
   Resume los datos de esta tabla. Indica el número total de órdenes de compra, 
   el monto total comprometido (suma de Precio_Real × Cantidad), las 3 categorías 
   con mayor gasto y los 3 proveedores con mayor número de órdenes.
   ```

2. Espera a que Copilot genere la respuesta (puede tomar entre 10 y 30 segundos).
3. Lee cuidadosamente la respuesta. Identifica si Copilot:
   - Calculó correctamente el número total de órdenes.
   - Presentó las categorías y proveedores en orden descendente.
   - Usó los nombres de columna correctos.
4. Si algún dato parece incorrecto, verifica manualmente en la tabla usando un filtro o una suma rápida con `=SUMA()`.
5. Copia la respuesta de Copilot en un documento de Word nuevo que llamarás `Lab01_Hallazgos.docx` (lo usarás a lo largo del laboratorio). Guárdalo en OneDrive.

**Resultado esperado:** Copilot genera un resumen en texto con los valores calculados, similar a:

> *"La tabla contiene 152 órdenes de compra. El monto total comprometido es de $1,284,500 USD. Las categorías con mayor gasto son: Materias Primas ($520,000), Embalaje ($310,000) y Mantenimiento ($180,000). Los proveedores con mayor número de órdenes son: Proveedor A (28 OC), Proveedor C (22 OC) y Proveedor F (19 OC)."*

> 📝 **Nota para el instructor:** Los valores exactos variarán según el archivo de práctica. Lo importante es que el participante evalúe la coherencia de la respuesta, no que coincida con un número específico.

**Verificación:** Compara el número total de órdenes con la cantidad de filas de la tabla (puedes ver esto en la barra de estado inferior de Excel al seleccionar la columna `ID_OC`). La diferencia no debe ser mayor a ±2 filas.

---

#### Paso A3 — Detectar variaciones de precio significativas

**Objetivo:** Identificar órdenes de compra donde el precio real pagado difiere más del 10% respecto al precio contratado, replicando el caso de uso de la Lección 1.1.

**Instrucciones:**

1. En el panel de Copilot, escribe el siguiente prompt:

   ```
   Analiza las columnas Precio_Contrato y Precio_Real. Identifica todas las filas 
   donde la variación porcentual entre ambos precios supere el 10% (en cualquier 
   dirección). Muestra cuántas filas cumplen esta condición, el proveedor con más 
   casos de variación y si las variaciones son predominantemente al alza o a la baja.
   ```

2. Revisa la respuesta de Copilot. Presta atención a:
   - ¿Cuántas órdenes presentan variación superior al 10%?
   - ¿Qué proveedor aparece con mayor frecuencia en esas filas?
   - ¿Las variaciones son mayoritariamente al alza (el proveedor cobró más de lo contratado) o a la baja?
3. Ahora pide a Copilot que genere una fórmula para identificar estas variaciones automáticamente. Escribe:

   ```
   Genera una fórmula de Excel para agregar en una nueva columna llamada 
   "Alerta_Precio" que muestre "⚠️ Variación >10%" si la diferencia porcentual 
   entre Precio_Real y Precio_Contrato supera el 10%, y "OK" en caso contrario.
   ```

4. Copilot generará una fórmula similar a:

   ```excel
   =SI(ABS(([@Precio_Real]-[@Precio_Contrato])/[@Precio_Contrato])>0.1,
      "⚠️ Variación >10%","OK")
   ```

5. Haz clic en la celda vacía en la primera fila de datos de la columna inmediatamente a la derecha de la tabla (o inserta una nueva columna con el encabezado `Alerta_Precio`).
6. Copia y pega la fórmula generada por Copilot en esa celda.
7. Verifica que la fórmula se aplique a todas las filas de la tabla (Excel debería propagarla automáticamente si es una tabla estructurada; si no, arrastra el controlador de relleno hacia abajo).
8. Registra los hallazgos en tu documento `Lab01_Hallazgos.docx`.

**Resultado esperado:** La columna `Alerta_Precio` muestra "⚠️ Variación >10%" en las filas problemáticas y "OK" en las demás. Copilot también habrá proporcionado el conteo de filas con variación y el proveedor más frecuente en esos casos.

**Verificación:** Aplica un filtro en la columna `Alerta_Precio` para mostrar solo las filas con "⚠️ Variación >10%". Verifica manualmente 3 filas al azar calculando `=ABS((Precio_Real - Precio_Contrato)/Precio_Contrato)` para confirmar que el resultado supera 0.10.

---

#### Paso A4 — Identificar productos en riesgo de desabasto

**Objetivo:** Analizar la hoja de inventario para detectar productos con cobertura crítica.

**Instrucciones:**

1. Haz clic en la pestaña **`Inventario_Actual`**.
2. Haz clic en cualquier celda dentro de la tabla de inventario.
3. En el panel de Copilot (que debe seguir abierto), escribe:

   ```
   Analiza esta tabla de inventario. Identifica todos los productos donde 
   Días_Cobertura sea menor a 15 días o donde Stock_Actual sea inferior al 
   Stock_Mínimo. Ordénalos de mayor a menor urgencia y señala el proveedor 
   principal de cada uno.
   ```

4. Revisa la lista generada por Copilot. Verifica que los productos listados efectivamente tienen `Días_Cobertura < 15` o `Stock_Actual < Stock_Mínimo`.
5. Solicita a Copilot un análisis adicional:

   ```
   ¿Existe algún proveedor que concentre varios de los productos en riesgo 
   de desabasto? ¿Qué implicación operativa tendría si ese proveedor 
   tuviera un problema de entrega?
   ```

6. Copia los hallazgos más relevantes en `Lab01_Hallazgos.docx` bajo el título **"Riesgos de Inventario Identificados"**.

**Resultado esperado:** Copilot genera una lista ordenada de productos en riesgo con su proveedor principal, y proporciona una interpretación sobre la concentración de riesgo en proveedores específicos.

**Verificación:** Aplica un filtro en la columna `Días_Cobertura` para mostrar valores menores a 15. Confirma que los productos listados por Copilot coinciden con los resultados del filtro.

---

### Bloque B — Interpretación del Dashboard de Power BI con Copilot

**Objetivo del bloque:** Utilizar las capacidades de Copilot en Power BI para interpretar visualizaciones del dashboard de suministros, generar narrativas automáticas y extraer conclusiones sobre el desempeño de proveedores y cumplimiento de entregas.

---

#### Paso B1 — Abrir el dashboard y explorar su estructura

**Objetivo:** Familiarizarte con el reporte de Power BI y localizar las funciones de Copilot disponibles.

**Instrucciones:**

1. Abre **Power BI Desktop** desde el menú de inicio de Windows.
2. Haz clic en **Archivo > Abrir** y navega a tu carpeta de OneDrive donde está guardado `Lab01_Dashboard_Suministros.pbix`.
3. Espera a que el archivo cargue completamente (puede tomar 30-60 segundos).
4. Explora las páginas del reporte. El dashboard contiene las siguientes páginas:
   - **`Resumen Ejecutivo`** — KPIs principales: Tasa de cumplimiento de entregas, Costo total de compras, Número de OC abiertas, Variación de precio promedio.
   - **`Desempeño de Proveedores`** — Gráfico de barras con puntaje por proveedor, mapa de calor de incidencias, tabla de detalle.
   - **`Niveles de Stock`** — Gráfico de líneas de evolución de inventario, semáforo de cobertura por categoría.
   - **`Cumplimiento de Entregas`** — Gráfico de tendencia mensual, análisis por proveedor y categoría.
5. Dedica 3-4 minutos a navegar por cada página para familiarizarte con los datos antes de usar Copilot.

> ⚠️ **Nota sobre Copilot en Power BI Desktop vs. Power BI Service:** Las funcionalidades de Copilot son más completas en **Power BI Service** (web). Si tu versión de Power BI Desktop no muestra el panel de Copilot, el instructor indicará cómo publicar el reporte en Power BI Service para continuar. En ese caso, sigue las instrucciones del Paso B1-alternativo a continuación.

**Paso B1-alternativo (si Copilot no aparece en Power BI Desktop):**

1. En Power BI Desktop, haz clic en **Inicio > Publicar**.
2. Selecciona tu área de trabajo personal en Power BI Service.
3. Una vez publicado, abre `https://app.powerbi.com` en el navegador.
4. Navega a **Mi área de trabajo** y abre el reporte `Lab01_Dashboard_Suministros`.

**Resultado esperado:** El reporte está abierto y puedes navegar entre sus cuatro páginas sin errores. Si usas Power BI Service, el panel de Copilot es accesible desde el botón **Copilot** en la barra de herramientas superior.

**Verificación:** Confirma que puedes ver al menos 3 visualizaciones en la página `Resumen Ejecutivo` y que los datos se muestran correctamente (no hay mensajes de error de fuente de datos).

---

#### Paso B2 — Generar una narrativa automática del resumen ejecutivo

**Objetivo:** Usar Copilot para convertir las visualizaciones del dashboard en texto interpretativo listo para un reporte ejecutivo.

**Instrucciones:**

1. Navega a la página **`Resumen Ejecutivo`** del reporte.
2. Abre el panel de Copilot (botón **Copilot** en la barra superior o en el panel derecho).
3. Escribe el siguiente prompt:

   ```
   Genera un resumen ejecutivo en español de los KPIs mostrados en esta página. 
   Incluye: la tasa de cumplimiento de entregas actual y si está por encima o 
   debajo del objetivo, el costo total de compras del período, la variación de 
   precio promedio y cualquier indicador que muestre una tendencia preocupante.
   Redacta el resumen en un párrafo de máximo 150 palabras, adecuado para 
   presentar a un director de operaciones.
   ```

4. Lee la narrativa generada. Evalúa:
   - ¿Refleja con precisión los valores mostrados en el dashboard?
   - ¿El tono es apropiado para un reporte ejecutivo?
   - ¿Identifica correctamente las tendencias positivas y negativas?
5. Si necesitas ajustar el tono o el nivel de detalle, usa un prompt de refinamiento:

   ```
   Ajusta el resumen anterior para que sea más conciso. Elimina los adjetivos 
   genéricos y enfócate en los números concretos y las acciones que se 
   desprenden de ellos.
   ```

6. Copia la versión final de la narrativa en `Lab01_Hallazgos.docx` bajo el título **"Narrativa Ejecutiva — Dashboard de Suministros"**.

**Resultado esperado:** Copilot genera un párrafo coherente que describe los KPIs del dashboard con valores específicos extraídos de las visualizaciones, en tono ejecutivo y sin necesidad de edición mayor.

**Verificación:** Compara manualmente al menos 2 valores mencionados en la narrativa con los que se muestran en las tarjetas KPI del dashboard. La variación aceptable es ±5% (puede haber diferencias de redondeo).

---

#### Paso B3 — Analizar el desempeño de proveedores con Copilot

**Objetivo:** Extraer conclusiones sobre los proveedores con mejor y peor desempeño usando Copilot como intérprete del dashboard.

**Instrucciones:**

1. Navega a la página **`Desempeño de Proveedores`**.
2. En el panel de Copilot, escribe:

   ```
   Basándote en las visualizaciones de esta página, identifica:
   1. Los 2 proveedores con mejor desempeño general (considerando calidad, 
      entrega y precio).
   2. Los 2 proveedores con peor desempeño o mayor número de incidencias.
   3. ¿Existe algún proveedor que tenga buen puntaje en calidad pero bajo 
      puntaje en entregas? ¿Qué podría indicar esto operativamente?
   ```

3. Revisa la respuesta. Presta atención especial a la interpretación operativa del punto 3, ya que refleja la capacidad de Copilot para ir más allá de los datos y ofrecer contexto.
4. Formula un prompt de seguimiento para profundizar:

   ```
   Para el proveedor con mayor número de incidencias, ¿qué categorías de 
   productos están siendo más afectadas según el mapa de calor? ¿Qué 
   recomendación darías para gestionar este riesgo?
   ```

5. Registra los hallazgos en `Lab01_Hallazgos.docx` bajo el título **"Análisis de Desempeño de Proveedores"**.

**Resultado esperado:** Copilot identifica correctamente los proveedores destacados y los problemáticos, y ofrece una interpretación operativa que va más allá de simplemente leer los números del gráfico.

**Verificación:** Navega manualmente por el gráfico de barras de puntaje de proveedores. Confirma que los proveedores identificados por Copilot como "mejor desempeño" efectivamente tienen las barras más altas en el visual.

---

#### Paso B4 — Interpretar la tendencia de cumplimiento de entregas

**Objetivo:** Usar Copilot para identificar patrones temporales en el cumplimiento de entregas.

**Instrucciones:**

1. Navega a la página **`Cumplimiento de Entregas`**.
2. En el panel de Copilot, escribe:

   ```
   Analiza la tendencia de cumplimiento de entregas mostrada en el gráfico 
   de líneas. ¿En qué meses se observan las caídas más significativas? 
   ¿Hay algún patrón estacional? ¿Qué proveedores o categorías concentran 
   los incumplimientos según los filtros disponibles?
   ```

3. Revisa la respuesta y toma nota de los meses o períodos identificados como críticos.
4. Registra los hallazgos en `Lab01_Hallazgos.docx` bajo el título **"Tendencia de Cumplimiento de Entregas"**.

**Resultado esperado:** Copilot identifica los períodos con menor cumplimiento, señala si existe un patrón (por ejemplo, caídas en meses de alta demanda) y menciona los proveedores o categorías más afectados.

**Verificación:** Observa visualmente el gráfico de líneas y confirma que los meses mencionados por Copilot corresponden a los puntos más bajos de la curva.

---

### Bloque C — Análisis de Datos ERP con Copilot Chat

**Objetivo del bloque:** Simular el análisis de datos exportados de un sistema ERP usando Copilot Chat, identificando patrones de consumo, riesgos de desabasto y anomalías operativas en los datos de movimientos de almacén.

---

#### Paso C1 — Preparar los datos del ERP para análisis con Copilot Chat

**Objetivo:** Importar el archivo CSV de exportación ERP a Excel y prepararlo para su análisis mediante Copilot Chat.

**Instrucciones:**

1. Abre **Microsoft Excel** y crea un nuevo libro en blanco.
2. Ve a **Datos > Obtener datos > Desde archivo > Desde texto/CSV**.
3. Navega a tu carpeta de OneDrive y selecciona `Lab01_Exportacion_ERP.csv`.
4. En el asistente de importación:
   - Confirma que el delimitador es **coma (,)**.
   - Verifica que las columnas se detectan correctamente: `Fecha_Movimiento`, `Código_Material`, `Descripción_Material`, `Tipo_Movimiento`, `Cantidad`, `Almacén`, `Centro_Costo`, `Proveedor`.
   - Haz clic en **Cargar**.
5. Una vez importados los datos, convierte el rango a tabla: selecciona cualquier celda de los datos y presiona **Ctrl + T**. Acepta el rango sugerido y confirma que "La tabla tiene encabezados" está marcado.
6. Nombra la tabla: en la pestaña **Diseño de tabla**, cambia el nombre a `Movimientos_ERP`.
7. Guarda el archivo como `Lab01_Analisis_ERP.xlsx` en tu carpeta de OneDrive.

**Resultado esperado:** El archivo CSV está importado como tabla estructurada en Excel, guardado en OneDrive con el nombre `Lab01_Analisis_ERP.xlsx`.

**Verificación:** La tabla `Movimientos_ERP` debe mostrar datos en todas las columnas sin celdas vacías en los encabezados. La barra de estado inferior debe indicar el número de registros importados.

---

#### Paso C2 — Usar Copilot Chat para analizar patrones de consumo del ERP

**Objetivo:** Emplear Copilot Chat (vía web o Teams) para interpretar los datos de movimientos de almacén y detectar patrones de consumo relevantes.

> 📝 **Nota:** Copilot Chat puede analizar datos que pegues directamente en el chat o que compartas como archivo adjunto. En este paso usaremos la función de adjuntar archivo en Copilot Chat.

**Instrucciones:**

1. Abre tu navegador y ve a `https://copilot.microsoft.com`. Inicia sesión con tu cuenta corporativa.
2. Asegúrate de que Copilot Chat está en modo **Trabajo** (no Personal). Busca el selector de modo en la parte superior de la interfaz; debe indicar "Trabajo" o mostrar el ícono de tu organización.
3. Haz clic en el ícono de **adjuntar archivo** (clip 📎) en la barra de entrada del chat.
4. Selecciona el archivo `Lab01_Analisis_ERP.xlsx` desde OneDrive.
5. Una vez adjunto el archivo, escribe el siguiente prompt:

   ```
   Este archivo contiene movimientos de almacén exportados de un sistema ERP 
   de una empresa manufacturera. Analiza los datos y responde:
   1. ¿Cuáles son los 5 materiales con mayor volumen de salidas del almacén 
      en el período?
   2. ¿Existe algún material que muestre un patrón de consumo irregular 
      (picos o caídas abruptas)?
   3. ¿Hay algún material con entradas de proveedor muy bajas en comparación 
      con sus salidas? Esto podría indicar riesgo de desabasto.
   ```

6. Revisa la respuesta de Copilot. Evalúa la coherencia del análisis con lo que puedes observar directamente en la tabla de Excel.
7. Registra los hallazgos en `Lab01_Hallazgos.docx` bajo el título **"Patrones de Consumo — Datos ERP"**.

**Resultado esperado:** Copilot Chat identifica los materiales de mayor movimiento, señala al menos un material con patrón irregular y detecta posibles riesgos de desabasto basándose en la relación entradas/salidas.

**Verificación:** En Excel, aplica un filtro en la columna `Tipo_Movimiento` para separar entradas (ej.: "Recepción de OC") de salidas (ej.: "Consumo a producción"). Compara el top 5 de materiales con mayor volumen de salidas con lo que Copilot identificó.

---

#### Paso C3 — Detectar anomalías operativas en los datos ERP

**Objetivo:** Usar Copilot Chat para identificar irregularidades en los datos de movimientos que podrían indicar errores de registro o problemas operativos.

**Instrucciones:**

1. En la misma sesión de Copilot Chat (con el archivo aún disponible en el contexto), escribe:

   ```
   Analiza los datos en busca de anomalías operativas. Específicamente:
   1. ¿Existen movimientos con cantidades negativas o valores fuera del 
      rango normal para su tipo de material?
   2. ¿Hay fechas de movimiento que parezcan incorrectas (fechas futuras, 
      fechas muy antiguas o concentración inusual de movimientos en un 
      solo día)?
   3. ¿Algún código de material aparece con descripciones inconsistentes 
      (el mismo código con nombres diferentes)?
   Indica el nivel de confianza de cada hallazgo y si podría ser un error 
   de datos o un evento operativo legítimo.
   ```

2. Revisa cada anomalía identificada. Para cada una, pregúntate:
   - ¿Es plausible como evento operativo real?
   - ¿Requiere verificación con el equipo de almacén o el administrador del ERP?
3. Solicita a Copilot una recomendación de acción para las anomalías más críticas:

   ```
   Para las 2 anomalías más críticas que identificaste, ¿qué acción 
   correctiva recomendarías y con qué área funcional debería coordinarse 
   el equipo de Suministros para resolverlas?
   ```

4. Registra los hallazgos y recomendaciones en `Lab01_Hallazgos.docx` bajo el título **"Anomalías Detectadas en Datos ERP"**.

**Resultado esperado:** Copilot identifica al menos 2-3 anomalías en los datos (el archivo de práctica incluye anomalías plantadas intencionalmente) y proporciona recomendaciones de acción concretas con indicación del área responsable.

**Verificación:** Revisa manualmente en Excel la columna `Cantidad` usando la función `=MIN(Movimientos_ERP[Cantidad])` para confirmar si existen valores negativos. Verifica también la columna `Fecha_Movimiento` con `=MAX(Movimientos_ERP[Fecha_Movimiento])` para detectar fechas futuras.

---

### Bloque D — Generación del Plan de Acción Priorizado

**Objetivo del bloque:** Consolidar todos los hallazgos de los bloques anteriores y usar Copilot Chat para generar una lista de acciones prioritarias con recomendaciones concretas para el equipo de Suministros.

---

#### Paso D1 — Consolidar hallazgos y generar el plan de acción

**Objetivo:** Usar Copilot Chat para sintetizar todos los análisis realizados y producir un plan de acción estructurado y priorizado.

**Instrucciones:**

1. Abre `Lab01_Hallazgos.docx` y revisa brevemente todos los hallazgos registrados en los bloques anteriores. Asegúrate de tener anotaciones en las cuatro secciones:
   - Resumen de órdenes de compra
   - Riesgos de inventario
   - Análisis de desempeño de proveedores
   - Patrones de consumo y anomalías ERP
2. En Copilot Chat, escribe el siguiente prompt consolidador. Adapta los hallazgos específicos con los valores que obtuviste en tu análisis:

   ```
   Soy analista de Suministros de una empresa manufacturera. Durante el día 
   de hoy analicé los siguientes hallazgos en nuestra cadena de suministro:

   HALLAZGOS DE EXCEL (Órdenes de Compra):
   - [X] órdenes de compra presentan variación de precio superior al 10% 
     respecto al contrato, concentradas en [Proveedor X].
   - [Y] productos tienen cobertura de inventario menor a 15 días, siendo 
     los más críticos [Producto A] y [Producto B].

   HALLAZGOS DE POWER BI (Dashboard):
   - La tasa de cumplimiento de entregas está por debajo del objetivo en 
     los últimos [N] meses.
   - [Proveedor Z] tiene el mayor número de incidencias del trimestre.
   - Se observa una caída en cumplimiento de entregas en [mes/período].

   HALLAZGOS DE DATOS ERP:
   - [Material X] muestra riesgo de desabasto por baja relación entradas/salidas.
   - Se detectaron [N] anomalías en los registros de movimientos de almacén.

   Con base en estos hallazgos, genera un Plan de Acción Priorizado con 
   máximo 8 acciones, ordenadas de mayor a menor urgencia. Para cada acción 
   indica: descripción de la acción, área responsable, plazo sugerido 
   (inmediato/1 semana/1 mes) y el hallazgo que la origina.
   Presenta el resultado en formato de tabla.
   ```

   > 📝 **Instrucción para el participante:** Reemplaza los valores entre corchetes `[...]` con los hallazgos reales que obtuviste en los bloques anteriores. Esta personalización es parte fundamental del ejercicio.

3. Revisa la tabla de acciones generada por Copilot. Evalúa:
   - ¿Las acciones son concretas y ejecutables?
   - ¿La priorización es lógica dado el contexto de suministros?
   - ¿Las áreas responsables asignadas son correctas?
4. Si alguna acción es demasiado genérica, usa un prompt de refinamiento:

   ```
   La acción número [N] es demasiado general. Reformúlala de manera más 
   específica para el contexto de compras industriales, indicando qué 
   información debe recopilarse y con quién debe coordinarse el comprador.
   ```

5. Copia la tabla final del plan de acción en `Lab01_Hallazgos.docx` bajo el título **"Plan de Acción Priorizado — Análisis de Cadena de Suministro"**.

**Resultado esperado:** Copilot genera una tabla con 6-8 acciones priorizadas, cada una con descripción, área responsable, plazo y origen del hallazgo. Las acciones reflejan los datos específicos que el participante ingresó en el prompt.

**Verificación:** Revisa que al menos 3 de las acciones generadas por Copilot tienen una relación directa y verificable con los hallazgos que registraste en los bloques anteriores. Si Copilot generó acciones que no se derivan de los datos analizados, señálalas como "no fundamentadas en datos" en tu documento.

---

#### Paso D2 — Guardar y organizar el documento de hallazgos final

**Objetivo:** Asegurarte de que el documento de hallazgos esté completo, bien estructurado y guardado correctamente en OneDrive.

**Instrucciones:**

1. Abre `Lab01_Hallazgos.docx` y verifica que contiene las siguientes secciones con contenido:
   - [ ] Resumen Ejecutivo de Órdenes de Compra (Bloque A)
   - [ ] Riesgos de Inventario Identificados (Bloque A)
   - [ ] Narrativa Ejecutiva — Dashboard de Suministros (Bloque B)
   - [ ] Análisis de Desempeño de Proveedores (Bloque B)
   - [ ] Tendencia de Cumplimiento de Entregas (Bloque B)
   - [ ] Patrones de Consumo — Datos ERP (Bloque C)
   - [ ] Anomalías Detectadas en Datos ERP (Bloque C)
   - [ ] Plan de Acción Priorizado (Bloque D)
2. Agrega en la primera página del documento un encabezado con:
   - Tu nombre
   - Fecha de realización del laboratorio
   - Nombre del laboratorio: "Lab 01-00-01"
3. Guarda el documento (`Ctrl + S`). Confirma que se guarda en OneDrive (el ícono de nube debe aparecer junto al nombre del archivo).
4. Comparte el documento con el instructor usando la opción **Compartir** de Word, seleccionando la opción "Solo lectura" para el enlace.

**Resultado esperado:** El documento `Lab01_Hallazgos.docx` está completo con todas las secciones, guardado en OneDrive y compartido con el instructor.

**Verificación:** Cierra el documento y vuelve a abrirlo desde OneDrive en el navegador (`onedrive.com`) para confirmar que la versión guardada en la nube está actualizada.

---

## 7. Validación y Pruebas del Laboratorio

Utiliza la siguiente lista de verificación para confirmar que completaste exitosamente todos los objetivos del laboratorio:

| # | Criterio de validación | ¿Completado? |
|---|---|---|
| 1 | Copilot en Excel generó un resumen de las órdenes de compra con número total, monto y top categorías/proveedores | ☐ |
| 2 | Se creó la columna `Alerta_Precio` con la fórmula generada por Copilot y se identificaron las órdenes con variación >10% | ☐ |
| 3 | Se identificaron los productos con cobertura de inventario crítica (<15 días o stock bajo mínimo) | ☐ |
| 4 | Copilot en Power BI generó una narrativa ejecutiva del dashboard de resumen | ☐ |
| 5 | Se identificaron los proveedores con mejor y peor desempeño usando Copilot en Power BI | ☐ |
| 6 | Los datos del CSV de ERP fueron importados correctamente a Excel como tabla estructurada | ☐ |
| 7 | Copilot Chat analizó los movimientos de ERP e identificó patrones de consumo y riesgo de desabasto | ☐ |
| 8 | Copilot Chat detectó al menos 2 anomalías en los datos de ERP | ☐ |
| 9 | Se generó un Plan de Acción Priorizado con al menos 6 acciones en formato de tabla | ☐ |
| 10 | El documento `Lab01_Hallazgos.docx` está completo y guardado en OneDrive | ☐ |

**Criterio de aprobación:** Al menos 8 de los 10 criterios deben estar marcados como completados para considerar el laboratorio exitoso.

### Reflexión Final (Opcional — 5 minutos adicionales)

Si el tiempo lo permite, responde brevemente en tu documento de hallazgos:

1. ¿En cuál de los tres bloques (Excel, Power BI, Copilot Chat) encontraste que Copilot fue más útil? ¿Por qué?
2. ¿Hubo algún caso en que la respuesta de Copilot fue incorrecta o incompleta? ¿Cómo lo detectaste?
3. ¿Qué ajustes harías a los prompts utilizados para obtener mejores resultados en un contexto real de trabajo?

---

## 8. Solución de Problemas

### Problema 1 — El botón de Copilot no aparece en Excel o genera error "Copilot no disponible"

**Síntomas:**
- El botón de Copilot no se muestra en la cinta de opciones de Excel.
- Al hacer clic en el botón, aparece el mensaje: *"Copilot no está disponible para este archivo"* o *"Se requiere una licencia de Microsoft 365 Copilot"*.
- El panel de Copilot se abre pero muestra un error al intentar enviar un prompt.

**Causa probable:**
El archivo de Excel está guardado en el disco local (`C:\Usuarios\...`) en lugar de en OneDrive for Business, o la licencia de Microsoft 365 Copilot no está activa para la cuenta del usuario. Copilot en Excel **requiere obligatoriamente** que el archivo esté en OneDrive o SharePoint para acceder al contenido del documento.

**Solución paso a paso:**

1. Verifica la ubicación del archivo: en la barra de título de Excel, busca el ícono de nube (☁️). Si no aparece, el archivo está en local.
2. Si está en local: haz clic en **Archivo > Guardar una copia** y selecciona **OneDrive — [Nombre de tu organización]**. Guarda el archivo en la carpeta `Curso_Copilot_Suministros > Modulo1`.
3. Cierra el archivo y vuelve a abrirlo **desde OneDrive** (ya sea desde el explorador de archivos apuntando a la carpeta sincronizada de OneDrive, o desde `onedrive.com` en el navegador).
4. Si el problema persiste después de mover el archivo a OneDrive, verifica la licencia: abre `https://portal.microsoft.com`, inicia sesión con tu cuenta corporativa, ve a **Mi cuenta > Suscripciones** y confirma que "Microsoft 365 Copilot" aparece como licencia activa.
5. Si la licencia no aparece, contacta al instructor para que coordine con el área de TI. Como alternativa temporal, usa **Copilot Chat** en `copilot.microsoft.com` adjuntando el archivo de Excel para continuar con el análisis.

---

### Problema 2 — Copilot Chat genera respuestas genéricas o no analiza el archivo adjunto correctamente

**Síntomas:**
- Copilot Chat responde con información genérica sobre cadena de suministro en lugar de analizar los datos del archivo adjunto.
- El análisis menciona columnas o valores que no existen en el archivo de práctica.
- Copilot indica que "no puede acceder al contenido del archivo" o que "el archivo está vacío".

**Causa probable:**
El archivo adjunto puede no haberse cargado correctamente en el contexto de la sesión de Copilot Chat, o el prompt no especificó con suficiente claridad que la respuesta debe basarse en los datos del archivo adjunto. También puede ocurrir que el archivo CSV no fue convertido a formato `.xlsx` antes de adjuntarlo, lo que dificulta el análisis por parte de Copilot.

**Solución paso a paso:**

1. Verifica que el archivo adjunto fue aceptado por Copilot: debe aparecer un ícono de archivo con el nombre del documento encima del cuadro de texto antes de enviar el prompt.
2. Si el archivo no se cargó, intenta adjuntarlo nuevamente. Si el problema persiste, verifica que el tamaño del archivo no supere los 10 MB (límite habitual de Copilot Chat para adjuntos).
3. Asegúrate de usar el archivo `.xlsx` (no el `.csv` directamente). El CSV importado a Excel y guardado como `.xlsx` tiene mejor compatibilidad con Copilot Chat.
4. Reformula el prompt para hacer explícita la referencia al archivo:

   ```
   Basándote exclusivamente en los datos del archivo Excel adjunto llamado 
   "Lab01_Analisis_ERP.xlsx", responde las siguientes preguntas sobre los 
   movimientos de almacén: [continúa con las preguntas]
   ```

5. Si Copilot sigue sin procesar el archivo, como alternativa copia y pega las primeras 20-30 filas de datos directamente en el chat (incluyendo los encabezados) y solicita el análisis sobre esos datos de muestra. Indica explícitamente: *"Estos datos son una muestra representativa del archivo completo."*
6. Recuerda que Copilot puede generar respuestas diferentes en cada sesión. Si la primera respuesta es insatisfactoria, no elimines el chat — usa un prompt de seguimiento para refinar o corregir el análisis.

---

## 9. Limpieza del Entorno

Al finalizar el laboratorio, realiza los siguientes pasos para dejar el entorno ordenado:

**En Excel:**

1. Cierra el archivo `Lab01_OrdenesDe Compra_Inventario.xlsx`. Si Excel pregunta si deseas guardar cambios, haz clic en **Guardar** (queremos conservar la columna `Alerta_Precio` que creaste).
2. Cierra el archivo `Lab01_Analisis_ERP.xlsx` y guarda los cambios.

**En Power BI Desktop:**

1. Cierra Power BI Desktop. Si pregunta si deseas guardar cambios en el archivo `.pbix`, haz clic en **No guardar** (los archivos de práctica deben mantenerse en su estado original para otros participantes o para repetir el laboratorio).
2. Si publicaste el reporte en Power BI Service durante el Paso B1-alternativo, puedes dejarlo publicado o eliminarlo desde `app.powerbi.com > Mi área de trabajo`.

**En Copilot Chat:**

1. No es necesario eliminar el historial de chat, pero si tu organización tiene políticas de privacidad sobre datos en Copilot, consulta con el instructor si debes limpiar el historial de la sesión.

**Archivos generados:**

| Archivo | Acción |
|---|---|
| `Lab01_Hallazgos.docx` | ✅ Conservar en OneDrive — es el entregable del laboratorio |
| `Lab01_OrdenesDe Compra_Inventario.xlsx` | ✅ Conservar (con columna `Alerta_Precio` agregada) |
| `Lab01_Analisis_ERP.xlsx` | ✅ Conservar en OneDrive |
| `Lab01_Dashboard_Suministros.pbix` | ✅ Conservar sin cambios |

---

## 10. Resumen y Recursos Adicionales

### Resumen del Laboratorio

En este laboratorio aplicaste Microsoft 365 Copilot en tres contextos distintos del ecosistema de datos de suministros:

1. **Copilot en Excel** — Generaste resúmenes automáticos de órdenes de compra, detectaste variaciones de precio superiores al 10% mediante fórmulas asistidas por Copilot, e identificaste productos con riesgo de desabasto en la tabla de inventario. Comprobaste que la calidad del análisis depende directamente de tener los archivos en OneDrive y los datos bien estructurados como tablas.

2. **Copilot en Power BI** — Transformaste visualizaciones del dashboard en narrativas ejecutivas en texto, identificaste proveedores con bajo desempeño y detectaste patrones temporales en el cumplimiento de entregas. Experimentaste cómo Copilot puede ir más allá de la lectura de datos para ofrecer interpretaciones operativas.

3. **Copilot Chat con datos ERP** — Analizaste movimientos de almacén exportados de un sistema ERP para detectar patrones de consumo, riesgos de desabasto y anomalías de registro. Practicaste la construcción de prompts contextualizados para obtener análisis relevantes a partir de datos adjuntos.

4. **Plan de Acción Priorizado** — Consolidaste todos los hallazgos en un prompt estructurado que permitió a Copilot generar un plan de acción ejecutable con responsables y plazos, demostrando el valor de Copilot como herramienta de síntesis y toma de decisiones.

### Conceptos Clave Reforzados

| Concepto | Aplicación en el laboratorio |
|---|---|
| Copilot como capa de inteligencia sobre datos existentes | Usado en Excel, Power BI y Copilot Chat sin modificar las fuentes de datos |
| Requisito de OneDrive para Copilot en Excel | Verificado en la configuración inicial y en el troubleshooting |
| Ingeniería de prompts para suministros | Practicada en cada bloque con prompts específicos y refinamientos |
| Análisis indirecto de datos ERP vía exportación | Demostrado en el Bloque C con el archivo CSV importado a Excel |
| Variabilidad de respuestas de Copilot | Observada al comparar resultados con datos reales de las tablas |

### Recursos Adicionales

- 📖 [Documentación oficial de Microsoft Copilot en Excel](https://support.microsoft.com/es-es/office/introducción-a-copilot-en-excel-d7110502-0334-4b4f-a175-a73abdfc118a)
- 📖 [Guía de Copilot en Power BI Service — Microsoft Learn](https://learn.microsoft.com/es-es/power-bi/create-reports/copilot-introduction)
- 📖 [Descripción general de Microsoft 365 Copilot para empresas](https://learn.microsoft.com/es-es/microsoft-365-copilot/microsoft-365-copilot-overview)
- 📖 [Dar formato a los datos como tabla de Excel (prerrequisito para Copilot)](https://support.microsoft.com/es-es/office/dar-formato-a-los-datos-como-tabla-de-excel-e81aa349-b006-4f8a-9806-5af9df0ac664)
- 📖 [Integración de Microsoft Dynamics 365 con Microsoft 365 Copilot](https://learn.microsoft.com/es-es/dynamics365/copilot/copilot-for-finance-overview)

### Próximos Pasos

En el **Laboratorio 01-00-02** profundizarás en la identificación de patrones recurrentes y la generación de alertas proactivas en la cadena de suministro, aplicando los prompts de análisis que practicaste hoy para construir una lógica de monitoreo continuo con Copilot.

---

> 💡 **Recordatorio final:** Las respuestas de Copilot son un punto de partida para el análisis, no una conclusión definitiva. Siempre valida los hallazgos críticos contra los datos originales antes de tomar decisiones operativas o presentar resultados a la dirección.

---

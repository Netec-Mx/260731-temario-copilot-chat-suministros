# Aplicación de Copilot como apoyo en investigaciones de mercado, análisis de precios, benchmarking y evaluación de tendencias relevantes para Suministros.

## 1. Metadatos del Laboratorio

| Atributo | Detalle |
| :--- | :--- |
| **Duración** | 60 minutos |
| **Complejidad** | Intermedia - Investigación de Mercado y Selección Estratégica de Proveedores |
| **Audiencia** | Equipos de Compras, Almacenes y Comercio Exterior. |
| **Tecnologías** | Microsoft Copilot Chat (Gratuito / M365), Microsoft Excel y Microsoft Word. |
| **Enfoque** | Investigación de costos/mercado, benchmarking comparativo de proveedores, análisis de tendencias y documentación ejecutiva. |

---

## 2. Descripción Corta

En este laboratorio práctico de 60 minutos, los participantes aplicarán Microsoft Copilot Chat para acelerar las investigaciones de mercado, análisis de precios y benchmarking de proveedores en el área de suministros. A lo largo de 6 fases secuenciales, los estudiantes recopilarán tendencias de precios y factores de costo, estructurarán una matriz comparativa con exportación directa a Excel, redactarán un informe de evaluación en Word, generarán un soporte visual del ecosistema y resolverán un reto autónomo de negociación estratégica.

---

## 3. Objetivos del Laboratorio

Al finalizar este laboratorio, el estudiante será capaz de:
* **Investigar rangos de precios, factores de costo y tendencias** de insumos o servicios logísticos mediante búsquedas asistidas en Copilot Chat.
* **Estructurar matrices de benchmarking de proveedores** evaluando criterios de costo, calidad, tiempos y prácticas sostenibles.
* **Exportar matrices de datos analíticos a Microsoft Excel** de forma limpia y directa sin errores de formato.
* **Sintetizar hallazgos de mercado en un informe ejecutivo formal en Microsoft Word** respaldado por maquetas gráficas generadas por IA.

---

## 4. Prerrequisitos

* Cuenta activa de **Microsoft Copilot Chat (Gratuito / M365)**.
* Aplicación de **Microsoft Excel** abierta.
* Aplicación de **Microsoft Word** abierta.

---

## 5. Procedimiento Paso a Paso

### Fase 1: Investigación de Mercado y Estructura de Costos (Cost Breakdown)

Identificaremos los factores que componen el precio de un insumo/servicio crítico y sus tendencias actuales en el mercado internacional o regional.

1. Abra la interfaz de **Microsoft Copilot Chat**.
2. Copie y ejecute el siguiente prompt:

```
Actúa como un Especialista en Inteligencia de Mercado para Compras Estratégicas. Necesito realizar una investigación sobre el servicio de "Flete Marítimo Internacional y Almacenaje de Contenedores" (o un insumo industrial clave como Resina Plástica/Acero).

Por favor, proporcióname:
1. Una lista de los 4 componentes principales que integran la estructura de costo (drivers de costo: ej. combustible, tarifas portuarias, mano de obra, seguros).
2. Un estimado del rango de precios promedio actual en el mercado y su tendencia estimada para los próximos trimestres.
3. Tres supuestos de mercado que el equipo de Compras debe validar externamente antes de tomar una decisión de contratación.

Sintetiza la respuesta en formato de tabla limpia y viñetas ejecutivas.
```

3. Copie los hallazgos generados por el chat para utilizarlos en los pasos siguientes.

---

### Fase 2: Benchmarking Comparativo de Proveedores y Modelos Logísticos

Evaluaremos una terna de proveedores bajo criterios ponderados para identificar la opción de menor riesgo y mayor beneficio integral.

1. En la misma ventana de Copilot Chat, ejecute el siguiente prompt:

```
Actúa como un Consultor de Benchmarking de Suministros. Crea una matriz comparativa simulada de 3 proveedores internacionales/nacionales para la contratación del servicio o insumo investigado en la Fase 1.

Genera una tabla con las siguientes columnas:
- Proveedor
- Precio_Unitario_USD
- Tiempo_Entrega_Dias
- Certificacion_Calidad_ISO
- Nivel_Servicio_Garantizado_SLA%
- Practicas_Sostenibilidad_ESG (Alta, Media, Básica)

Asegúrate de que la tabla refleje compensaciones reales (ej. un proveedor es más barato pero con mayor tiempo de entrega, y otro es más costoso pero con SLA superior y certificaciones ESG).
```

---

### Fase 3: Consolidación y Exportación Directa e Inmediata a Excel

Llevaremos la matriz comparativa a Excel. Para evitar que las columnas se peguen amontonadas en una sola celda, le pediremos a Copilot los datos estructurados en formato de tabulación TSV.

1. Abra **Microsoft Excel** con un libro nuevo en blanco.
2. En Copilot Chat, ejecute el siguiente prompt:

```
Actúa como un Especialista en Datos de Excel. Toma la matriz comparativa de la Fase 2 y preséntala en una TABLA MARKDOWN RENDERIZADA limpia y clara (no uses bloques de código con formato de texto sin formato).

Reglas estrictas de la respuesta:

Utiliza el formato de tabla estándar de Markdown con barras verticales (|).

Las columnas deben ser exactamente:
| Proveedor | Precio_Unitario_USD | Tiempo_Entrega_Dias | Certificacion_ISO | SLA_Garantizado_% | Nivel_ESG | Puntaje_Tecnico_1a10 | Puntaje_Economico_1a10 | Recomendacion_Final |

Incluye los datos de los 3 proveedores de la Fase 2.

Agrega una última fila llamada PROMEDIO_MERCADO y coloca la fórmula explícita =PROMEDIO(B2:B4) en la celda correspondiente al precio.

Asegúrate de que la tabla se muestre de forma visual y elegante en el chat para que el usuario pueda seleccionar los datos con el mouse o copiar la tabla y pegarla directamente en Excel en la celda A1.
```

3. Haga clic en el botón **"Copiar"** (Copy) en la esquina superior del bloque de código generado por Copilot.
4. Vaya a su hoja de **Microsoft Excel**, seleccione la celda **A1** y presione `Ctrl + V`. Verá que cada dato se coloca automáticamente en su columna correspondiente.
5. Guarde el archivo como `Benchmarking_Proveedores_Suministros.xlsx`.

---

### Fase 4: Generación Visual del Ecosistema de Mercado (Imagen)

Generaremos un apoyo gráfico en Copilot Chat para representar el mapa del mercado que se insertará en nuestro reporte de Word.

1. Introduzca el siguiente prompt directamente en Copilot Chat:

```
Genera una imagen conceptual de un "Mapa de Inteligencia de Mercado y Matriz de Proveedores para Cadena de Suministro".

Estilo visual: Diseño corporativo UI/UX moderno, estilo infografía clara, tema empresarial azul oscuro, verde teal y blanco.
Elementos visuales que debe contener:
1. Centro: Un ícono de globo terráqueo con rutas marítimas/terrestres interconectadas.
2. Alrededor: Tres tarjetas o cuadrantes destacados titulados "Análisis de Precios", "Evaluación de Riesgo Proveedor" y "Tendencias ESG".
3. Gráficos circulares simples y barras comparativas de estilo ejecutivo.
```

2. Guarde la imagen descargada directamente desde la ventana del chat.

---

### Fase 5: Redacción del Informe Ejecutivo en Microsoft Word

Estructuraremos la narrativa gerencial y el análisis justificativo directamente para su entrega formal en Microsoft Word.

1. Abra **Microsoft Word** con un documento en blanco.
2. Solicite a Copilot Chat la redacción del informe formal con el siguiente prompt:

```
Actúa como un Líder de Compras Estratégicas y Comercio Exterior. Redacta un "Informe Ejecutivo de Investigación de Mercado y Selección de Proveedores" formal para Microsoft Word.

Utilizando los datos analizados en las fases previas, estructura el documento con las siguientes secciones:
1. **Encabezado y Resumen Ejecutivo:** Síntesis de la situación del mercado, tendencias de precios y drivers de costo identificados.
2. **Evaluación de la Terna de Proveedores:** Un análisis narrativo comparativo destacando las fortalezas, riesgos y nivel de servicio de cada opción evaluada.
3. **Justificación de la Adjudicación:** Argumentación técnica y económica que respalde la elección del proveedor ganador y los próximos pasos para la firma del contrato.

Mantén un tono estrictamente corporativo, claro, profesional y estructurado con títulos y subtítulos.
```

3. Copie el texto generado por Copilot Chat y péguelo en su archivo de Word.
4. Inserte la imagen del mapa de inteligencia de mercado (generada en la Fase 4) justo debajo del Resumen Ejecutivo.
5. Guarde el documento como `Informe_Investigacion_Mercado.docx`.

---

### Fase 6: Reto de Aplicación Autónoma – Benchmarking de Tarifas de Almacenamiento y 3PL

**Escenario del Reto:** La gerencia requiere evaluar a 3 operadores logísticos 3PL (Third-Party Logistics) para tercerizar el almacenamiento de producto terminado en una nueva zona geográfica.

#### Pistas y Guía para Resolver el Reto:

* **Pista 1 (Investigación y Matriz en Excel):**
  * *Estructura sugerida para el Prompt en Copilot Chat:* Solicita a Copilot Chat en formato TSV una tabla con 3 operadores 3PL analizando: `Operador_3PL`, `Costo_Posicion_Pallet_USD`, `Flexibilidad_Espacio_M2`, `Sistemas_WMS_Integrable` (Sí/No) y `Distancia_A_Puerto_KM`.
  * *Cálculo:* Pídele a Copilot que identifique el operador con el costo por pallet más competitivo.
  * Copie el bloque de código y péguelo en una nueva pestaña llamada `Reto_3PL_Benchmarking` en el archivo `Benchmarking_Proveedores_Suministros.xlsx`.

* **Pista 2 (Visual del Proceso 3PL en Chat):**
  * *Estructura sugerida para el Prompt:* En Copilot Chat, solicita directamente: *"Genera una imagen conceptual de un esquema comparativo de Almacenamiento 3PL y Red Logística..."*.
  * *Detalles:* Pide un estilo claro (Light Mode) con íconos de centro de distribución, camiones y conectividad digital.

* **Pista 3 (Reporte Final en Word):**
  * Pide a Copilot Chat que redacte un reporte de 1 página en Word titulado *"Selección Estratégica de Operador Logístico 3PL"*.
  * Pegue el contenido al final de su archivo `Informe_Investigacion_Mercado.docx` o cree un documento nuevo llamado `Informe_Reto_3PL.docx` e inserte la imagen generada.

---

## 6. Conceptos Clave para Recordar

* **Benchmarking de Suministros:** Metodología sistemática para evaluar y comparar productos, servicios y procesos de trabajo de proveedores frente a los mejores estándares del mercado.
* **Formato TSV (Tab-Separated Values):** Estructura de texto limpio separada por tabulaciones que permite copiar datos desde la web o IA y pegarlos directamente en Microsoft Excel sin perder la estructura de filas y columnas.
* **Uso Responsable de Información Externa:** Validación rigurosa que el analista debe realizar sobre los datos generados por IA, contrastando supuestos de mercado con fuentes oficiales y cotizaciones reales antes de autorizar contratos.

---

## 7. Resultado Esperado del Estudiante

El portafolio de evidencias de esta práctica debe incluir:

1. **Archivo de Excel (`Benchmarking_Proveedores_Suministros.xlsx`):**
   * **Pestaña `Matriz_Proveedores`:** Evaluación comparativa pegada limpiamente desde el bloque TSV (Fase 3).
   * **Pestaña `Reto_3PL_Benchmarking`:** Matriz comparativa de operadores logísticos 3PL del reto (Fase 6).
2. **Archivo de Word (`Informe_Investigacion_Mercado.docx`):**
   * Reporte ejecutivo con el análisis de mercado y la justificación de adjudicación (Fase 5).
   * Imagen del mapa de inteligencia de mercado incrustada (Fase 4).

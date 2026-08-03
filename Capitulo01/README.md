# Uso de Copilot para acelerar el análisis de información extraída de Excel, Power BI y sistemas ERP, identificando patrones, riesgos, anomalías y acciones prioritarias.

## 1. Metadatos del Laboratorio

| Atributo | Detalle |
| :--- | :--- |
| **Duración** | 60 minutos |
| **Complejidad** | Intermedia - Analítica Operativa y Cadena de Suministro |
| **Audiencia** | Equipos de Compras, Almacenes y Comercio Exterior. |
| **Tecnologías** | Microsoft Copilot Chat (Gratuito / M365), Microsoft Excel y Microsoft Word. |
| **Enfoque** | Extracción e interpretación de reportes ERP/Power BI, identificación de desabasto, rutas críticas y síntesis ejecutiva. |

---

## 2. Descripción Corta

En este laboratorio de 60 minutos, los participantes aplicarán Microsoft Copilot Chat sobre reportes masivos extraídos de un sistema ERP (SAP/Oracle) para acelerar el análisis de inventarios, compras y comercio exterior. A través de 6 fases secuenciales, el estudiante simulará la descarga de datos transaccionales, detectará anomalías y riesgos de desabasto, consolidará KPIs en Excel, generará apoyos gráficos del proceso y redactará un informe de acciones prioritarias en Microsoft Word.

---

## 3. Objetivos del Laboratorio

Al finalizar este laboratorio, el estudiante será capaz de:
* **Interpretar reportes transaccionales de ERP y Power BI** mediante prompts de análisis avanzado en Copilot Chat.
* **Identificar materiales en riesgo, proveedores críticos y anomalías de gasto** en grandes volúmenes de datos.
* **Generar alertas tempranas de inventario** para evitar quiebres de stock en operaciones de Compras y Almacén.
* **Sintetizar hallazgos analíticos en un reporte ejecutivo formal en Microsoft Word** orientado a la toma de decisiones.

---

## 4. Prerrequisitos

* Cuenta activa de **Microsoft Copilot Chat (Gratuito / M365)**.
* Aplicación de **Microsoft Excel** abierta.
* Aplicación de **Microsoft Word** abierta.

---

## 5. Procedimiento Paso a Paso

### Fase 1: Extracción Sintética de Reporte ERP (SAP / Oracle)

Simularemos un reporte de extracción masiva del sistema ERP que contiene datos cruzados de compras, inventario actual y tránsito internacional.

1. Abra la interfaz de **Microsoft Copilot Chat**.
2. Copie y ejecute el siguiente prompt:

```
Actúa como un Especialista Senior de Datos en Cadena de Suministro. Genera un dataset en una tabla Markdown con 12 filas que simule una extracción directa de un sistema ERP (módulo MM/SD).

Las columnas deben ser:
- `SKU_Material`
- `Descripcion_Material`
- `Categoria` (Materia Prima, Repuestos, Empaque)
- `Stock_Actual_Unidades`
- `Punto_Reorden_Unidades`
- `Proveedor_Principal`
- `Lead_Time_Dias`
- `Estatus_Transito` (Nacional, En Puerto/Aduana, En Nave)
- `Gasto_Mensual_USD`

Asegúrate de incluir casos críticos:
1. Al menos 3 materiales con `Stock_Actual` por debajo del `Punto_Reorden`.
2. Un proveedor concentrando el mayor gasto con retrasos de `Lead_Time` superiores a 45 días.
3. Materiales importados retenidos en aduana.
```

3. Copie la tabla generada para utilizarla en las fases siguientes.

---

### Fase 2: Identificación de Riesgos, Anomalías y Alertas Tempranas

Someteremos la extracción del ERP a un análisis guiado por IA para identificar los cuellos de botella y materiales críticos.

1. En la misma ventana de Copilot Chat, ejecute el siguiente prompt:

```
Actúa como un Analista de Riesgos de Suministros y Comercio Exterior. Analiza la tabla ERP extraída en la Fase 1 y realiza las siguientes tareas:

1. **Alertas de Desabasto:** Enlista los SKUs cuyo `Stock_Actual` esté por debajo del `Punto_Reorden` y calcula el déficit en unidades.
2. **Rutas y Proveedores Críticos:** Identifica cuál es el proveedor que representa el mayor riesgo operativo por combinación de `Gasto_Mensual_USD` y alto `Lead_Time_Dias`.
3. **Bloqueo de Comercio Exterior:** Filtra los materiales que se encuentran detenidos en `Estatus_Transito` "En Puerto/Aduana" y calcula el valor financiero estancado.

Presenta las conclusiones agrupadas en 3 categorías claras con listas numeradas.
```

---

### Fase 3: Consolidación y Exportación a Matriz de Control en Excel

Transformaremos las conclusiones analíticas de Copilot en una matriz de control de inventarios para trabajar en Excel.

1. Abra **Microsoft Excel** con un libro en blanco.
2. Ejecute el siguiente prompt en Copilot Chat:

```
Toma los hallazgos de las Fases 1 y 2 y organízalos en una tabla limpia de "Matriz de Priorización de Compras y Almacén".

La tabla debe tener las columnas:
- `SKU_Material`
- `Descripcion`
- `Nivel_Riesgo` (Crítico, Medio, Normal)
- `Accion_Inmediata_Sugerida` (Ej. Expeditar compra, Alternativa nacional, Gestión aduanal)
- `Responsable_Area` (Compras, Almacén, Comercio Exterior)

Asegúrate de que la estructura esté lista para copiar directamente a una hoja de cálculo.
```

3. Copie la tabla generada por Copilot Chat, péguela en Excel y guarde el archivo como `Control_Riesgos_Suministros.xlsx`.

---

### Fase 4: Generación Visual de la Maqueta de Proceso (Imagen)

Aprovecharemos la generación de imágenes en el chat de Copilot para crear un diagrama conceptual del flujo de alertas que acompañará el reporte oficial.

1. Introduzca el siguiente prompt directamente en Copilot Chat:

```
Genera una imagen conceptual de una infografía visual sobre "Flujo de Alertas Tempranas y Control de Suministros".

Estilo visual: Diseño corporativo limpio, moderno, fondo claro (Light Mode) con acentos en azul industrial y verde de aprobación.
Elementos visuales que debe incluir:
1. Tres fases conectadas por flechas: Extracción ERP (ícono de base de datos), Análisis de Riesgo por IA (ícono de lupa y chip) y Acción Prioritaria (ícono de camión y escudo de seguridad).
2. Tarjetas flotantes elegantes con números y etiquetas claras.
3. Apariencia de un estándar operativo de cadena de suministro profesional.
```

2. Guarde la imagen generada directamente desde el chat.

---

### Fase 5: Redacción del Reporte Gerencial de Suministros en Word

Estructuraremos el documento formal que se entregará a las jefaturas de Compras, Almacén y Comercio Exterior.

1. Abra **Microsoft Word** con un documento en blanco.
2. Solicite a Copilot Chat la redacción del reporte formal mediante el siguiente prompt:

```
Actúa como Gerente de Suministros y Logística. Redacta un "Informe Ejecutivo de Diagnóstico de Inventarios y Alertas Tempranas" para la Dirección de Operaciones en Microsoft Word.

Utilizando los datos analizados en las fases previas, estructura el documento con los siguientes puntos:
1. **Encabezado y Resumen Ejecutivo:** Un párrafo sintetizando la situación de riesgo actual del inventario y las mercancías en tránsito.
2. **Matriz de Análisis Operativo:** Resumen narrativo sobre los materiales en punto de quiebre, el proveedor crítico y los embarques retenidos en aduana.
3. **Plan de Acción Inmediato:** 3 recomendaciones concretas divididas por área (Compras, Almacenes y Comercio Exterior) con plazos de ejecución en horas/días.

Mantén un tono ejecutivo, directo y enfocado en la mitigación del riesgo operacional.
```

3. Copie el texto generado por Copilot Chat en su archivo de Word.
4. Inserte la imagen del flujo de alertas (generada en la Fase 4) debajo del Resumen Ejecutivo.
5. Guarde el archivo como `Informe_Diagnostico_Suministros.docx`.

---

### Fase 6: Reto de Aplicación Autónoma – Análisis de Variación de Costos y Rutas Críticas

**Escenario del Reto:** Se ha detectado un incremento inesperado en los costos de flete internacional y una desviación en los tiempos de entrega de materia prima crítica de importación.

#### Pistas y Guía para Resolver el Reto:

* **Pista 1 (Dataset y Análisis en Excel):**
  * *Estructura sugerida para el Prompt en Copilot Chat:* Pídele a la IA que cree una tabla con 6 proveedores internacionales mostrando: `Proveedor`, `Insumo`, `Costo_Flete_Anterior_USD`, `Costo_Flete_Actual_USD` y `Dias_Retraso_Acumulado`.
  * *Cálculo:* Indícale a Copilot Chat que identifique el % de incremento en el costo de flete y filtre los proveedores con más de 10 días de retraso.
  * Guarda estos datos en una nueva pestaña llamada `Reto_Fletes_Aduana` en tu archivo `Control_Riesgos_Suministros.xlsx`.

* **Pista 2 (Generación Gráfica en Chat):**
  * *Estructura sugerida para el Prompt:* Solicita directamente en Copilot Chat: *"Genera una imagen con un diagrama visual que represente un 'Plan de Contingencia para Rutas Críticas de Importación'..."*.
  * *Detalles:* Pide un mapa conceptual estilizado con iconos de barco de carga, aduana y almacén en tonos corporativos.

* **Pista 3 (Reporte Final en Word):**
  * Solicita a Copilot Chat que redacte un reporte de 1 página titulado *"Memoria de Impacto en Costos de Flete y Contingencia de Comercio Exterior"*.
  * Copia el texto a Word, inserta la imagen del plan de contingencia generada en la Pista 2 y guarda el documento como `Informe_Impacto_Fletes.docx`.

---

## 6. Conceptos Clave para Recordar

* **Punto de Reorden (ROP):** Nivel crítico de inventario que activa automáticamente una solicitud de compra para evitar el desabasto antes de que llegue el nuevo pedido.
* **Lead Time (Tiempo de Entrega):** Total de días transcurridos desde que se emite la orden de compra hasta que la mercancía está disponible en el almacén.
* **Consolidación ERP-AI:** Proceso de extraer datos crudos de sistemas de gestión (SAP, Oracle, Dynamics) y procesarlos en Copilot Chat para reducir tiempos de análisis de horas a minutos.

---

## 7. Resultado Esperado del Estudiante

El portafolio de evidencias de esta práctica debe incluir:

1. **Archivo de Excel (`Control_Riesgos_Suministros.xlsx`):**
   * **Pestaña `Matriz_Riesgos`:** Matriz de priorización de compras y almacén (Fase 3).
   * **Pestaña `Reto_Fletes_Aduana`:** Análisis de variación de fletes y retrasos del reto (Fase 6).
2. **Archivo de Word (`Informe_Diagnostico_Suministros.docx`):**
   * Reporte estructurado formalmente con el diagnóstico de inventarios y plan de acción (Fase 5).
   * Imagen del flujo de alertas incrustada (Fase 4).
3. **Archivo de Word (`Informe_Impacto_Fletes.docx`):**
   * Reporte final del reto autónomo con la imagen del plan de contingencia incrustada (Fase 6).

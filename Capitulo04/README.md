# Aplicación de Copilot como apoyo en la validación de procesos operativos, decisiones críticas y análisis inicial de cambios regulatorios.

## 1. Metadatos del Laboratorio

| Atributo | Detalle |
| :--- | :--- |
| **Duración** | 90 minutos |
| **Complejidad** | Avanzada - Gobierno de Procesos, Análisis Regulatorio y Gestión de Decisiones |
| **Audiencia** | Líderes de comercio exterior, gerentes de operaciones, auditores de procesos, especialistas de cumplimiento y compras. |
| **Tecnologías** | Microsoft Copilot Chat (M365 / Web), Microsoft PowerPoint, Microsoft Word y Microsoft Excel. |
| **Enfoque** | Detección de puntos de falla en la cadena de suministro, auditoría de cumplimiento normativo, evaluación de cambios regulatorios y presentación ejecutiva de adaptaciones. |

---

## 2. Descripción Corta

En este laboratorio de 90 minutos, los participantes utilizarán Microsoft Copilot Chat para validar la solidez de los procesos de compra, almacenamiento y comercio exterior frente a cambios normativos y riesgos operativos. A través de un flujo estructurado en 7 fases (Mapas de Falla en Word, Matriz de Cumplimiento en Excel, Generación de Diagramas de Flujo/Gráficos, Generación de Infografía de Impacto Regulatorio, Presentación Ejecutiva en PowerPoint, Resumen Estratégico y Reto Autónomo Guiado), el estudiante articulará la suite completa de Microsoft 365 para sostener decisiones operativas de alto nivel.

---

## 3. Objetivos del Laboratorio

Al finalizar este laboratorio, el estudiante será capaz de:
* **Auditar flujos operacionales de comercio exterior y almacenes** para detectar vacíos de control y puntos únicos de falla (SPOF).
* **Evaluar el impacto conceptual de modificaciones regulatorias y aduanales** en la cadena de suministro.
* **Diseñar checklists de cumplimiento y matrices de control normativo** exportables a Excel.
* **Crear componentes visuales (gráficos de árbol/flujo e infografías)** solicitados directamente en el chat para ilustrar riesgos.
* **Estructurar una presentación ejecutiva de cambio normativo para PowerPoint** sintetizando impactos de negocio y planes de adaptación.

---

## 4. Prerrequisitos

* Cuenta activa de **Microsoft Copilot Chat (M365 / Web)** (con capacidad de generación de imágenes integrada).
* Aplicación de **Microsoft Word** abierta.
* Aplicación de **Microsoft Excel** abierta.
* Aplicación de **Microsoft PowerPoint** abierta.

---

## 5. Procedimiento Paso a Paso

### Fase 1: Diagnóstico de Procesos Operativos y Detección de Puntos de Falla (Word)

Evaluaremos el flujo de importación y recepción de mercancía nacionalizada para identificar vacíos de control legal y operativo.

1. Abra **Microsoft Word** con un documento en blanco.
2. Abra la interfaz de **Microsoft Copilot Chat**.
3. Copie y ejecute el siguiente prompt:

```
Actúa como un Auditor Senior de Procesos Logísticos y Comercio Exterior. Analiza el siguiente flujo descriptivo de un proceso de importación:

"El departamento de Compras emite la Orden de Compra al proveedor extranjero. Cuando el embarque llega a la aduana, el agente aduanal realiza el despacho y envía la factura. La mercancía se traslada al almacén central donde los montacarguistas reciben los pallets, firman la carta de porte al operador del camión y acomodan el material. Si faltan documentos de origen o pedimento, el material se guarda temporalmente en una esquina del almacén mientras Compras arregla el expediente."

Realiza lo siguiente:
1. Identifica los 4 puntos de falla críticos (puntos ciegos o brechas de cumplimiento) en este proceso.
2. Explica el riesgo legal, fiscal o de inventario que representa cada punto de falla.
3. Redacta la reingeniería del proceso proponiendo controles estrictos para cada etapa.

Presenta el diagnóstico con tono formal listo para incorporar a Word.
```

4. Copie el texto generado por Copilot Chat y péguelo en su documento de Word. Guarde el archivo como `Auditoria_Procesos_y_Riesgos.docx`.

---

### Fase 2: Matriz de Riesgos Normativos y Checklist de Cumplimiento (Excel)

Transformaremos los riesgos identificados en una matriz de control de cumplimiento apta para auditoría.

1. Abra **Microsoft Excel** con un libro en blanco.
2. En Copilot Chat, ejecute el siguiente prompt:

```
Actúa como un Especialista en Cumplimiento Normativo Aduanero. Toma las fallas y controles identificados en la Fase 1 y genera una TABLA MARKDOWN RENDERIZADA (no uses bloques de código sin formato).

Reglas de la respuesta:
1. Utiliza el formato de tabla estándar de Markdown con barras verticales (|).
2. Las columnas deben ser exactamente:
   | ID_Control | Etapa_Proceso | Punto_de_Falla | Requisito_Normativo_Obligatorio | Frecuencia_Auditoria | Responsable_Directo | Estatus_Cumplimiento |
3. Incluye los 4 puntos de control analizados previamente.
4. Agrega una última fila llamada "EVALUACIÓN DE RIESGO GLOBAL" con la instrucción: "NIVEL DE CUMPLIMIENTO REQUERIDO: 100%".

Asegúrate de que la tabla sea fácil de seleccionar con el mouse para copiar y pegar directamente en Excel.
```

3. Seleccione la tabla en la ventana de Copilot Chat, presione `Ctrl + C`, vaya a Excel en la celda **A1** y presione `Ctrl + V`.
4. Guarde el archivo como `Matriz_Cumplimiento_Normativo.xlsx`.

---

### Fase 3: Generación Gráfica de Diagramas de Flujo y Árbol de Decisiones (Gráfico)

Generaremos un diagrama visual que muestre el árbol de decisión para la liberación de mercancía regulada en almacén.

1. Ingrese el siguiente prompt directamente en el chat de Copilot:

```
Genera una imagen conceptual que muestre un "Diagrama de Árbol de Decisiones para Liberación de Mercancía Aduanal en Almacén".

Estilo visual: Esquema visual técnico y moderno estilo diagrama de flujo de ingeniería de procesos, en tonos azul marino, verde esmeralda y blanco.
Contenido que debe mostrar la imagen:
1. Nodo raíz superior: "Llegada de Contenedor a Rampa".
2. Rombo de decisión central: "¿Pedimento y Permisos Validados?".
3. Rama Sí (Verde): "Apertura y Carga en WMS".
4. Rama No (Rojo/Naranja): "Bloqueo Automático en Zona de Cuarentena" y "Notificación a Cumplimiento".
5. Conectores claros con flechas e íconos de seguridad documental.
```

2. Guarde la imagen generada directamente desde la conversación para utilizarla en la documentación.

---

### Fase 4: Análisis de Impacto Regulatorio y Generación de Infografía (Infografía)

Analizaremos conceptualmente el impacto de un cambio en regulaciones ambientales/sustentables en la cadena de empaque y transporte, generando una infografía ejecutiva.

1. Ejecute el siguiente prompt en Copilot Chat:

```
Actúa como un Consultor en Regulación Marítima y Ambiental. Analiza el impacto de una nueva normativa que exige un "Límite del 0.5% en emisiones de carbono para el transporte de carga y prohibición de plásticos de un solo uso en empaques de exportación".

Genera dos entregables en tu respuesta:
1. Un resumen analítico con: Impacto Financiero en Tarifas de Flete, Cambios Requeridos en Almacén y Riesgo de Sanciones.
2. A continuación, genera una imagen de una "Infografía de Impacto Regulatorio y Sustentabilidad Logística".

Detalles visuales de la infografía:
- Estilo: Infografía ejecutiva vertical en tema oscuro con detalles en verde neón y azul cian.
- Secciones: Bloque superior "Nueva Normativa Ambiental", Bloque medio "3 Pilares de Impacto (Costos, Empaque, Flota)" y Bloque inferior "Estrategia de Adaptación 2026".
```

2. Guarde la imagen de la infografía generada en el chat.

---

### Fase 5: Estructuración de la Presentación Ejecutiva (PowerPoint)

Estructuraremos una presentación de alto nivel para la junta directiva solicitando la distribución diapositiva por diapositiva.

1. Abra **Microsoft PowerPoint** con una presentación en blanco.
2. En Copilot Chat, ejecute el siguiente prompt:

```
Actúa como un Director de Operaciones y Cumplimiento. Necesito diseñar una presentación ejecutiva de 5 diapositivas para la Junta Directiva titulada: "Estrategia de Adaptación Normativa y Mitigación de Riesgos Operativos".

Proporcióname la estructura y contenido detallado diapositiva por diapositiva:
- **Diapositiva 1:** Título, Subtítulo y Mensaje Principal.
- **Diapositiva 2:** Diagnóstico de Riesgos Actuales (3 puntos críticos encontrados en auditoría).
- **Diapositiva 3:** Impacto del Cambio Regulatorio (Costos vs Implicaciones Legales).
- **Diapositiva 4:** Plan de Acción de 3 Fases (Corto, Mediano y Largo Plazo).
- **Diapositiva 5:** Conclusión y Solicitud de Presupuesto/Aprobación.

Para cada diapositiva, incluye: Título de la diapositiva, Viñetas de contenido clave y la Sugerencia del recurso visual a colocar (ej. imágenes, diagramas, tablas).
```

3. Construya las 5 diapositivas en PowerPoint utilizando el contenido proporcionado.
4. En la Diapositiva 2, inserte la imagen del Diagrama de Decisiones (Fase 3), y en la Diapositiva 3, inserte la Infografía de Impacto (Fase 4).
5. Guarde la presentación como `Presentacion_Adaptacion_Normativa.pptx`.

---

### Fase 6: Síntesis de Decisiones Críticas en Word

Unificaremos los análisis en una Hoja de Decisión Directiva (Decision Memo) para respaldar la aprobación del plan.

1. En Copilot Chat, ejecute el siguiente prompt:

```
Actúa como un Asesor de Alta Dirección. Redacta un "Memorándum de Decisión Directiva" de 1 página para incorporar en Word.

Estructura requerida:
1. **Contexto de la Decisión:** Necesidad urgente de actualizar procesos por cambios regulatorios y hallazgos de auditoría.
2. **Evaluación de Alternativas:** Opción A (Inacción/Riesgo alto) vs Opción B (Transformación de Procesos y Cumplimiento).
3. **Recomendación Final:** Justificación técnica, económica y reputacional para autorizar el presupuesto de adaptación.

Copie el texto y péguelo al final de su archivo `Auditoria_Procesos_y_Riesgos.docx`.
```

---

### Fase 7: Reto de Aplicación Autónoma – Validación de Procesos de Compras y Certificación OEA / CTPAT

**Escenario del Reto:** La empresa busca obtener una certificación de seguridad en la cadena de suministro (como OEA o CTPAT) para agilizar sus cruces fronterizos, pero requiere auditar su proceso actual de selección de proveedores de transporte.

#### Pistas y Guía para Resolver el Reto:

* **Pista 1 (Auditoría y Checklist en Excel):**
  * *Prompt en Copilot Chat:* Solicita en formato de tabla Markdown renderizada para Excel una *"Lista de Verificación de Seguridad para Transporte de Carga (C-TPAT / OEA)"* analizando 5 puntos: Antecedentes del chofer, Rastreo GPS activo, Inspección de 17 puntos del contenedor, Sellos de alta seguridad y Capacitación anti-contrabando.
  * *Acción:* Péguela en una nueva pestaña llamada `Reto_Certificacion_OEA` en el archivo `Matriz_Cumplimiento_Normativo.xlsx`.

* **Pista 2 (Infografía Visual en Chat):**
  * *Prompt en Copilot Chat:* Pide directamente: *"Genera una imagen con una infografía titulada 'Ruta de Certificación OEA/CTPAT' que muestre 4 pasos visuales de auditoría de seguridad..."*.

* **Pista 3 (Presentación de 3 Diapositivas en PowerPoint):**
  * Solicita a Copilot Chat la estructura para 3 diapositivas sobre *"Justificación de Inversión para Certificación OEA"*.
  * Cree una nueva presentación o agregue la sección final en `Presentacion_Adaptacion_Normativa.pptx`, inserte la infografía del reto y guarde los cambios.

---

## 6. Conceptos Clave para Recordar

* **Punto Único de Falla (SPOF):** Etapa vulnerable en un proceso cuya interrupción o falla sin control provoca la detención completa de la operación.
* **Cumplimiento Regulativo (Compliance):** Alineación obligatoria de los procesos de compra, transporte y almacenamiento con las leyes locales e internacionales vigentes.
* **Memorándum de Decisión (Decision Memo):** Documento sintético que resume análisis complejos para facilitar la aprobación ejecutiva por parte de la alta dirección.

---

## 7. Resultado Esperado del Estudiante

El portafolio de evidencias de esta práctica debe incluir:

1. **Archivo de Word (`Auditoria_Procesos_y_Riesgos.docx`):**
   * Diagnóstico de procesos y hallazgos de fallas (Fase 1).
   * Memorándum de Decisión Directiva (Fase 6).
2. **Archivo de Excel (`Matriz_Cumplimiento_Normativo.xlsx`):**
   * **Pestaña `Matriz_Controles`:** Tabla de puntos de control y requisitos normativos (Fase 2).
   * **Pestaña `Reto_Certificacion_OEA`:** Checklist de verificación del reto autónomo (Fase 7).
3. **Archivo de PowerPoint (`Presentacion_Adaptacion_Normativa.pptx`):**
   * Presentación ejecutiva de 5 diapositivas estructurada con análisis de impacto y plan de acción (Fase 5).
   * Imágenes incrustadas del Diagrama de Decisiones (Fase 3), Infografía de Sustentabilidad (Fase 4) e Infografía OEA del reto (Fase 7).

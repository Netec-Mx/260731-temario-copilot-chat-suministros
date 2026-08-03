# Uso de Copilot para revisar, mejorar y generar borradores de documentos clave, reduciendo retrabajos y errores operativos

## 1. Metadatos del Laboratorio

| Atributo | Detalle |
| :--- | :--- |
| **Duración** | 90 minutos |
| **Complejidad** | Interactiva - Estandarización Documental y Gestión de Riesgos |
| **Audiencia** | Coordinadores de tráfico, especialistas de almacén, supervisores de compras y servicio al cliente logístico. |
| **Tecnologías** | Microsoft Copilot Chat (M365 / Web), Microsoft Word y Microsoft Excel. |
| **Enfoque** | Auditoría de documentos confusos, mitigación de ambigüedades en RFQs, creación de SOPs/checklists e instructivos de comunicación. |

---

## 2. Descripción Corta

En este laboratorio de 90 minutos, los participantes utilizarán Microsoft Copilot Chat para transformar documentos operativos ambiguos, correos mal redactados y solicitudes de cotización (RFQ) incompletas en artefactos logísticos estandarizados y profesionales. A través de un flujo estructurado en 7 fases (Auditoría de RFQs, Evaluación de Riesgos, Elaboración de Procedimientos/SOPs, Checklists de Control, Plantillas de Comunicación, Análisis de Formato en Excel y Reto Autónomo Guiado), el estudiante eliminará malentendidos operativos con proveedores y transportistas.

---

## 3. Objetivos del Laboratorio

Al finalizar este laboratorio, el estudiante será capaz de:
* **Identificar y corregir vacíos, ambigüedades y vacíos de responsabilidad** en solicitudes de cotización (RFQ) y correos operativos.
* **Redactar Procedimientos Operativos Estándar (SOPs) e instructivos de trabajo** estructurados de forma lógica mediante Copilot Chat.
* **Diseñar checklists de verificación de campo** para procesos de recepción, embarque y auditoría de inventario.
* **Estandarizar las comunicaciones críticas con proveedores y transportistas** asegurando acuerdos de nivel de servicio (SLA) claros.

---

## 4. Prerrequisitos

* Cuenta activa de **Microsoft Copilot Chat (M365 / Web)**.
* Aplicación de **Microsoft Word** abierta.
* Aplicación de **Microsoft Excel** abierta.

---

## 5. Procedimiento Paso a Paso

### Fase 1: Auditoría y Saneamiento de Solicitudes de Cotización (RFQ) e Emails Obscuros

Analizaremos un correo borrador de cotización enviado a un transportista que carece de especificaciones técnicas esenciales, lo que genera sobrecostos e incongruencias en las tarifas recibidas.

1. Abra la interfaz de **Microsoft Copilot Chat**.
2. Copie y ejecute el siguiente prompt:

```
Actúa como un Auditor de Compras y Contratación Logística. Analiza la siguiente Solicitud de Cotización (RFQ) borradora que un analista redactó para enviar a una empresa de autotransporte:

"Hola, necesito que me cotices el flete para mover unos pallets de azulejo y cerámica desde la planta hasta el almacén del cliente. Son como 15 o 18 toneladas, queremos salir el lunes temprano y llegar lo antes posible. Cotízame la tarifa completa con todo incluido. Saludos."

Por favor, realiza lo siguiente:
1. Enumera los 5 vacíos de información o ambigüedades más graves que pueden provocar sobrecargos, retrasos o rechazo del servicio.
2. Reescribe el texto convirtiéndolo en un Correo Formal de Solicitud de Cotización (RFQ) estructurado con campos claros (origen, destino, tipo de unidad, maniobras, horario de cita, seguro y penalizaciones).
```

3. Revise la reescritura generada y consérvela para la documentación formal.

---

### Fase 2: Evaluación de Riesgos y Matriz de Ambigüedad Documental

Convertiremos los hallazgos de la auditoría en una matriz de control de riesgos operativos para medir el impacto financiero y legal de las malas especificaciones.

1. En la misma ventana de Copilot Chat, ejecute el siguiente prompt:

```
Actúa como un Gestor de Riesgos en Cadena de Suministro. Toma las 5 ambigüedades detectadas en la Fase 1 y genera una Matriz de Riesgo Documental.

Presenta la respuesta en una tabla Markdown con las siguientes columnas:
- ID_Riesgo
- Error_o_Vacio_Detectado
- Impacto_Operativo_o_Financiero
- Nivel_de_Riesgo (Alto, Medio, Bajo)
- Cláusula_de_Mitigación_Sugerida
```

---

### Fase 3: Generación de un Procedimiento Operativo Estándar (SOP) e Instructivo de Trabajo

A partir del problema detectado, utilizaremos Copilot Chat para redactar un procedimiento normativo formal que asegure que todos los embarques sigan las mismas reglas de operación.

1. Abra **Microsoft Word** con un documento en blanco.
2. Ingrese el siguiente prompt en Copilot Chat:

```
Actúa como un Especialista en Procesos y Calidad Logística. Redacta un Procedimiento Operativo Estándar (SOP) titulado: "SOP-LOG-004: Solicitud, Aceptación y Despacho de Unidades de Transporte de Carga".

Estructura el procedimiento con los siguientes apartados normativos:
1. **Objetivo y Alcance:** Aplicable a coordinadores de tráfico y almacenes.
2. **Responsabilidades:** Roles de Tráfico, Transportista y Almacén.
3. **Flujo del Proceso Paso a Paso:** Desde la solicitud de cotización hasta la liberación de la unidad en rampa (incluyendo tiempos límite de confirmación).
4. **Criterios de Rechazo de Unidad:** 4 condiciones obligatorias por las cuales el almacén no debe cargar un camión (ej. piso sucio/húmedo, llantas lisas, sin sellos de seguridad).

Utiliza un lenguaje normativo, técnico y estructurado listo para copiar en Word.
```

3. Copie el texto del SOP y péguelo en su documento de Word. Guarde el archivo como `SOP_Despacho_Transporte.docx`.

---

### Fase 4: Creación del Checklist de Verificación para Operaciones en Rampa

Para asegurar que el SOP de la Fase 3 se cumpla en la práctica diaria, diseñaremos una lista de verificación gráfica/estructurada que los operadores puedan usar en rampa.

1. En Copilot Chat, ejecute el siguiente prompt:

```
Actúa como un Supervisor de Almacén. Basado en los "Criterios de Rechazo de Unidad" del SOP generado en la Fase 3, diseña un "Checklist de Inspección de Transporte previo a Carga".

Muestra la respuesta en una tabla Markdown con el formato:
- Item_A_Inspeccionar
- Criterio_Aceptable
- Estado (Cumple / No Cumple / N/A)
- Observaciones_del_Inspector

Incluye verificaciones para: Estructura de la caja seca/plataforma, Limpieza interna, Elementos de sujeción (bandas/esquineros), Documentación del chofer y Equipo de Protección Personal (EPP).
```

---

### Fase 5: Redacción de Plantillas de Comunicación y Manejo de Escalaciones

Crearemos una biblioteca de correos tipo para gestionar desviaciones comunes (demoras en rampa, rechazo de unidad, cobro indebido de estadías) manteniendo un tono firme pero profesional.

1. Ejecute el siguiente prompt en Copilot Chat:

```
Actúa como un Gerente de Servicio al Cliente y Relaciones con Proveedores Logísticos. Redacta 2 plantillas de comunicación ejecutiva para resolver contingencias:

**Plantilla 1:** Notificación formal de Rechazo de Unidad en Almacén por incumplimiento de condiciones de seguridad/limpieza (exigiendo unidad de reemplazo sin costo adicional en menos de 2 horas).
**Plantilla 2:** Respuesta de aclaración por cobro improcedente de "Estadías/Tiempos muertos" justificando con evidencia de rampa que el retraso fue imputable al operador de la línea de transporte.

Asegúrate de incluir variables entre corchetes tipo `[Nombre_Transportista]`, `[Número_Guía]`, `[Hora_Entrada]`.
```

---

### Fase 6: Estructuración y Exportación de Checklists a Excel

Llevaremos la lista de verificación a Excel para su impresión o integración en dispositivos móviles de revisión en rampa.

1. Abra **Microsoft Excel** con un libro en blanco.
2. Ejecute el siguiente prompt en Copilot Chat:

```
Actúa como un Diseñador de Herramientas Operativas para Excel. Toma el Checklist de la Fase 4 y preséntalo en una TABLA MARKDOWN RENDERIZADA limpia y clara (sin bloques de código sin formato).

Reglas de la respuesta:
1. Utiliza el formato de tabla estándar de Markdown con barras verticales (|).
2. Las columnas deben ser exactamente:
   | No_Item | Categoria | Punto_de_Inspeccion | Criterio_de_Aprobacion | Estatus_Cumplimiento | Accion_Correctiva_Requerida |
3. Llena la tabla con los 6 puntos de inspección trabajados en la Fase 4.
4. Agrega una fila final de firma que diga: "INSPECCIÓN APROBADA (SI/NO):" y "FIRMA DE AUDITOR:".

Asegúrate de que la tabla sea fácil de seleccionar con el mouse para copiar y pegar directamente en la celda A1 de Excel.
```

3. Seleccione la tabla en la ventana de Copilot Chat, presione `Ctrl + C`, vaya a Excel en la celda **A1** y presione `Ctrl + V`.
4. Guarde la hoja como `Checklist_Inspeccion_Rampa.xlsx`.

---

### Fase 7: Reto de Aplicación Autónoma – Instructivo y Protocolo de Devoluciones (RMA)

**Escenario del Reto:** La operación tiene un alto índice de mercancía devuelta por clientes que llega dañada al almacén sin un protocolo claro de aceptación, lo que provoca disputas entre servicio al cliente, transporte y almacén.

#### Pistas y Guía para Resolver el Reto:

* **Pista 1 (Procedimiento de Devolución en Word):**
  * *Prompt en Copilot Chat:* Solicita la redacción de un instructivo corto de 1 página llamado *"Protocolo de Recepción de Devoluciones y Mermas en Almacén (RMA)"*.
  * *Estructura:* Exige que defina: 1) Pasos para recibir mercancía dañada, 2) Evidencia fotográfica obligatoria y 3) Formato de Acta de Incidencia. Copie el texto en su archivo `SOP_Despacho_Transporte.docx` bajo el apartado de Anexos.

* **Pista 2 (Checklist de Recepción en Excel):**
  * *Prompt en Copilot Chat:* Pide una tabla Markdown renderizada para Excel titulada *"Checklist de Calidad para Devolución de Cliente"*, analizando empaque, etiquetas, estado del producto y dictamen final (Apto para re-inventario / Merma destruida).
  * *Acción:* Seleccione la tabla del chat, péguela en su archivo `Checklist_Inspeccion_Rampa.xlsx` en una nueva pestaña llamada `Reto_Checklist_Devoluciones`.

* **Pista 3 (Correo de Escalación):**
  * Solicita a Copilot Chat que redacte una plantilla de correo dirigida al área comercial/cliente explicando el motivo del rechazo de una devolución no autorizada o fuera de tiempo de política.

---

## 6. Conceptos Clave para Recordar

* **Ambigüedad Operativa:** Deficiencia en la redacción de instrucciones o contrataciones que deja espacio a interpretaciones libres, derivando en retrasos, cargos extras o disputas contractuales.
* **SOP (Standard Operating Procedure):** Documento normativo formal que describe paso a paso cómo debe ejecutarse una tarea para garantizar consistencia y calidad.
* **Validación en Rampa:** Proceso físico de inspección mediante checklist antes de autorizar la carga o descarga de una unidad para deslindar responsabilidades de daño en tránsito.

---

## 7. Resultado Esperado del Estudiante

El portafolio de evidencias de esta práctica debe incluir:

1. **Archivo de Word (`SOP_Despacho_Transporte.docx`):**
   * Correo de RFQ reescrito y corregido (Fase 1).
   * Procedimiento Operativo Estándar (`SOP-LOG-004`) completo (Fase 3).
   * Plantillas de comunicación para contingencias (Fase 5).
   * Anexo con el Protocolo de Devoluciones del reto (Fase 7).
2. **Archivo de Excel (`Checklist_Inspeccion_Rampa.xlsx`):**
   * **Pestaña `Inspeccion_Transporte`:** Tabla de inspección en rampa pegada directamente desde el chat (Fase 6).
   * **Pestaña `Reto_Checklist_Devoluciones`:** Tabla de control de mermas y devoluciones del reto autónomo (Fase 7).

# Uso de Copilot para revisar, mejorar y generar borradores de documentos clave, reduciendo retrabajos y errores operativos

## Metadatos

| Atributo | Detalle |
|---|---|
| **Duración estimada** | 96 minutos |
| **Complejidad** | Alta |
| **Nivel Bloom** | Crear (Create) |
| **Módulo** | Módulo 3 — Generación y Optimización de Documentos de Suministros con Copilot |
| **Laboratorio** | 03-00-01 |
| **Modalidad** | Individual con revisión grupal al cierre |

---

## Descripción General

En este laboratorio aplicarás de forma integral las capacidades de Microsoft 365 Copilot para generar, revisar y optimizar documentos clave del área de Suministros, incluyendo especificaciones técnicas de compra, solicitudes de cotización (RFQ), contratos marco y comunicaciones logísticas en Outlook. Trabajarás con un portafolio de cuatro documentos de práctica que contienen errores deliberados, omisiones y ambigüedades comunes del entorno operativo real. Al finalizar, habrás construido un flujo de trabajo documentado y una biblioteca de prompts reutilizables que tu equipo podrá adoptar de inmediato para reducir los ciclos de retrabajo en la elaboración de documentos de suministros.

---

## Objetivos de Aprendizaje

Al completar este laboratorio, serás capaz de:

- [ ] **Generar** borradores completos de documentos clave de suministros (RFQ, especificación técnica, resumen ejecutivo) utilizando prompts estructurados de cinco componentes en Copilot en Word.
- [ ] **Revisar y mejorar** documentos existentes con errores operativos, ambigüedades y cláusulas faltantes empleando Copilot como asistente de revisión crítica.
- [ ] **Optimizar** comunicaciones logísticas en Outlook con Copilot, ajustando tono, claridad y completitud de correos de seguimiento, notificación de incidencias y confirmación de pedidos.
- [ ] **Diseñar y documentar** un flujo de trabajo estándar para la creación y revisión de documentos de suministros asistida por Copilot, incluyendo una biblioteca de prompts reutilizables.

---

## Prerrequisitos

### Conocimientos Previos

| Área | Nivel requerido |
|---|---|
| Uso de Microsoft 365 Copilot (conceptos básicos de prompting) | Intermedio — haber completado Módulos 1 y 2, o equivalente |
| Tipos de documentos en el proceso de compras (RFQ, OC, especificaciones técnicas, contratos marco) | Básico — conocimiento conceptual suficiente |
| Redacción de documentos técnicos y comunicaciones formales en suministros | Básico |
| Microsoft Word (edición, estilos, control de cambios) | Básico |
| Microsoft Outlook (redacción y gestión de correos corporativos) | Básico |

### Acceso y Permisos Requeridos

| Recurso | Estado requerido |
|---|---|
| Cuenta corporativa de Microsoft 365 con licencia **Copilot activa** | ✅ Verificado por TI antes del laboratorio |
| Acceso a **OneDrive for Business** con permiso de escritura | ✅ Requerido |
| Acceso a **Microsoft Word** (versión 2406 o posterior, canal actual) | ✅ Requerido |
| Acceso a **Microsoft Outlook** (versión 2406 o posterior, o Outlook Web) | ✅ Requerido |
| Archivos de práctica del Módulo 3 descargados y guardados en OneDrive | ✅ Requerido — ver Sección de Entorno |

> ⚠️ **RECORDATORIO CRÍTICO DE PRIVACIDAD:** Durante todo el laboratorio, utiliza **únicamente los archivos de práctica proporcionados**. No ingreses datos reales de proveedores, precios contractuales ni información financiera sensible de la organización en Copilot.

---

## Entorno del Laboratorio

### Hardware Recomendado

| Componente | Mínimo | Recomendado |
|---|---|---|
| Procesador | Intel Core i5 8ª gen / AMD Ryzen 5 | Intel Core i7 / AMD Ryzen 7 |
| RAM | 8 GB | 16 GB |
| Almacenamiento disponible | 10 GB libres | 20 GB libres |
| Conexión a internet | 10 Mbps estable | 25 Mbps o superior |
| Resolución de pantalla | 1366 × 768 | 1920 × 1080 |

### Software Requerido

| Aplicación | Versión mínima | Verificación |
|---|---|---|
| Microsoft Word | 2406 (Microsoft 365 Apps) | Archivo → Cuenta → Acerca de Word |
| Microsoft Outlook | 2406 (Microsoft 365 Apps) o Outlook Web | Archivo → Cuenta de Office |
| OneDrive for Business | Versión en la nube (siempre actualizada) | Icono en bandeja del sistema — estado "Sincronizado" |
| Microsoft Edge o Chrome | Edge 120+ / Chrome 120+ | Menú → Ayuda → Acerca de |
| Copilot en Microsoft 365 | Licencia activa en el tenant | copilot.microsoft.com — debe cargar sin error de acceso |

### Preparación del Entorno — Instrucciones de Configuración Inicial

Ejecuta los siguientes pasos **antes de iniciar el laboratorio**. Tiempo estimado: 10 minutos.

**1. Verificar licencia de Copilot activa**

Abre tu navegador y navega a:
```
https://copilot.microsoft.com
```
Inicia sesión con tu cuenta corporativa. Si ves la interfaz de chat de Copilot sin mensajes de error de licencia, tu acceso está activo. Si aparece un mensaje de "licencia no disponible", notifica al instructor **antes de continuar**.

**2. Verificar que OneDrive for Business esté sincronizado**

En la barra de tareas de Windows, localiza el ícono de la nube de OneDrive. Debe mostrar estado "Actualizado" (ícono azul sin señales de error). Si no está sincronizado:
```
Click derecho en ícono OneDrive → Configuración → Cuenta → Verificar sesión activa
```

**3. Descargar y ubicar los archivos de práctica en OneDrive**

El instructor habrá compartido los archivos de práctica vía SharePoint o correo. Guárdalos en la siguiente ruta dentro de tu OneDrive for Business:
```
OneDrive - [NombreEmpresa] / Cursos / M365Copilot / Modulo3 /
```
Los archivos requeridos son:

| Archivo | Descripción |
|---|---|
| `M3_Practica_01_Especificacion_Tecnica_INCOMPLETA.docx` | Especificación técnica con secciones faltantes |
| `M3_Practica_02_RFQ_CON_ERRORES.docx` | RFQ con inconsistencias y cláusulas ambiguas |
| `M3_Practica_03_Contrato_Marco_REVISION.docx` | Contrato marco que requiere revisión y mejoras |
| `M3_Practica_04_Cadena_Correos_Logistica.msg` | Cadena de correos con problemas de tono y completitud |
| `M3_Plantilla_Flujo_Trabajo_Copilot.docx` | Plantilla en blanco para el entregable final |

> ⚠️ **IMPORTANTE:** Todos los archivos `.docx` deben abrirse directamente desde OneDrive (no desde el disco local) para que Copilot en Word funcione correctamente. Verifica que la barra de título de Word muestre el nombre del archivo seguido de "OneDrive" o "SharePoint".

**4. Abrir las aplicaciones necesarias**

Abre y mantén disponibles en tu barra de tareas:
- Microsoft Word (con `M3_Practica_01_Especificacion_Tecnica_INCOMPLETA.docx` cargado desde OneDrive)
- Microsoft Outlook (o Outlook Web en una pestaña del navegador)
- Una pestaña del navegador con `copilot.microsoft.com` iniciado

---

## Instrucciones Paso a Paso

> 📋 **Nota para el participante:** Este laboratorio se divide en **cuatro bloques** de trabajo. Cada bloque tiene un tiempo estimado. Administra tu tiempo según las indicaciones. Copilot puede generar respuestas diferentes en cada sesión — esto es normal y esperado. Evalúa la **calidad del proceso y el criterio aplicado**, no la coincidencia exacta con un resultado esperado.

---

### Bloque 1: Generación de un Documento desde Cero — Especificación Técnica de Compra
**Tiempo estimado: 22 minutos**

---

#### Paso 1.1 — Analizar el documento incompleto de referencia

**Objetivo:** Identificar qué secciones y elementos faltan en la especificación técnica de práctica antes de usar Copilot para completarla.

**Instrucciones:**

1. Abre `M3_Practica_01_Especificacion_Tecnica_INCOMPLETA.docx` desde tu OneDrive. Verifica que la barra de título confirme que está en la nube.

2. Lee el documento completo. Identifica y anota en papel o en un documento de notas las siguientes deficiencias:
   - Secciones presentes pero con contenido incompleto o marcadas con `[COMPLETAR]`
   - Secciones que debería tener una especificación técnica estándar y que **no existen** en el documento
   - Datos técnicos que parecen inconsistentes o contradictorios

3. Completa la siguiente tabla de análisis (puedes hacerlo en papel o en un documento aparte):

   | Sección | Estado | Observación |
   |---|---|---|
   | Objeto de la compra | | |
   | Especificaciones técnicas del material | | |
   | Normas y estándares aplicables | | |
   | Criterios de aceptación y rechazo | | |
   | Condiciones de embalaje y transporte | | |
   | Documentación requerida al proveedor | | |
   | Vigencia de la especificación | | |

**Resultado Esperado:** Una tabla de análisis con al menos 4 deficiencias identificadas en el documento de práctica. Este análisis será el insumo para el prompt de Copilot en el siguiente paso.

**Verificación:** Compara tu análisis con el de un compañero cercano. ¿Identificaron las mismas deficiencias? ¿Hay alguna que uno vio y el otro no? El instructor puede pedir 2–3 participantes que compartan sus hallazgos en voz alta.

---

#### Paso 1.2 — Generar el borrador completo con Copilot en Word

**Objetivo:** Usar Copilot en Word para completar y enriquecer la especificación técnica, aplicando la estructura de prompt de cinco componentes aprendida en la Lección 3.1.

**Instrucciones:**

1. Con el archivo `M3_Practica_01_Especificacion_Tecnica_INCOMPLETA.docx` abierto en Word, localiza el panel de **Copilot** en la cinta de opciones:
   ```
   Pestaña Inicio → Grupo "Copilot" → Botón "Copilot"
   ```
   Si no aparece en la cinta, usa el atajo:
   ```
   Alt + I  (o busca "Copilot" en la barra de búsqueda de Word)
   ```

2. En el panel de Copilot que se abre a la derecha, ingresa el siguiente prompt. **Personaliza los campos entre corchetes** con la información del documento de práctica que analizaste:

   ```text
   Actúa como especialista senior en adquisiciones industriales con
   experiencia en documentación técnica de compras.

   Tengo una especificación técnica de compra incompleta para
   [PRODUCTO DEL DOCUMENTO DE PRÁCTICA]. Necesito que la completes
   y mejores con el siguiente criterio:

   1. Completa todas las secciones marcadas con [COMPLETAR] usando
      lenguaje técnico preciso y formal en español.
   2. Agrega las siguientes secciones que faltan:
      - Criterios de aceptación y rechazo con parámetros medibles
      - Documentación técnica requerida al proveedor (certificados,
        fichas técnicas, pruebas de calidad)
      - Cláusula de vigencia y control de cambios del documento
   3. Verifica que las especificaciones técnicas sean coherentes
      entre sí y no presenten contradicciones.
   4. Usa numeración jerárquica (1., 1.1, 1.2, 2., etc.) en todo
      el documento.
   5. Tono: técnico, formal, sin ambigüedades.

   El documento completo debe poder entregarse directamente a un
   proveedor sin requerir aclaraciones adicionales.
   ```

3. Presiona **Enter** y espera la respuesta de Copilot (10–20 segundos aproximadamente).

4. Revisa el borrador generado. Copilot puede presentar el contenido como texto sugerido directamente en el documento o como respuesta en el panel. Si presenta opciones de "Insertar" o "Reemplazar", selecciona la opción más apropiada según el contexto.

5. Si el resultado requiere ajustes, ingresa un prompt de refinamiento. Por ejemplo:
   ```text
   El criterio de aceptación que generaste es demasiado genérico.
   Hazlo más específico con tolerancias numéricas para las
   dimensiones y propiedades mecánicas del material.
   ```

6. Cuando estés satisfecho con el borrador, guarda el archivo con un nuevo nombre:
   ```
   M3_Practica_01_Especificacion_Tecnica_COMPLETADA_[TuNombre].docx
   ```
   Asegúrate de guardarlo en la misma carpeta de OneDrive.

**Resultado Esperado:** Un documento de especificación técnica completo, con todas las secciones cubiertas, numeración jerárquica aplicada y lenguaje técnico preciso. El documento debe ser legible y coherente de principio a fin, sin secciones marcadas como `[COMPLETAR]`.

**Verificación:**
- Abre el documento completado y usa **Ctrl + F** para buscar `[COMPLETAR]`. El resultado debe ser **cero coincidencias**.
- Verifica que el documento tenga al menos las 7 secciones de la tabla del Paso 1.1 cubiertas.
- Lee en voz alta (internamente) la sección de "Criterios de aceptación y rechazo" — ¿contiene parámetros medibles y objetivos? Si es vaga o subjetiva, itera el prompt.

---

### Bloque 2: Revisión y Mejora de Documentos Existentes con Errores
**Tiempo estimado: 28 minutos**

---

#### Paso 2.1 — Auditar el RFQ con errores usando Copilot como revisor crítico

**Objetivo:** Usar Copilot para identificar sistemáticamente errores, omisiones y ambigüedades en un borrador de RFQ deficiente, simulando una revisión de calidad documental.

**Instrucciones:**

1. Abre `M3_Practica_02_RFQ_CON_ERRORES.docx` desde tu OneDrive.

2. **Sin leer el documento completo todavía**, ve directamente al panel de Copilot en Word y usa el siguiente prompt de auditoría:

   ```text
   Actúa como auditor de documentación de compras con criterio
   estricto. Revisa este documento RFQ (Request for Quotation)
   completo y genera un reporte de hallazgos estructurado con:

   SECCIÓN A — ERRORES CRÍTICOS:
   Lista todos los errores que podrían generar disputas legales,
   malentendidos comerciales o cotizaciones incomparables entre
   proveedores. Incluye el número de sección donde aparece cada
   error.

   SECCIÓN B — OMISIONES IMPORTANTES:
   Lista las secciones o cláusulas que un RFQ profesional debe
   incluir y que están ausentes en este documento.

   SECCIÓN C — AMBIGÜEDADES DE REDACCIÓN:
   Identifica frases, términos o condiciones que son imprecisas
   o que diferentes proveedores podrían interpretar de manera
   distinta.

   SECCIÓN D — RECOMENDACIONES DE MEJORA:
   Para cada hallazgo en las secciones anteriores, proporciona
   una recomendación concreta de corrección.

   Formato: usa viñetas y numeración. Sé específico y directo.
   ```

3. Espera la respuesta de Copilot y léela con atención. **No cierres el panel.**

4. En un documento de notas separado (o en papel), registra los hallazgos más críticos identificados por Copilot. Clasifícalos por nivel de impacto:
   - 🔴 **Crítico** — Podría invalidar el proceso de cotización o generar disputas
   - 🟡 **Importante** — Podría causar confusión o cotizaciones no comparables
   - 🟢 **Mejora** — Elevaría la calidad del documento pero no es bloqueante

5. Ahora lee el documento RFQ manualmente. ¿Identificas algún error que Copilot **no** detectó? Anótalo. Este ejercicio es importante: Copilot es un asistente, no un reemplazante del criterio profesional.

**Resultado Esperado:** Un reporte de auditoría generado por Copilot con al menos 8–10 hallazgos distribuidos en las cuatro secciones, más tus anotaciones personales de revisión manual.

**Verificación:** Compara tu clasificación de hallazgos (crítico/importante/mejora) con la de un compañero. ¿Coinciden en los elementos críticos? Las discrepancias son oportunidades de aprendizaje — discútelas brevemente.

---

#### Paso 2.2 — Reescribir el RFQ corregido con Copilot

**Objetivo:** Usar Copilot para generar una versión corregida y mejorada del RFQ, incorporando todos los hallazgos del paso anterior.

**Instrucciones:**

1. Continuando con `M3_Practica_02_RFQ_CON_ERRORES.docx` abierto y el panel de Copilot activo, ingresa el siguiente prompt de corrección:

   ```text
   Basándote en el reporte de auditoría que generaste, ahora
   reescribe este RFQ completo con todas las correcciones
   aplicadas. Asegúrate de:

   1. Corregir todos los errores críticos identificados en la
      Sección A del reporte.
   2. Agregar todas las secciones omitidas identificadas en la
      Sección B.
   3. Reemplazar todas las frases ambiguas con lenguaje preciso
      y medible.
   4. Mantener la estructura estándar de un RFQ profesional:
      - Encabezado con número de RFQ, fecha y vigencia
      - Objeto de la cotización
      - Especificaciones técnicas detalladas
      - Condiciones comerciales (precio, pago, entrega, Incoterm)
      - Criterios de evaluación de propuestas
      - Penalizaciones por incumplimiento
      - Instrucciones de respuesta (formato, fecha límite, contacto)
      - Términos y condiciones generales
   5. Tono: formal, claro, sin ambigüedades.
   6. Formato: numeración jerárquica, tablas donde aplique.
   ```

2. Revisa el documento generado. Usa **Control de Cambios** en Word para comparar la versión original con la nueva:
   ```
   Pestaña Revisar → Grupo "Seguimiento" → "Mostrar marcas" → 
   Selecciona "Todas las marcas"
   ```

3. Acepta o rechaza los cambios propuestos según tu criterio profesional. Para aceptar todos:
   ```
   Pestaña Revisar → "Aceptar" → "Aceptar todos los cambios"
   ```
   Para revisar cambio por cambio:
   ```
   Pestaña Revisar → "Siguiente" → "Aceptar" o "Rechazar"
   ```

4. Guarda el documento corregido como:
   ```
   M3_Practica_02_RFQ_CORREGIDO_[TuNombre].docx
   ```
   en tu carpeta de OneDrive del Módulo 3.

**Resultado Esperado:** Un RFQ corregido y completo que no contenga ninguno de los errores críticos identificados en la auditoría. El documento debe ser profesionalmente presentable y listo para enviarse a proveedores.

**Verificación:**
- Ejecuta nuevamente el prompt de auditoría del Paso 2.1 sobre el documento **corregido**. La Sección A (Errores Críticos) debe estar vacía o tener como máximo 1–2 observaciones menores.
- Verifica que el documento tenga las 8 secciones estructurales listadas en el prompt de corrección.

---

#### Paso 2.3 — Revisar el Contrato Marco con Copilot

**Objetivo:** Aplicar Copilot para revisar un contrato marco de proveedor, identificando cláusulas problemáticas y agregando elementos faltantes estándar.

**Instrucciones:**

1. Abre `M3_Practica_03_Contrato_Marco_REVISION.docx` desde OneDrive.

2. En el panel de Copilot en Word, ingresa el siguiente prompt de revisión contractual:

   ```text
   Actúa como especialista en contratos de suministro. Revisa
   este contrato marco de proveedor y realiza las siguientes
   acciones:

   1. SIMPLIFICACIÓN: Identifica las tres cláusulas más complejas
      o difíciles de entender y proporciona una versión simplificada
      de cada una, sin perder precisión legal ni comercial.

   2. RIESGOS: Señala cualquier cláusula que represente un riesgo
      desproporcionado para el comprador (nuestra empresa) o que
      esté redactada de manera favorable solo para el proveedor.

   3. FALTANTES: Verifica si el contrato incluye las siguientes
      cláusulas y, si no existen, redacta una versión estándar
      para cada una:
      - Cláusula de fuerza mayor
      - Cláusula de confidencialidad y protección de datos
      - Cláusula de resolución de disputas (arbitraje o mediación)
      - Cláusula de modificaciones y adendas

   4. FORMATO: Verifica que la numeración de cláusulas sea
      jerárquica y consistente. Señala cualquier inconsistencia.

   Presenta los resultados en secciones claramente separadas
   con el número de cláusula afectada en cada hallazgo.
   ```

3. Revisa los resultados. Para las cláusulas faltantes que Copilot haya redactado, evalúa si el lenguaje es apropiado para el contexto de tu organización.

4. Si necesitas ajustar el tono o la especificidad de alguna cláusula generada, usa un prompt de refinamiento:
   ```text
   La cláusula de fuerza mayor que generaste es demasiado amplia.
   Limítala a eventos no previsibles e irresistibles, y agrega
   un requisito de notificación dentro de 48 horas del evento.
   Incluye también una cláusula de terminación si la fuerza mayor
   se extiende por más de 30 días calendario.
   ```

5. Guarda el documento revisado como:
   ```
   M3_Practica_03_Contrato_Marco_REVISADO_[TuNombre].docx
   ```

**Resultado Esperado:** Un análisis de revisión del contrato marco con: identificación de cláusulas complejas con versiones simplificadas, señalamiento de al menos 2 riesgos para el comprador, y redacción de las cláusulas faltantes identificadas.

**Verificación:** ¿Las cláusulas generadas por Copilot son coherentes con el resto del contrato en términos de numeración, tono y terminología? Si hay inconsistencias, usa Copilot para armonizarlas con un prompt adicional.

---

### Bloque 3: Optimización de Comunicaciones Logísticas en Outlook
**Tiempo estimado: 22 minutos**

---

#### Paso 3.1 — Analizar y mejorar una cadena de correos logísticos con Copilot en Outlook

**Objetivo:** Usar Copilot en Outlook para analizar una cadena de correos con problemas de tono y completitud, y generar versiones mejoradas de los mensajes clave.

**Instrucciones:**

1. Abre Microsoft Outlook. Si usas Outlook Web, navega a:
   ```
   https://outlook.office.com
   ```

2. El instructor habrá compartido (o importado) el archivo `M3_Practica_04_Cadena_Correos_Logistica.msg` en tu bandeja de entrada o en una carpeta de práctica. Ábrelo y lee la cadena completa de correos.

3. Identifica los siguientes problemas en la cadena (anótalos):
   - Correos con tono inapropiado (demasiado informal, agresivo o pasivo-agresivo)
   - Mensajes que omiten información crítica (número de orden, fechas, responsables)
   - Correos donde el llamado a la acción no es claro
   - Mensajes que escalan innecesariamente el conflicto

4. Para el correo más problemático de la cadena, usa **Copilot en Outlook** para mejorarlo. Localiza el botón de Copilot en la barra de herramientas de redacción:
   ```
   Nuevo correo → Botón "Copilot" en la barra de herramientas
   (ícono de Copilot / estrella de colores)
   ```

5. En el panel de Copilot de Outlook, usa el siguiente prompt para generar un correo mejorado de notificación de incumplimiento:

   ```text
   Redacta un correo electrónico formal de notificación de
   retraso en entrega con los siguientes datos:

   Para: Ing. Carlos Mendoza, Gerente de Ventas
   Empresa proveedora: Suministros Industriales del Centro S.A.
   De: [Tu nombre], Especialista en Suministros

   Contexto:
   - Orden de Compra: OC-2025-1134
   - Producto: 150 piezas de brida de acero inoxidable 3" clase 150
   - Fecha de entrega acordada: 18 de abril de 2025
   - Fecha actual: 25 de abril de 2025 (7 días de retraso)
   - El retraso está causando paros parciales en la línea de
     ensamble 2 de nuestra planta

   Requisitos del correo:
   - Tono: formal y firme, pero no agresivo; preservar la
     relación comercial
   - Solicitar confirmación de nueva fecha de entrega en un
     plazo máximo de 24 horas hábiles
   - Mencionar que según la cláusula 9.3 del contrato marco
     vigente, aplican penalizaciones de 0.5% del valor de la
     orden por cada día hábil de retraso
   - Reconocer brevemente el historial positivo del proveedor
     antes de abordar el incumplimiento
   - Incluir asunto del correo, saludo, cuerpo y cierre formal
   - Extensión: máximo 250 palabras
   ```

6. Revisa el correo generado. Evalúa:
   - ¿El tono es apropiado para la relación con este proveedor?
   - ¿Están todos los datos operativos incluidos (número de OC, fechas, producto)?
   - ¿El llamado a la acción es claro y con plazo definido?
   - ¿La mención de penalizaciones está formulada de manera que no sea amenazante sino informativa?

7. Si requiere ajustes, usa un prompt de refinamiento. Ejemplos:
   ```text
   El tono del segundo párrafo es demasiado confrontacional.
   Suavízalo manteniendo la firmeza sobre el plazo de 24 horas.
   ```
   ```text
   Agrega una frase de apertura que reconozca que el proveedor
   normalmente cumple sus compromisos, antes de abordar el
   retraso actual.
   ```

**Resultado Esperado:** Un correo de notificación de retraso profesional, con todos los datos operativos incluidos, tono apropiado, llamado a la acción claro y referencia a cláusulas contractuales. El correo debe poder enviarse sin modificaciones adicionales.

**Verificación:** Intercambia el correo generado con un compañero. Que tu compañero lo evalúe usando esta rúbrica rápida (1–5 puntos cada criterio):
- Tono apropiado (formal, firme, no agresivo)
- Completitud de información operativa
- Claridad del llamado a la acción
- Profesionalismo general
- Longitud apropiada (≤ 250 palabras)

**Puntaje mínimo esperado:** 18/25 puntos.

---

#### Paso 3.2 — Generar correos de seguimiento y confirmación con Copilot

**Objetivo:** Crear dos tipos adicionales de comunicaciones logísticas frecuentes usando Copilot en Outlook, construyendo una mini-biblioteca de plantillas de correo.

**Instrucciones:**

1. Usando el panel de Copilot en Outlook, genera un **correo de confirmación de recepción de pedido** con el siguiente prompt:

   ```text
   Redacta un correo formal de confirmación de recepción de
   mercancía para enviar al proveedor:

   Proveedor: Plásticos y Polímeros del Bajío S.A. de C.V.
   Contacto: Lic. Ana Guerrero, Coordinadora de Logística
   Número de OC: OC-2025-0923
   Producto recibido: Película stretch transparente calibre 80,
   1,200 rollos
   Fecha de recepción: hoy
   Estado: recepción conforme — sin diferencias en cantidad ni
   daños visibles
   Próximo paso: factura debe emitirse a nombre de [Empresa
   Compradora] con RFC [RFC-EJEMPLO-001] en un plazo de 5 días

   Tono: cordial y profesional. Extensión: máximo 150 palabras.
   Incluir asunto del correo.
   ```

2. Genera un segundo correo: **notificación de rechazo parcial de entrega** con este prompt:

   ```text
   Redacta un correo formal de rechazo parcial de entrega:

   Proveedor: Metales y Aleaciones del Norte S.A.
   Contacto: Ing. Jorge Villarreal, Gerente de Operaciones
   OC: OC-2025-1089
   Producto: Tubo de acero al carbono 2" cédula 40, 500 metros
   Entrega recibida: 500 metros (cantidad correcta)
   Motivo de rechazo parcial: 85 metros presentan marcas de
   corrosión superficial que no cumplen con la especificación
   técnica ET-MAT-2025-003
   Acción requerida: reposición de los 85 metros rechazados en
   un plazo máximo de 10 días hábiles, sin costo adicional
   Evidencia: se adjuntan 6 fotografías del material rechazado

   Tono: formal y objetivo, sin emociones. Extensión: máximo
   200 palabras. Incluir asunto del correo.
   ```

3. Guarda los tres correos generados (notificación de retraso del Paso 3.1 + confirmación de recepción + rechazo parcial) en un documento Word como referencia:
   ```
   M3_Biblioteca_Correos_Logisticos_[TuNombre].docx
   ```
   Guárdalo en tu carpeta de OneDrive del Módulo 3.

4. Para cada correo, agrega una nota breve (2–3 líneas) explicando:
   - En qué situación se usa este tipo de correo
   - Qué elementos del prompt son los más críticos para obtener el tono correcto
   - Qué ajustes hiciste durante la iteración (si los hubo)

**Resultado Esperado:** Una biblioteca de tres correos logísticos profesionales, listos para usar como plantillas, con notas de uso y aprendizajes de prompting documentados.

**Verificación:** Lee los tres correos en secuencia. ¿Cada uno tiene un tono y propósito claramente diferenciado? ¿Ninguno omite el número de OC, el producto o el llamado a la acción? Si alguno falla en estos criterios básicos, itera el prompt correspondiente.

---

### Bloque 4: Diseño del Flujo de Trabajo Estándar con Copilot
**Tiempo estimado: 24 minutos**

---

#### Paso 4.1 — Documentar el flujo de trabajo para creación de documentos asistida por Copilot

**Objetivo:** Crear un documento de flujo de trabajo estándar que el equipo de suministros pueda adoptar para la generación y revisión de documentos con Copilot, consolidando los aprendizajes de los bloques anteriores.

**Instrucciones:**

1. Abre `M3_Plantilla_Flujo_Trabajo_Copilot.docx` desde tu OneDrive.

2. Usa Copilot en Word para generar el contenido base del flujo de trabajo con el siguiente prompt:

   ```text
   Actúa como consultor de mejora de procesos especializado en
   gestión de suministros y herramientas de inteligencia artificial.

   Genera el contenido para un documento de "Flujo de Trabajo
   Estándar para la Creación y Revisión de Documentos de
   Suministros con Microsoft 365 Copilot" con las siguientes
   secciones:

   1. PROPÓSITO Y ALCANCE
      Describe el objetivo del flujo de trabajo y los tipos de
      documentos que cubre (RFQ, especificaciones técnicas,
      contratos marco, comunicaciones logísticas).

   2. ROLES Y RESPONSABILIDADES
      Define los roles involucrados: Especialista en Suministros
      (generador del prompt y revisor técnico), Supervisor de
      Compras (aprobador final), Área Legal (revisión de contratos).

   3. FLUJO DE TRABAJO PASO A PASO
      Describe un proceso de 6 pasos para la generación de
      cualquier documento de suministros con Copilot:
      Paso 1: Definir el tipo y propósito del documento
      Paso 2: Recopilar el contexto operativo necesario
      Paso 3: Construir el prompt estructurado (5 componentes)
      Paso 4: Generar y revisar el borrador con Copilot
      Paso 5: Iterar y refinar según criterio profesional
      Paso 6: Aprobar y archivar el documento final

   4. ESTRUCTURA DEL PROMPT ESTÁNDAR (5 COMPONENTES)
      Explica cada componente con un ejemplo aplicado a suministros:
      - Rol asignado
      - Tipo de documento
      - Contexto operativo
      - Restricciones y requisitos
      - Formato de salida

   5. CRITERIOS DE CALIDAD DEL DOCUMENTO FINAL
      Lista 8 criterios verificables que debe cumplir cualquier
      documento generado con Copilot antes de su aprobación.

   6. ADVERTENCIAS Y LIMITACIONES
      Incluye 4 advertencias sobre el uso responsable de Copilot
      en documentación de suministros (privacidad, verificación
      de datos, criterio profesional, variabilidad de respuestas).

   Formato: usa numeración jerárquica, viñetas y tablas donde
   aplique. Tono: profesional, claro y directo. El documento
   debe ser práctico y usable por el equipo desde el primer día.
   ```

3. Revisa el contenido generado e **incorpora tus aprendizajes personales** de los Bloques 1, 2 y 3 de este laboratorio. Específicamente:
   - En la Sección 3 (Flujo de trabajo), agrega notas basadas en lo que funcionó y lo que requirió iteración durante tus ejercicios.
   - En la Sección 5 (Criterios de calidad), asegúrate de que los criterios reflejen los errores que encontraste en los documentos de práctica.

4. Guarda el documento como:
   ```
   M3_Flujo_Trabajo_Copilot_Suministros_[TuNombre].docx
   ```
   en tu carpeta de OneDrive del Módulo 3.

**Resultado Esperado:** Un documento de flujo de trabajo estándar completo, con las 6 secciones cubiertas, personalizado con tus aprendizajes del laboratorio. El documento debe tener entre 600 y 1,000 palabras de contenido útil.

**Verificación:** ¿El documento es autoexplicativo? Pide a un compañero que no haya participado en el mismo grupo que lea la Sección 3 (Flujo de trabajo) y te diga si podría seguirlo sin tu ayuda. Si necesita explicaciones adicionales, el documento requiere más detalle.

---

#### Paso 4.2 — Construir la Biblioteca de Prompts Reutilizables del Equipo

**Objetivo:** Consolidar todos los prompts utilizados durante el laboratorio en una biblioteca de referencia estructurada, lista para ser compartida con el equipo de suministros.

**Instrucciones:**

1. Abre un nuevo documento Word en blanco desde OneDrive y nómbralo:
   ```
   M3_Biblioteca_Prompts_Suministros_[TuNombre].docx
   ```

2. Usa Copilot en Word para generar la estructura base de la biblioteca con el siguiente prompt:

   ```text
   Crea la estructura de una "Biblioteca de Prompts para
   Documentos de Suministros con Microsoft 365 Copilot".
   Genera una tabla maestra con las siguientes columnas:

   | ID | Tipo de Documento | Situación de Uso | Prompt Base |
   Variables Requeridas | Nivel de Detalle | Notas |

   Pre-llena la tabla con las siguientes categorías de documentos,
   dejando el campo "Prompt Base" con la instrucción
   "[COMPLETAR CON PROMPT DEL EQUIPO]":

   1. Solicitud de Cotización (RFQ) — Compra estándar
   2. Solicitud de Cotización (RFQ) — Compra urgente
   3. Especificación Técnica de Material
   4. Notificación de Incumplimiento de Entrega
   5. Confirmación de Recepción Conforme
   6. Rechazo Parcial de Entrega
   7. Solicitud de Prórroga a Proveedor
   8. Escalamiento de Incidencia a Gerencia
   9. Resumen Ejecutivo de Evaluación de Proveedor
   10. Adenda a Contrato Marco

   Después de la tabla, agrega una sección de "Instrucciones de
   Uso" con 5 reglas para usar esta biblioteca correctamente.
   ```

3. Ahora **completa manualmente** los campos "Prompt Base" para al menos **5 de las 10 categorías**, usando los prompts que desarrollaste y refinaste durante los Bloques 1, 2 y 3 de este laboratorio. Copia y pega los prompts más efectivos que utilizaste, asegurándote de:
   - Reemplazar los datos específicos del ejercicio con **variables entre corchetes** (ej: `[NOMBRE_PROVEEDOR]`, `[NUMERO_OC]`, `[PRODUCTO]`)
   - Incluir en la columna "Variables Requeridas" la lista de datos que deben sustituirse antes de usar el prompt
   - Agregar en "Notas" cualquier aprendizaje de iteración relevante

4. Guarda el documento en tu carpeta de OneDrive del Módulo 3.

**Resultado Esperado:** Una biblioteca de prompts con estructura de tabla, al menos 5 prompts base completos con variables identificadas, y una sección de instrucciones de uso. Este documento debe ser inmediatamente útil para el equipo.

**Verificación:** Toma uno de los prompts de tu biblioteca, sustituye las variables con datos ficticios coherentes, y pruébalo en Copilot. ¿Genera un documento de calidad comparable al que obtuviste durante el laboratorio? Si no, refina el prompt base en la biblioteca.

---

## Validación y Pruebas Finales

Al completar los cuatro bloques, verifica que hayas producido los siguientes entregables en tu carpeta de OneDrive (`OneDrive - [NombreEmpresa] / Cursos / M365Copilot / Modulo3 /`):

| # | Archivo | Criterio de Completitud |
|---|---|---|
| 1 | `M3_Practica_01_Especificacion_Tecnica_COMPLETADA_[TuNombre].docx` | Sin secciones `[COMPLETAR]`, numeración jerárquica, criterios de aceptación medibles |
| 2 | `M3_Practica_02_RFQ_CORREGIDO_[TuNombre].docx` | Sin errores críticos al re-auditar con Copilot, 8 secciones estructurales presentes |
| 3 | `M3_Practica_03_Contrato_Marco_REVISADO_[TuNombre].docx` | Cláusulas faltantes agregadas, riesgos señalados, numeración consistente |
| 4 | `M3_Biblioteca_Correos_Logisticos_[TuNombre].docx` | 3 correos logísticos con notas de uso y aprendizajes de prompting |
| 5 | `M3_Flujo_Trabajo_Copilot_Suministros_[TuNombre].docx` | 6 secciones completas, 600–1,000 palabras, personalizado con aprendizajes propios |
| 6 | `M3_Biblioteca_Prompts_Suministros_[TuNombre].docx` | Tabla de 10 categorías, mínimo 5 prompts base completos con variables identificadas |

**Prueba de validación final — Ronda de revisión cruzada (10 minutos):**

El instructor organizará pares de participantes. Cada participante deberá:

1. Compartir (vía OneDrive o Teams) su archivo `M3_Practica_02_RFQ_CORREGIDO_[TuNombre].docx` con su compañero asignado.
2. El compañero ejecutará el prompt de auditoría del Paso 2.1 sobre el RFQ recibido y compartirá los resultados.
3. Si la Sección A (Errores Críticos) del reporte de auditoría generado por Copilot está vacía o tiene máximo 1 observación menor, el documento pasa la validación.
4. Si hay más de 1 error crítico, el participante tiene 5 minutos adicionales para corregirlos.

---

## Solución de Problemas

### Problema 1: Copilot en Word no aparece en la cinta de opciones o no responde

**Síntoma:** El botón de Copilot no está visible en la pestaña "Inicio" de Word, o al hacer clic no abre el panel lateral. Alternativamente, el panel aparece pero muestra el mensaje "Copilot no está disponible en este momento".

**Causa probable:** El archivo no está guardado en OneDrive for Business (está en el disco local), la licencia de Copilot no está activa para la cuenta actual, o la versión de Word no es la 2406 o posterior del canal actual.

**Solución paso a paso:**

1. Verifica dónde está guardado el archivo. La barra de título de Word debe mostrar el nombre del archivo seguido de "OneDrive" o "SharePoint". Si no lo dice, guarda el archivo en OneDrive:
   ```
   Archivo → Guardar como → OneDrive - [NombreEmpresa] →
   Selecciona la carpeta del Módulo 3 → Guardar
   ```
2. Cierra y vuelve a abrir el archivo **desde OneDrive** (no desde "Documentos recientes" si el acceso directo apunta al disco local).
3. Verifica la versión de Word: `Archivo → Cuenta → Acerca de Word`. Debe mostrar versión 2406 o posterior. Si no, solicita al área de TI la actualización.
4. Verifica la licencia: `Archivo → Cuenta → Estado del producto`. Debe mostrar "Licencia activa" y la cuenta corporativa correcta. Si muestra una cuenta personal, cierra sesión y vuelve a iniciar con la cuenta corporativa.
5. Si el problema persiste, usa Copilot Chat directamente en `copilot.microsoft.com` para generar el contenido y luego cópialo manualmente a Word.

---

### Problema 2: Los borradores generados por Copilot son demasiado genéricos o no reflejan el contexto de suministros

**Síntoma:** Copilot genera texto que parece un documento de plantilla genérica, sin terminología específica de suministros, sin los datos del proveedor o producto incluidos en el prompt, o con un tono inadecuado (demasiado informal o excesivamente legal).

**Causa probable:** El prompt carece de suficiente contexto operativo específico, o no incluye el rol asignado y las restricciones de formato. También puede ocurrir cuando el prompt es muy corto o usa instrucciones vagas como "redacta un contrato" sin más detalles.

**Solución paso a paso:**

1. Revisa tu prompt contra la estructura de 5 componentes de la Lección 3.1:
   - ¿Asignaste un **rol específico** a Copilot? (ej: "Actúa como especialista en adquisiciones industriales")
   - ¿Especificaste el **tipo exacto de documento** con su nombre formal?
   - ¿Incluiste **datos operativos concretos** (nombres, números, fechas, cantidades)?
   - ¿Definiste **restricciones** (tono, extensión, cláusulas obligatorias)?
   - ¿Especificaste el **formato de salida** (secciones, tablas, numeración)?

2. Agrega más contexto al prompt. Por ejemplo, si el resultado fue genérico para una RFQ, añade:
   ```text
   Contexto adicional: esta RFQ es para una empresa manufacturera
   del sector automotriz en México. Los proveedores son empresas
   medianas nacionales. El lenguaje debe ser formal pero directo,
   sin tecnicismos legales excesivos. Incluye referencias a
   normativa mexicana de calidad donde aplique (NMX).
   ```

3. Si después de mejorar el prompt el resultado sigue siendo genérico, prueba dividir el documento en secciones y genera cada una con un prompt específico, en lugar de intentar generar todo el documento en un solo prompt.

4. Recuerda que Copilot puede generar respuestas diferentes en cada intento. Si un prompt bien construido produjo un resultado pobre, intenta ejecutarlo de nuevo sin cambios — el siguiente intento puede ser significativamente mejor.

---

## Limpieza del Entorno

Al finalizar el laboratorio, realiza las siguientes acciones de cierre:

1. **Verificar que todos los archivos estén guardados en OneDrive:**
   ```
   En cada documento Word abierto: Ctrl + S
   Verificar que la barra de título no muestre asterisco (*) de cambios no guardados
   ```

2. **Cerrar todos los documentos Word** que ya no necesites activos.

3. **Verificar sincronización de OneDrive:** El ícono de OneDrive en la bandeja del sistema debe mostrar "Actualizado" antes de cerrar sesión o apagar el equipo.

4. **Compartir los entregables con el instructor** (si se indica):
   El instructor puede solicitar que compartas la carpeta `Modulo3` de tu OneDrive:
   ```
   Abre OneDrive en el navegador → Navega a Cursos/M365Copilot/Modulo3 →
   Click derecho → Compartir → Ingresa el correo del instructor →
   Permiso: "Puede ver"
   ```

5. **Cerrar sesión de Copilot** si estás en una computadora compartida:
   ```
   copilot.microsoft.com → Ícono de perfil (esquina superior derecha) →
   "Cerrar sesión"
   ```

6. **No elimines** los archivos de práctica originales (`M3_Practica_0X_*`) — pueden ser necesarios para referencia en módulos posteriores.

---

## Resumen

### Lo que Aprendiste en Este Laboratorio

En este laboratorio de 96 minutos desarrollaste competencias avanzadas de nivel "Crear" (Bloom) para la generación y optimización de documentos de suministros con Microsoft 365 Copilot:

| Bloque | Habilidad Desarrollada | Entregable Producido |
|---|---|---|
| **Bloque 1** | Generación de documentos desde cero con prompts estructurados de 5 componentes | Especificación técnica completa y coherente |
| **Bloque 2** | Auditoría y corrección de documentos con errores usando Copilot como revisor crítico | RFQ corregido + Contrato marco revisado |
| **Bloque 3** | Optimización de comunicaciones logísticas en Outlook con tono y completitud apropiados | Biblioteca de 3 correos logísticos profesionales |
| **Bloque 4** | Diseño de flujo de trabajo estándar y biblioteca de prompts reutilizables | Flujo de trabajo documentado + Biblioteca de prompts |

### Principios Clave para Llevar a la Práctica

- **La calidad del prompt determina la calidad del documento.** Un prompt con los 5 componentes (rol, tipo, contexto, restricciones, formato) produce documentos utilizables de inmediato; un prompt vago produce texto que requiere reescritura extensa.
- **Copilot es el redactor; tú eres el responsable.** La precisión técnica, legal y comercial del documento final es responsabilidad del profesional de suministros, no de Copilot.
- **La iteración es el método, no el fallo.** Rara vez el primer borrador es el definitivo — el flujo generar → revisar → refinar → regenerar es el proceso correcto, no una señal de que algo salió mal.
- **Los prompts efectivos son activos del equipo.** Guardar y compartir los prompts que funcionan multiplica la productividad de todo el equipo, no solo de quien los desarrolló.
- **La variabilidad de Copilot es normal.** El mismo prompt puede generar respuestas diferentes en distintas sesiones — evalúa la calidad del resultado, no su coincidencia con una respuesta "correcta" única.

### Recursos de Referencia

| Recurso | URL |
|---|---|
| Documentación oficial de Microsoft 365 Copilot | https://learn.microsoft.com/es-es/copilot/microsoft-365/microsoft-365-copilot-overview |
| Biblioteca de prompts por función empresarial (Microsoft Adoption) | https://adoption.microsoft.com/es-es/copilot/ |
| Principios de ingeniería de prompts para usuarios de negocio | https://learn.microsoft.com/es-es/ai/playbook/technology-guidance/generative-ai/working-with-llms/prompt-engineering |
| Mejores prácticas en contratos y documentación de compras (CIPS) | https://www.cips.org/knowledge/procurement-topics-and-skills/contract-management/ |
| Estándares para documentación de adquisiciones (ISM) | https://www.ismworld.org/supply-management-news-and-reports/news-publications/inside-supply-management-magazine/ |

> 📌 **Próximo paso:** En la **Lección 3.2** aplicarás Copilot para identificar y mitigar errores operativos en documentos ya elaborados — inconsistencias en especificaciones técnicas, condiciones contractuales contradictorias — y para mejorar la efectividad de comunicaciones en situaciones de alta presión. Antes de continuar, practica generando al menos un documento adicional de tu área real usando los prompts de tu biblioteca, y documenta los ajustes que debiste hacer.

---

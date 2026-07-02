# Automatización de cotizaciones

## 1. Metadatos del Laboratorio

| Atributo | Detalle |
| :--- | :--- |
| **Duración** | 90 minutos (Guiado + Reto de Aplicación Autónoma de Alta Densidad) |
| **Complejidad** | Avanzada |
| **Audiencia** | Directores Comerciales, Gerentes de Operaciones, Analistas de Precios, Key Account Managers (KAM) y Personal de Backoffice Comercial |
| **Tecnologías** | Microsoft Copilot Chat (M365), Microsoft Excel y Microsoft Word |
| **Enfoque** | Configuración de un Copilot especializado en cotizaciones: desde la recepción de la solicitud hasta la generación de PDFs uniformes. Consulta automática de costos, reglas de negocio, cálculo de cubicaje logístico y despacho automatizado por correo. |

---

## 2. Descripción Corta

Este laboratorio práctico de 90 minutos entrena a los profesionales comerciales en el diseño de un flujo de trabajo de extremo a extremo automatizado con Microsoft Copilot para la gestión de ofertas económicas masivas. Los estudiantes aprenderán a estructurar costos base y simular márgenes en **Microsoft Excel**, aplicar reglas corporativas complejas (descuentos escalonados y recargos por cubicaje de transporte pesado) mediante la IA, redactar acuerdos de reserva técnica de stock, y estructurar correos de despacho en **Microsoft Word** diseñados bajo un estándar riguroso para su exportación a **PDFs uniformes**.

---

## 3. Objetivos del Laboratorio

Al finalizar este laboratorio, el estudiante será capaz de:
* **Estructurar simuladores de costeo comercial y cubicaje en Excel** configurando márgenes de contribución, precios de lista y empaque logístico por palé.
* **Orquestar a Copilot como un motor de cotizaciones avanzado**, aplicando políticas de descuento por volumen y penalizaciones por entrega fraccionada.
* **Redactar Acuerdos de Reserva Técnica de Stock en Word**, asegurando el bloqueo de inventario en fábrica para proyectos de gran envergadura.
* **Diseñar plantillas de propuestas comerciales y correos persuasivos en Word**, optimizando la velocidad de respuesta ante solicitudes de cotización (RFQs).
* **Configurar directrices estrictas para la exportación a PDFs uniformes**, garantizando que la documentación comercial no pierda el estándar visual corporativo.

---

## 4. Prerrequisitos

* Cuenta activa de **Microsoft 365** con acceso a **Copilot Chat**.
* Aplicación de **Microsoft Excel** abierta con un libro en blanco guardado como `Calculador_Costos_Cotizaciones.xlsx`.
* Aplicación de **Microsoft Word** abierta con un documento en blanco guardado como `Plantillas_Envio_Cotizacion.docx`.

---

## 5. Procedimiento Paso a Paso (Flujo de Automatización de Ofertas)

### Fase A: El Motor de Costeo y Márgenes Comerciales (Excel) 
Para que una cotización institucional sea rentable, el backend numérico debe estar perfectamente calculado. Crearemos la base analítica en Excel para que sirva de referencia en los cálculos de la IA.

1. En su libro de Excel, nombre la primera hoja como `Simulador de Costeo`.
2. Vaya al chat de **Copilot** e introduzca el siguiente prompt para estructurar su calculadora financiera:

```
Actúa como un Analista Financiero Comercial de la industria de acabados. Necesito crear una estructura de cálculo en Excel para determinar el Precio de Venta al Público (PVP) por metro cuadrado de 3 referencias premium de recubrimientos (Porcelanato Lítico, Cerámica Modular Urbana y Mosaico Hidráulico).

Por favor, devuélveme una tabla limpia para Excel con las fórmulas lógicas explicadas paso a paso en las columnas. La tabla debe incluir los siguientes encabezados de columna:
- **Producto**
- **Costo de Fabricación/Importación Base por m²** (Asígnale valores realistas entre $12 y $35 USD)
- **Margen de Utilidad Objetivo (%)** (Fíjalo en el 40% para todos)
- **Fórmula de Precio de Venta Sugerido** (Muestra matemáticamente cómo calcularlo: `Costo Base / (1 - Margen)`)
- **Precio de Venta Sugerido (PVP)** (Resultado del cálculo)
- **Costo de Desperdicio Estimado por Rotura en Instalación (5%)** (Fórmula: `PVP * 0.05`)
- **Precio Técnico Final con Mermas Incluidas** (Fórmula: `PVP + Costo de Desperdicio`)
```

3. Seleccione la tabla numérica generada por Copilot.
4. Cópiela (`Ctrl+C`), vaya a su archivo de **Excel**, posiciónese en la celda `A1` y péguela. 

---

### Fase B: Aplicación de Reglas de Negocio y Estructura de Cotización (Copilot) 
Entrenaremos a Copilot para que procese solicitudes de cotizaciones de clientes institucionales aplicando las políticas comerciales y de volumen de la empresa de recubrimientos.

1. Manteniendo el mismo hilo de conversación en **Copilot**, introduzca el siguiente prompt de procesamiento de reglas de negocio:

```
Actúa como un Sistema Experto de Cotizaciones de nuestra fábrica de recubrimientos. Acabamos de recibir una solicitud de un constructor para el proyecto "Torres del Horizonte" que requiere:
- **1,500 m² de Porcelanato Lítico**
- **800 m² de Cerámica Modular Urbana**

Nuestras reglas de negocio comerciales vigentes para este año 2026 son:
1. Si el volumen de un solo producto es mayor a 1,000 m², se aplica un descuento automático del 10% sobre el 'Precio Técnico Final con Mermas' calculado en la Fase A.
2. Si el volumen es menor a 1,000 m², se mantiene el precio de lista pleno.
3. Se debe agregar un cargo fijo logístico de transporte en obra de $450 USD si el pedido total supera los 2,000 m².

Tomando como base los precios finales que calculamos en la tabla de Excel de la Fase A, por favor realiza el cálculo matemático completo para esta orden y devuélveme el resumen ejecutivo de la cotización desglosado por: Subtotal por producto, Descuentos aplicados, Cargo logístico y **Valor Total Neto de la Oferta**.
```

2. Revise detalladamente los cálculos que Copilot arroja en la pantalla y verifique la exactitud del neto.

---

### Fase C: Cálculo de Cubicaje Logístico y Despacho de Carga (Excel) 
*(Nueva Tarea)* Una cotización masiva de pisos no está completa sin la viabilidad logística. Forzaremos a Copilot a calcular cuántos palés (pallets) y camiones se necesitan para transportar el peso de la orden, integrando esta información en el simulador.

1. En su libro de Excel, cree una segunda hoja llamada `Cubicaje Logístico`.
2. Vaya al chat de Copilot e introduzca el siguiente prompt de despacho industrial:

```
Actúa como un Gerente de Operaciones y Logística de Distribución de Cerámicas. Basándote en el pedido de "Torres del Horizonte" (1,500 m² de Porcelanato Lítico y 800 m² de Cerámica Urbana), necesito estructurar una tabla de despacho para Excel.

Asume las siguientes constantes técnicas de empaque:
- 1 m² de Porcelanato Lítico pesa 22 kg. Una caja contiene 1.5 m². Un palé soporta máximo 1,200 kg.
- 1 m² de Cerámica Urbana pesa 16 kg. Una caja contiene 2.0 m². Un palé soporta máximo 1,000 kg.

Por favor, devuélveme una tabla para Excel con las siguientes columnas:
`| Producto | m² Totales | Total Cajas Requeridas | Peso Total (kg) | Número de Palés Necesarios (Redondeado al entero superior) |`
Al final de la tabla, calcula cuántos camiones de capacidad de 10 toneladas (10,000 kg) se requieren para transportar la orden completa.
```

3. Copie la tabla generada por Copilot y péguela en la hoja `Cubicaje Logístico` en la celda `A1`.

---

### Fase D: Redacción de Contrato de Preventa y Reserva de Stock (Word) 
*(Nueva Tarea)* En el negocio de acabados, las constructoras exigen un documento formal que garantice que la fábrica congelará los lotes de producción para asegurar la uniformidad del tono y el calibre de la cerámica. Trasladaremos el flujo a Word.

1. Abra su archivo de **Word** (`Plantillas_Envio_Cotizacion.docx`) y escriba como título principal: `# Documentación de Cierre Comercial y Operativo`.
2. Regrese al chat de Copilot e introduzca el siguiente prompt de redacción de contratos comerciales:

```
Actúa como un Director de Contratos Comerciales e Ingeniería de Valor. Necesito redactar un "Acuerdo de Reserva Técnica de Stock y Uniformidad de Tono" para el proyecto "Torres del Horizonte".

Por favor, redáctame un documento formal de 3 secciones para mi archivo de Word:
1. **Cláusula de Garantía de Tono y Calibre**: Explicación técnica de cómo la fábrica reservará el mismo lote de producción para evitar variaciones de color entre las torres.
2. **Compromiso de Retiros Programados**: Establece que el constructor se compromete a retirar el material en un plazo máximo de 90 días calendario alineado con las fases de vaciado de acabados en la obra.
3. **Condición de Penalización por Incumplimiento**: Si el constructor cancela la orden una vez fabricada, perderá el 15% del anticipo por concepto de re-almacenamiento y costo de oportunidad.
```

3. Copie el texto legal-comercial y péguelo en su archivo de **Word**.

---

### Fase E: Plantilla de Correo y Formato de Salida Uniforme para PDF (Word) 
Estructuraremos la notificación formal de despacho y las reglas de diseño para que el PDF final sea visualmente impecable.

1. En el mismo documento de **Word**, cree una sección titulada `## Comunicación Formal de Oferta`.
2. Ejecute el siguiente prompt en Copilot:

```
Actúa como un Líder de Operaciones Comerciales. Basándote en las cifras financieras de la Fase B y los datos de palés de la Fase C, redáctame dos apartados para Word:
1. **Borrador de Correo Electrónico**: Un mensaje persuasivo y ejecutivo para el Director de Compras de "Torres del Horizonte" adjuntando la oferta, resumiendo los subtotales netos y detallando la logística de despacho (número de camiones/palés).
2. **Checklist para PDF Uniforme**: 4 puntos clave de diseño que el equipo debe validar en Word antes de guardar como PDF (márgenes fijos, logo en alta resolución, tipografías institucionales y pie de página legal) para que todas las propuestas de la fábrica se vean idénticas y profesionales.
```

3. Copie el resultado y péguelo en Word debajo de la sección creada.

---

### Fase F: Reto de Aplicación Autónoma – Cláusula de Ajuste por Fluctuación Cambiaria 

**Instrucciones para el estudiante:** Has completado la automatización avanzada del flujo. Ahora te enfrentas a una variable macroeconómica crítica e imprevista: el porcelanato de tu catálogo utiliza arcillas y esmaltes importados, y el tipo de cambio de la divisa extranjera ha fluctuado un 8% al alza esta semana. Tu cotización corre el riesgo de perder margen si el cliente tarda más de 5 días en firmar.

#### El Desafío:
Debes utilizar ingeniería de prompts por tu cuenta de forma totalmente independiente para obligar a Copilot a diseñar una **Cláusula de Salvaguarda Cambiaria y Recalculador de Emergencia** que proteja la rentabilidad de la empresa.

#### Pistas de Ingeniería de Prompts para el Éxito:
Diseña un prompt avanzado en el chat asegurando incluir:
* **Rol de Alta Competencia:** Ordena a Copilot actuar como un *Especialista en Gestión de Riesgo Comercial y Contratos de Suministro*.
* **El Requerimiento Técnico para Word:** Pídele que redacte una cláusula formal de validez cambiaria donde se estipule que los precios del PDF están atados a la tasa del día de emisión y que variaciones mayores al 3% anulan la oferta original.
* **Formato de Salida para Excel:** Pídele que te dibuje una estructura de tabla con fórmulas lógicas para tu archivo de Excel que permita ingresar el `| Tipo de Cambio Inicial | Tipo de Cambio Actual | % de Variación | Nuevo Precio Ajustado |` para recalcular los precios si se vence el plazo.

#### Cierre del Laboratorio:
1. Copie la tabla cambiaria autónoma y péguela en una nueva hoja de su archivo de **Excel** llamada `Riesgo Cambiario` en la celda `A1`.
2. Copie la cláusula legal y péguela al final de su archivo de **Word** bajo el título `## Anexo Técnico: Cláusula de Estabilidad Financiera`.
3. Guarde y cierre ambos archivos (`Calculador_Costos_Cotizaciones.xlsx` y `Plantillas_Envio_Cotizacion.docx`). Su ecosistema integral de cotizaciones está finalizado.

---

## 6. Conceptos Clave para Recordar

* **Gobernanza de Reglas de Negocio en Ventas:** Automatizar procesos comerciales con IA requiere alimentar al sistema con reglas claras. Copilot actúa como un auditor veloz que evita errores humanos de cálculo en propuestas de alto volumen.
* **Sincronización Logístico-Comercial:** En el sector industrial de acabados, cotizar m² sin calcular el peso de la carga (cubicaje) es un error crítico. Integrar camiones y palés en la oferta inicial eleva la transparencia y la confianza con los constructores.
* **Consistencia de Marca mediante PDFs Uniformes:** El PDF final es el rostro de la empresa. Establecer directrices estrictas de maquetación en Word asegura que la automatización no sacrifique la elegancia institucional.

---

## 7. Resultado Esperado

Al finalizar los 90 minutos de la sesión práctica, el estudiante entregará dos archivos completados:

1. **Archivo `Calculador_Costos_Cotizaciones.xlsx` (Excel):**
   * **Hoja 1 (`Simulador de Costeo`):** Matriz analítica con costos base, márgenes del 40% y fórmulas de PVP con mermas mecánicas.
   * **Hoja 2 (`Cubicaje Logístico`):** Tabla de distribución física con cajas, pesos y total de camiones de 10 toneladas requeridos.
   * **Hoja 3 (`Riesgo Cambiario`):** Estructura del **Reto Autónomo** para indexar variaciones de divisas.
2. **Archivo `Plantillas_Envio_Cotizacion.docx` (Word):**
   * El acuerdo formal de Reserva Técnica de Stock y uniformidad de lotes.
   * El borrador de correo formal con el desglose financiero y logístico para el constructor.
   * El checklist de diseño y maquetación para asegurar PDFs uniformes.
   * **Anexo Autónomo:** La cláusula de estabilidad cambiaria para blindar jurídicamente la propuesta económica.

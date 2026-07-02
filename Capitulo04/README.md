# Simulación de Precios y Reportes

## 1. Metadatos del Laboratorio

| Atributo | Detalle |
| :--- | :--- |
| **Duración** | 90 minutos (Guiado + Reto de Aplicación Autónoma de Alta Densidad) |
| **Complejidad** | Avanzada |
| **Audiencia** | Directores de Ventas, Key Account Managers (KAM), Analistas de Operaciones Comerciales y Gerentes de Expansión |
| **Tecnologías** | Microsoft Copilot Chat (M365), Microsoft Excel y Microsoft Word |
| **Enfoque** | Simulación de escenarios de precios, impacto de descuentos en el margen y comparativos de rentabilidad por proyecto. Automatización de reportes semanales y optimización de rutas de visitas. |

---

## 2. Descripción Corta

Este laboratorio práctico de 90 minutos capacita a los profesionales comerciales del sector de acabados arquitectónicos en el uso estratégico de la IA para proteger la salud financiera de la operación. Los estudiantes aprenderán a orquestar prompts avanzados con Microsoft Copilot para simular el impacto real de otorgar descuentos masivos sobre el margen de contribución neta en **Microsoft Excel**. Adicionalmente, realizarán análisis de sensibilidad de volumen, estructurarán rutas lógicas de visitas técnicas a obras por proximidad geográfica y automatizarán la redacción de informes ejecutivos semanales utilizando **Microsoft Word**.

---

## 3. Objetivos del Laboratorio

Al finalizar este laboratorio, el estudiante será capaz de:
* **Simular múltiples escenarios de precios en Excel** evaluando cómo impactan los descuentos comerciales directos a la utilidad neta de la fábrica.
* **Construir análisis comparativos de rentabilidad cruzada** entre diferentes proyectos institucionales concurrentes.
* **Calcular la elasticidad de margen en Excel** para determinar el volumen de compensación requerido ante variaciones de precio.
* **Optimizar agendas e itinerarios geográficos de visitas a obras** basándose en criterios de prioridad de cuenta y proximidad para reducir tiempos muertos.
* **Automatizar la redacción de reportes semanales ejecutivos en Word** traduciendo métricas densas de Excel en narrativas estratégicas para la alta gerencia.

---

## 4. Prerrequisitos

* Cuenta activa de **Microsoft 365** con acceso a **Copilot Chat**.
* Aplicación de **Microsoft Excel** abierta con un libro en blanco guardado como `Analitica_Rentabilidad_Rutas.xlsx`.
* Aplicación de **Microsoft Word** abierta con un documento en blanco guardado como `Reporte_Semanal_Direccion.docx`.

---

## 5. Procedimiento Paso a Paso (Flujo de Inteligencia Comercial y Control)

### Fase A: Simulador de Impacto de Descuentos en el Margen (Excel) 
En grandes proyectos de revestimientos, conceder una rebaja de $1 o $2 dólares por metro cuadrado para ganar un volumen puede destruir la rentabilidad del negocio. Diseñaremos una matriz de simulación de escenarios financieros en Excel.

1. En su libro de Excel, nombre la primera hoja como `1. Simulación_Márgenes`.
2. Vaya al chat de **Copilot** e introduzca el siguiente prompt de ingeniería financiera comercial:

```
Actúa como un Director de Operaciones Financieras y Control de Gestión Comercial en la industria de recubrimientos (porcelanatos y cerámicas). Necesito organizar una matriz en Excel para evaluar el impacto de tres políticas de descuento sobre una orden base de 5,000 m² de Porcelanato Premium.

Datos Base:
- Precio de Venta Público (PVP) de lista: $25 USD por m².
- Costo de Producción y Operación de la fábrica: $15 USD por m².

Por favor, devuélveme una tabla limpia diseñada para Excel que compare los siguientes 3 escenarios en columnas o filas según corresponda:
1. Escenario A (Precio de Lista): 0% de descuento.
2. Escenario B (Descuento Corporativo): 5% de descuento.
3. Escenario C (Descuento de Cierre Agresivo): 12% de descuento.

La tabla debe incluir para cada escenario el cálculo con las siguientes columnas exactas:
`| Escenario | Precio m² Ajustado | Ingreso Bruto Total | Costo Operativo Total | Margen de Contribución Total ($) | Porcentaje de Margen Neto (%) |`
Asegúrate de mostrar claramente las fórmulas conceptuales (ej: Margen % = (Ingreso - Costo) / Ingreso) para asegurar su fácil replicación en la hoja de cálculo.
```

3. Seleccione la tabla simulada generada por Copilot.
4. Cópiela (`Ctrl+C`), vaya a su archivo de **Excel**, posiciónese en la celda `B3` de la hoja `1. Simulación_Márgenes` y péguela.

---

### Fase B: Comparativo de Rentabilidad Inter-Proyecto (Excel)
El equipo comercial debe priorizar la asignación de inventario de fábrica hacia los proyectos que dejen mayor rendimiento económico y no hacia los que tengan mayor volumen pero menor margen.

1. En su libro de Excel, cree una segunda hoja y nómbrela `2. Rentabilidad_Proyectos`.
2. Regrese al chat de Copilot e introduzca el siguiente prompt de análisis comparativo:

```
Actúa como un Controller Comercial de Cuentas Clave. Necesito estructurar un reporte comparativo en Excel para auditar la rentabilidad de 3 proyectos inmobiliarios que nos están solicitando suministro de material simultáneamente.

Por favor, devuélveme una tabla formateada para Excel con la siguiente información para las filas:
1. **Proyecto A (Torres de la Costa)**: Volumen pedido: 8,000 m² de Azulejo Cerámico. Margen neto dejado: 28%.
2. **Proyecto B (Centro Comercial Platinum)**: Volumen pedido: 3,500 m² de Porcelanato de Tráfico Pesado. Margen neto dejado: 42%.
3. **Proyecto C (Complejo Hospitalario Norte)**: Volumen pedido: 2,000 m² de Mosaico Sanitario Especializado. Margen neto dejado: 51%.

Estructura la tabla con las columnas:
`| Nombre del Proyecto | Producto Solicitado | Volumen (m²) | Margen Neto (%) | Prioridad de Despacho (Asigna 'Alta', 'Media' o 'Baja' basándote en la combinación de rentabilidad y volumen) | Justificación Estratégica del Porqué |`
```

3. Copie la tabla comparativa entregada por Copilot.
4. Vaya a la hoja `2. Rentabilidad_Proyectos` en **Excel** y péguela a partir de la celda `B3`.

---

### Fase C: Análisis de Sensibilidad y Elasticidad de Margen (Excel) 
*(Nueva Tarea)* Si reducimos el precio para asegurar un contrato, el volumen vendido debe crecer para mantener la misma masa de dólares de ganancia. Utilizaremos a Copilot para calcular el "Volumen de Compensación Mínimo" requerido ante variaciones de precio.

1. En su libro de Excel, cree una tercera hoja llamada `3. Análisis_Sensibilidad`.
2. Vaya al chat de Copilot e introduzca el siguiente prompt de elasticidad comercial:

```
Actúa como un Consultor de Estrategia de Pricing. Basándote en el Escenario C de la Fase A (Descuento del 12%, lo que reduce el margen de contribución de $10 USD a $7 USD por m²), necesito construir una tabla en Excel que calcule cuánto volumen extra debemos venderle al constructor para no ganar menos dinero que en el Escenario A original (donde la ganancia total esperada era de $50,000 USD).

Por favor, devuélveme una estructura de tabla para Excel con las siguientes columnas:
`| Escenario Financiero | Margen Unitario ($) | Ganancia Total Objetivo | m² Requeridos para Alcanzar el Objetivo (Fórmula: Ganancia / Margen Unitario) | % de Incremento Necesario en Esfuerzo de Ventas |`
Incluye una breve explicación metodológica de cómo un descuento lineal del 12% exige un aumento de volumen significativamente mayor en términos porcentuales para alcanzar el punto de equilibrio original.
```

3. Copie la tabla resultante y péguela en la hoja `3. Análisis_Sensibilidad` en la celda `B3`.

---

### Fase D: Optimización Logística de Rutas de Visitas Técnicas (Excel)
Los Key Account Managers del sector de recubrimientos pasan gran parte de su tiempo visitando frentes de obra para validar avances, revisar mermas y asesorar a los instaladores. Utilizaremos a Copilot para diseñar una ruta de visitas óptima en el mapa de operaciones que minimice los traslados mecánicos.

1. En su libro de Excel, cree una cuarta hoja llamada `4. Optimización_Rutas`.
2. Vaya al chat de Copilot e introduzca el siguiente prompt de eficiencia en campo:

```
Actúa como un Especialista en Excelencia Operacional y Logística de Rutas Comerciales. Un KAM Senior de acabados tiene que visitar 4 frentes de obra críticos esta semana en la zona metropolitana para verificar la correcta colocación de los porcelanatos y retener cuentas en riesgo.

Por favor, organízame un itinerario lógico y optimizado de visitas en una tabla para Excel. Usa los siguientes datos de las obras:
- Obra 1: "Residencias Alameda" (Ubicación: Sector Norte). Prioridad: Alta (Presenta quejas por rotura de material).
- Obra 2: "Plaza Comercial Sur" (Ubicación: Sector Sur). Prioridad: Media (Validación de inicio de fase de acabados).
- Obra 3: "Centro Ejecutivo Empresarial" (Ubicación: Sector Centro). Prioridad: Alta (Firma de adición de volumen).
- Obra 4: "Condominio Los Robles" (Ubicación: Periferia Norte). Prioridad: Baja (Visita de seguimiento de rutina).

Estructura el itinerario secuencial de lunes a jueves en una tabla con las columnas:
`| Día | Destino (Obra) | Sector Geográfico | Nivel de Prioridad | Objetivo de la Visita Técnica | Estrategia de Traslado (Indica cómo agrupar las visitas del Sector Norte y Periferia Norte consecutivamente para evitar cruzar la ciudad dos veces) |`
```

3. Seleccione el itinerario optimizado, cópielo y péguelo en la hoja `4. Optimización_Rutas` en la celda `B3`.

---

### Fase E: Automatización del Reporte Semanal para la Dirección (Word) 
Con toda la analítica consolidada y las rutas en marcha, el comercial debe presentar los resultados semanales a la gerencia general. Utilizaremos el procesamiento de texto de Copilot para traducir los datos tabulares de Excel en un reporte narrativo formal en Word.

1. Abra su archivo de **Word** (`Reporte_Semanal_Direccion.docx`) y escriba como título principal: `# Reporte Ejecutivo de Control Comercial, Rentabilidad y Productividad en Obras`.
2. Regrese al chat de Copilot e introduzca el siguiente prompt avanzado de redacción corporativa:

```
Actúa como un Gerente de Ventas Regional del Canal Institucional de Acabados. Necesito redactar un informe ejecutivo conciso y formal de 3 secciones para la Junta Directiva, consolidando los análisis numéricos y geográficos que estructuramos en los pasos anteriores (Fases A, B, C y D).

Por favor, genera el reporte para mi archivo de Word siguiendo este esquema formal:
1. **Resumen Ejecutivo de Protección de Márgenes e Impacto de Descuentos (Fases A y C)**: Un párrafo analítico que alerte a la junta sobre el peligro de aprobar descuentos del 12%, demostrando numéricamente que nos obliga a vender un 42.8% más de metros cuadrados solo para mantener la misma ganancia en dólares.
2. **Diagnóstico de Priorización de Inventarios (Fase B)**: Un párrafo estratégico que explique por qué se ordenó dar prioridad de despacho al "Centro Comercial Platinum" y al "Complejo Hospitalario" por encima de "Torres de la Costa", justificando la decisión basada en la rentabilidad neta por m².
3. **Indicador de Productividad de Campo y Eficiencia de Traslados (Fase D)**: Un párrafo operativo que resuma el plan de optimización de rutas de la semana, destacando el ahorro estimado en tiempos de viaje y viáticos al agrupar geográficamente los proyectos de la zona Norte.
```

4. Copie el texto de alta densidad ejecutiva devuelto por Copilot y péguelo en su documento de **Word** justo debajo del título principal.

---

### Fase F: Reto de Aplicación Autónoma – Simulación de Escenario de Guerra de Precios

**Instrucciones para el estudiante:** Has dominado la analítica estándar. Ahora el laboratorio te lanza un reto de alta presión: un agresivo competidor internacional acaba de entrar a la licitación del proyecto más rentable ("Centro Comercial Platinum") ofreciendo precios de remate que están un 20% por debajo de tus costos de fabricación actuales. La junta te exige un análisis de contramedidas financieras inmediato para ver si es viable igualar la oferta o si es mejor retirarse.

#### El Desafío:
Debes utilizar ingeniería de prompts por tu cuenta de forma totalmente independiente para obligar a Copilot a diseñar un **Análisis de Punto de Equilibrio y Defensa Estratégica de Margen**. Tu meta es demostrarle numéricamente a la junta por qué bajar el precio a ese nivel destruiría el punto de equilibrio y proponer una salida corporativa de valor.

#### Pistas de Ingeniería de Prompts para el Éxito:
Diseña un prompt avanzado en el chat asegurando incluir:
* **Rol de Blindaje Financiero:** Ordena a Copilot actuar como un *Consultor de Estrategia de Precios (Pricing) y Gestión de Crisis Financiera*.
* **El Requerimiento Analítico para Excel:** Pídele que dibuje una estructura tabular de simulación extrema donde demuestre el `| Margen de Pérdida Directa por m² |` si se aceptara esa rebaja del 20%, calculando el volumen adicional absurdo que se tendría que vender solo para cubrir los costos fijos.
* **El Requerimiento Técnico-Comercial para Word:** Solicítale un párrafo de copy estratégico (Argumento de Calidad Industrial) que el vendedor usará para convencer a los desarrolladores del Centro Comercial de que el material importado a precio de remate fallará bajo el tráfico pesado del centro comercial en menos de 6 meses, generando un sobrecosto millonario de reparación.

#### Cierre del Laboratorio:
1. Copie la tabla de simulación de crisis financiera generada por Copilot y péguela en una nueva hoja de su archivo de **Excel** llamada `5. Análisis_Punto_Equilibrio` en la celda `B3`.
2. Copie el argumento técnico de defensa ante guerra de precios y péguelo al final de su archivo de **Word** bajo el título `## Anexo Técnico: Plan de Defensa contra Guerra de Precios y Dumping`.
3. Guarde y cierre ambos archivos (`Analitica_Rentabilidad_Rutas.xlsx` y `Reporte_Semanal_Direccion.docx`). Su maletín de control financiero comercial y excelencia en campo está completo y listo para auditoría.

---

## 6. Conceptos Clave para Recordar

* **Erosión Silenciosa del Margen:** Otorgar descuentos en el sector B2B institucional de acabados de forma deliberada altera severamente el punto de equilibrio. El uso de matrices analíticas en Excel automatizadas por IA le da la capacidad al equipo de ventas de negociar con datos duros y no con corazonadas.
* **Optimización Territorial Lógica:** El tiempo que un asesor pasa atrapado en el tráfico cruzando la ciudad de un extremo a otro es tiempo perdido de venta. Agrupar visits por sectores geográficos eleva la productividad técnica de la fuerza de ventas.
* **Traducción de Datos a Narrativa Gerencial:** Los directivos de las organizaciones no leen hojas de cálculo crudas en su día a día; buscan conclusiones accionables. El uso estratégico de Word guiado por Copilot agiliza el flujo de gobernanza e informes dentro de la compañía.

---

## 7. Resultado Esperado

Al finalizar los 90 minutos de la práctica, el estudiante entregará dos archivos completados:

1. **Archivo `Analitica_Rentabilidad_Rutas.xlsx` (Excel):**
   * **Hoja 1 (`1. Simulación_Márgenes`):** Matriz que detalla la reducción exacta de los márgenes netos de contribución frente a los escenarios de descuento del 0%, 5% y 12%.
   * **Hoja 2 (`2. Rentabilidad_Proyectos`):** Tabla con la priorización estratégica y técnica de asignación de stock basándose en el retorno de inversión por proyecto.
   * **Hoja 3 (`3. Análisis_Sensibilidad`):** Matriz que calcula el volumen incremental obligatorio para compensar el sacrificio en el precio unitario.
   * **Hoja 4 (`4. Optimización_Rutas`):** Itinerario secuencial semanal que agrupa y optimiza geográficamente las visitas técnicas a obra.
   * **Hoja 5 (`5. Análisis_Punto_Equilibrio`):** Entregable numérico del **Reto Autónomo** que modela el peligro financiero de ceder ante ofertas de remate de la competencia.
2. **Archivo `Reporte_Semanal_Direccion.docx` (Word):**
   * Un reporte comercial ejecutivo formal de alta densidad analítica, redactado a nivel dirección, que justifica las decisiones de precios, inventarios, sensibilidad de volumen y rutas ante la junta gerencial de la empresa.
   * **Anexo Autónomo:** El argumento técnico-comercial y normativo de tráfico pesado listo para desarmar la oferta económica del competidor de bajo costo en el proyecto insignia.

# Investigación de competidores y clientes potenciales mediante IA

## 1. Metadatos del Laboratorio

| Atributo | Detalle |
| :--- | :--- |
| **Duración** | 60 minutos (Guiado + Reto de Aplicación Autónoma) |
| **Complejidad** | Intermedia  |
| **Audiencia** | Directores de Ventas, Ejecutivos de Cuenta B2B (KAM), y Gerentes de Desarrollo de Negocios |
| **Tecnologías** | Microsoft Copilot Chat (M365) y Microsoft Excel (Escritorio o Web) |
| **Enfoque** | Investigación de competidores y clientes potenciales mediante IA. Identificación de necesidades operativas, puntos de dolor y preparación rápida para reuniones comerciales con argumentos técnicos listos. |

---

## 2. Descripción Corta

Este laboratorio práctico entrena a los profesionales de ventas en el uso de Microsoft Copilot para acelerar la fase de preventa e inteligencia comercial. Los estudiantes aprenderán a estructurar prompts que fuercen a la IA a investigar perfiles de clientes corporativos, desglosar sus dolores operativos ocultos frente a la competencia y armar un maletín de argumentos técnicos personalizado para una reunión de alto nivel. Toda la información estratégica se consolidará en una matriz comercial en Excel mediante copiado directo, eliminando el tipeo manual.

---

## 3. Objetivos del Laboratorio

Al finalizar este laboratorio, el estudiante será capaz de:
* **Ejecutar estrategias de investigación de mercado express** utilizando la IA para perfilar cuentas clave (Key Accounts) y su ecosistema competitivo.
* **Mapear de forma precisa los puntos de dolor (Pain Points)** y las brechas operativas de un cliente potencial basándose en su sector industrial.
* **Estructurar un 'Pitch de Ventas Técnico' a la medida**, utilizando prompts de simulación de objeciones comerciales.
* **Diseñar un Cuadro de Mando de Preparación de Cuentas en Excel**, usando exclusivamente la exportación nativa de tablas desde el chat.

---

## 4. Prerrequisitos

* Cuenta activa de **Microsoft 365** con acceso a **Copilot Chat**.
* Aplicación de Microsoft Excel abierta con un libro nuevo guardado como `Inteligencia_Comercial_Copilot.xlsx`.

---

## 5. Procedimiento Paso a Paso (Flujo de Orquestación Comercial)

### Fase A: Perfilamiento del Cliente Potencial y Competidores
Para abrir una cuenta B2B grande, no basta con saber qué vende el cliente; se necesita entender su posicionamiento. En esta fase, utilizaremos a Copilot para analizar un cliente objetivo (para este caso, una empresa mediana en proceso de expansión logística en Latinoamérica) y mapear su entorno competitivo.

1. En su libro de Excel, renombre la primera pestaña como **"1. Inteligencia_de_Cuenta"**.
2. Vaya al chat de **Copilot** e introduzca el siguiente prompt de investigación comercial:

```
Actúa como un Director de Inteligencia Comercial y Estratega de Ventas B2B Enterprise. Necesito perfilar a un cliente potencial de la industria de Consumo Masivo / Logística que está buscando expandir sus operaciones en la región andina durante este año 2026. 

Por favor, proporcióname una TABLA MARKDOWN única (usando barras '|' y guiones) que contenga exactamente 5 empresas ficticias pero realistas que encajen en este perfil de "Cliente Ideal". Es obligatorio que la tabla se renderice de forma visual nativa en la pantalla del chat (no uses bloques de código gris) para que pueda copiarla directamente a Excel.

Usa la siguiente estructura de columnas:
| CLIENTE_ID | NOMBRE_EMPRESA | PAÍS_MATRIZ | VOLUMEN_ENVÍOS_MES | PRINCIPAL_COMPETIDOR_SECTOR | BRECHA_TECNOLÓGICA_DETECTADA |

Asegúrate de que en la columna 'BRECHA_TECNOLÓGICA_DETECTADA' menciones problemas críticos como: 'Sistemas legados desconectados', 'Falta de visibilidad de última milla', o 'Dependencia de procesos manuales en almacén'.
```

3. Seleccione con el cursor la tabla de inteligencia que Copilot desplegó en el chat.
4. Cópiela (`Ctrl+C`), sitúese en la celda **B3** de la pestaña "1. Inteligencia_de_Cuenta" en Excel y péguela (`Ctrl+V`).

---

### Fase B: Ingeniería de Puntos de Dolor y Argumentación Técnica
Una vez identificados los clientes potenciales y sus brechas, el vendedor moderno debe preparar la reunión comercial. Obligaremos a Copilot a procesar los datos de la Fase A para extraer los dolores operativos y convertirlos en argumentos de venta técnicos e irrefutables.

1. Cree una segunda pestaña en su archivo de Excel y llámela **"2. Preparacion_Reunion"**.
2. Regrese al chat de Copilot e introduzca el siguiente prompt de ingeniería de valor:

```
Actúa como un Ingeniero de Soluciones (Solution Engineer) y Consultor Comercial de Tecnología. Basándote en las 5 empresas y sus brechas tecnológicas analizadas en el paso anterior, necesito armar la estrategia de ataque para las reuniones comerciales.

Por favor, devuélveme una NUEVA TABLA MARKDOWN VISUAL NATIVA en el chat que conecte cada empresa con su estrategia técnica de ventas. La estructura debe ser la siguiente:
| NOMBRE_EMPRESA | PUNTO_DE_DOLOR_OPERATIVO | IMPACTO_FINANCIERO_DEL_PROBLEMA | ARGUMENTO_TÉCNICO_DE_NUESTRA_SOLUCIÓN | MÉTRICA_DE_ÉXITO_PROMETIDA |

Reglas para la argumentación:
- El 'Punto de Dolor Operativo' debe derivarse directamente de la brecha detectada en la Fase A.
- El 'Impacto Financiero' debe explicar cuánta eficiencia o dinero pierde el cliente por no solucionar el problema (ej: Costos de inventario +20%).
- El 'Argumento Técnico' debe redactarse vendiendo una solución moderna de automatización con IA y APIs de integración.
- La 'Métrica de Éxito' debe ser un indicador de negocio cuantificable (ej: Reducción del 35% en tiempos de entrega).
```

3. Seleccione la tabla de argumentos generada por Copilot.
4. Cópiela (`Ctrl+C`), vaya a la pestaña **"2. Preparacion_Reunion"** en Excel, haga clic en la celda **B3** y péguela (`Ctrl+V`).
5. Amplíe las columnas en Excel para que los argumentos técnicos queden perfectamente legibles.

---

### Fase C: Generación de Guías Rápidas de Preparación (Briefing de Reunión)
El Director de Ventas necesita un resumen ejecutivo en texto plano antes de entrar a la llamada con el cliente corporativo. Le pediremos a Copilot que redacte una guía de preparación exprés para la empresa de la lista que presente los dolores más complejos.

1. En el mismo hilo de conversación con Copilot, ejecute el siguiente prompt de habilitación comercial:

```
Actúa como un Account Executive Senior. Selecciona la empresa de la tabla anterior que consideres que tiene la brecha operativa más crítica y urgente de resolver. 

Redacta una Guía de Preparación de Reunión de 3 párrafos de alta densidad estratégica para el equipo comercial, usando el siguiente esquema formal:
1. **Objetivo de la Reunión y Perfil del Interlocutor**: Define la meta de la primera llamada y cómo enganchar al Director de Operaciones (COO) tocando sus fibras estratégicas.
2. **Guión de Apertura (Hook) y Preguntas de Diagnóstico**: Un texto literal e impactante de 3 líneas para iniciar la conversación y 3 preguntas abiertas que forzarán al cliente a admitir su dolor operativo.
3. **Manejo Técnico de Objeciones**: Anticípate a la objeción típica: "Ya tenemos un software interno que hace algo similar" o "No tenemos presupuesto este trimestre", y redacta una respuesta elegante, técnica y orientada al Retorno de Inversión (ROI).
```

2. Copie el texto de la guía de preparación devuelto por Copilot.
3. Regrese a la pestaña **"2. Preparacion_Reunion"** de Excel y péguelo directamente a partir de la celda **B12** (justo debajo de la tabla de argumentos).

---

### Fase D: Reto de Aplicación Autónoma – Matriz de Contramedidas Competitivas (15 minutos)

**Instrucciones para el estudiante:** Hasta este punto has seguido una estructura guiada. Ahora te enfrentas a un cambio de escenario de última hora. El cliente te acaba de informar que se está reuniendo simultáneamente con tu principal competidor global.

#### El Desafío:
Debes usar ingeniería de prompts por tu cuenta para obligar a Copilot a construir una **Matriz de Bloqueo de Competidores (Battlecard Express)** basada en los perfiles de la Fase A y B. El objetivo es blindar tu propuesta comercial frente a alternativas de bajo costo.

#### Pistas de Ingeniería de Prompts para el Éxito:
Diseña un prompt avanzado en el chat considerando las siguientes pautas de defensa comercial:
* **Rol Avanzado:** Ordena a Copilot actuar como un *Especialista en Inteligencia Competitiva (Competitive Intelligence) y Ventas de Alto Impacto*.
* **Definición del Escenario:** Explícale que el competidor del sector (mencionado en tu tabla de la Fase A) está ofreciendo un descuento del 30% en una herramienta genérica, pero que carece de integraciones nativas de IA y procesamiento en tiempo real.
* **Estructura Requerida:** Exígele a la IA que procese la información y te entregue una **Tabla Markdown Visual Nativa** con las columnas: `| NOMBRE_EMPRESA | Ventaja_Crítica_Nuestra | Punto_Débil_del_Competidor | Pregunta_Trampa_para_el_Cliente |`. 
  *(Nota: La "Pregunta Trampa" es una pregunta sutil que el vendedor le hará al cliente para sembrar la duda sobre las capacidades técnicas del competidor).*

#### Cierre del Laboratorio:
1. Copie la tabla de contramedidas competitivas generada de forma autónoma por Copilot y pégala en una nueva pestaña llamada **"3. Estrategia_Competitiva"**, iniciando en la celda **B3**.
2. Dale un formato visual profesional a los encabezados en Excel para concluir el entregable.

---

## 6. Conceptos Clave para Recordar

* **Venta Consultiva Habilitada por IA:** El uso de Copilot para diagnosticar problemas operativos antes de la primera interacción desplaza al vendedor tradicional y posiciona al comercial como un consultor técnico de confianza.
* **Puntos de Dolor Cuantificables:** Un argumento de ventas técnico solo es efectivo si se conecta directamente con el impacto financiero (dinero perdido) y una métrica de éxito clara (ROI). La IA destaca en realizar estas correlaciones sectoriales de manera inmediata.
* **Velocidad de Preparación (Speed to Market):** Reducir el tiempo de investigación de cuentas de horas a minutos mediante prompts relacionales permite a los equipos comerciales duplicar su volumen de prospección diaria manteniendo la hiper-personalización en cada mensaje.

---

## 7. Resultado Esperado

Al finalizar los 60 minutos de la sesión práctica, el estudiante guardará el archivo `Inteligencia_Comercial_Copilot.xlsx` estructurado de la siguiente forma:

1. **Pestaña "1. Inteligencia_de_Cuenta":** Contendrá la matriz con las 5 empresas target perfiladas junto con sus brechas logísticas y competidores (Rango B3:G8).
2. **Pestaña "2. Preparacion_Reunion":** Mostrará el arsenal de ataque guiado:
   * **Rango B3:F8:** La tabla de dolores operativos, impactos financieros y argumentos técnicos calculados por la IA.
   * **A partir de la celda B12:** El Briefing Ejecutivo con el guión de apertura, las preguntas de diagnóstico corporativo y el manejo avanzado de objeciones.
3. **Pestaña "3. Estrategia_Competitiva":** Presentará el entregable del **Reto Autónomo (Fase D)**: la matriz de contramedidas y preguntas trampa para bloquear el avance de los competidores del sector, lista para ser usada por el equipo comercial en el campo.

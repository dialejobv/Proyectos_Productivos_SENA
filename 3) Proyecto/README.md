# Prototipo Inicial de Agente Inteligente de Ingeniería Aeroespacial en la Era de los Sistemas Teleinformáticos
Desarrollo de proyecto orientado al comportamiento del agente inteligente que analiza las redes en la ingeniería aeroespacial.

<div align="center">
<pre>

┌─────────────────────────────┐
│ 1. Fuentes de datos         │
│  (telemetría satelital,     │
│   sensores, APIs NASA/ESA,  │
│   datos de misión)          │
└──────────────┬──────────────┘
│
▼
┌─────────────────────────────┐
│ 2. Adquisición y            │
│    preprocesamiento         │
│  (limpieza, sincronización, │
│   formatos)                 │
└──────────────┬──────────────┘
│
▼
┌─────────────────────────────┐
│ 3. Almacenamiento           │
│  (data lake, time-series DB,│
│   PostgreSQL/InfluxDB)      │
└──────────────┬──────────────┘
│
▼
┌─────────────────────────────┐
│ 4. Módulo de IA             │
│  (ML/DL: predicción,        │
│   anomalías, optimización)  │
└──────────────┬──────────────┘
│
▼
┌─────────────────────────────┐
│ 5. Motor de razonamiento    │
│  (reglas + LLM/agente,      │
│   planificación)            │
└──────────────┬──────────────┘
│
▼
┌─────────────────────────────┐
│ 6. Módulo de comunicación   │
│  teleinformática            │
│  (telemetría, teleco-       │
│   municaciones, DTN,        │
│   enlaces satelitales)      │
└──────────────┬──────────────┘
│
▼
┌─────────────────────────────┐
│ 7. Interfaz de operador     │
│  (HMI, dashboard, chatbot,  │
│   alertas)                  │
└──────────────┬──────────────┘
│
▼
┌─────────────────────────────┐
│ 8. Módulo de acción/        │
│    control (comandos a      │
│    subsistemas, simulación) │
└─────────────────────────────┘

</pre>
</div>

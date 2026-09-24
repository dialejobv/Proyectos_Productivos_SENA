# Redes de Datos con Visión Computacional — Lenguaje de señas con MediaPipe
Desarrollo de un proyecto de visión computacional orientado a redes y al manejo de lenguaje de señas.

<div align="center">
<pre>

┌─────────────────────┐
│ 1. Captura de video │
│  (webcam/cámara)    │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 2. MediaPipe Hands  │
│  (detección de      │
│   landmarks 21 pts) │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 3. Extracción de    │
│    características  │
│  (coordenadas x,y,z,│
│   ángulos, distancias)│
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 4. Normalización y  │
│    secuenciación    │
│  (ventanas tempora- │
│   les, padding)     │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 5. Modelo de        │
│    clasificación    │
│  (LSTM/GRU/Transformer│
│   /MLP)             │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 6. Traducción a     │
│    texto/voz        │
│  (TTS, subtítulos)  │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 7. Empaquetado de   │
│    datos (JSON/     │
│    protobuf/MQTT)   │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 8. Red de datos     │
│  (switch/router,    │
│   TCP/UDP, QoS)     │
└──────────┬──────────┘
│
▼
┌─────────────────────┐
│ 9. Receptor/        │
│    aplicación final │
│  (dashboard, app)   │
└─────────────────────┘

</pre>
</div>
